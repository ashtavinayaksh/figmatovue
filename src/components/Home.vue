<template>
  <div class="header-main">
    <div class="jij-section">
      <nav class="row navbar">
        <div class="col-6"></div>
        <div class="col-6">
          <button
            class="hamburger-menu"
            type="button"
            @click="menuOpen = !menuOpen"
          >
            &#9776;
          </button>
        </div>
      </nav>
      <div class="row dropdown" :class="{ 'dropdown-after': menuOpen }">
        <ul class="navlist">
          <li class="navlistitem">
            <a href="#">home</a>
          </li>
          <li class="navlistitem">
            <a href="#">about</a>
          </li>
          <li class="navlistitem">
            <a href="#">contact</a>
          </li>
        </ul>
      </div>
    </div>

    <div class="container-fluid">
      <div class="row">
        <div class="col-2 align-self-center font-weight-bold">
          <div>
            TRUSTED <br />
            BY
          </div>
        </div>
        <div class="col-2 align-self-center text-center">
          <img src="../assets/imgpsh_fullsize_anim (1).png" />
        </div>
        <div class="col-2 align-self-center text-center">
          <img src="../assets/imgpsh_fullsize_anim (2).png" />
        </div>
        <div class="col-2 align-self-center text-center">
          <img src="../assets/imgpsh_fullsize_anim (3).png" />
        </div>
        <div class="col-2 align-self-center text-center">
          <img src="../assets/imgpsh_fullsize_anim (4).png" />
        </div>
        <div class="col-2 align-self-center text-center">
          <img src="../assets/imgpsh_fullsize_anim.png" />
        </div>
      </div>
      <hr />
      <div>
        <div class="row">
          <div class="col-4"></div>
          <div>
            <div class="font-weight-bold mx-auto description">
              MediaJenie is a 15+ Year old digital media agency.
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-4"></div>
          <div class="">
            <div class="font-weight-bold mx-auto description">
              We bring brands and customers closer through digital media
              experiences.
            </div>
          </div>
        </div>
      </div>
      <hr />
      <div class="row">
        <capabilities></capabilities>
      </div>
      <div class="row">
        <work></work>
      </div>
      <div class="row mt-5 mb-5 p-4">
        <div class="col-3">
          <h6 class="titleYellow">CASE STUDY</h6>
          <h5 class="font-weight-bold casestudy pt-3 pb-4">
            How a Us start-up genrated 250LK USD revenue in 1 year from website.
          </h5>
          <button class="cmnButton mt-4 pl-3 pr-3 pb-2 pt-2">Download</button>
        </div>
        <div class="col-3">
          <img src="../assets/imgpsh_fullsize_anim (8).png" height="300" />
        </div>
        <div class="col-4">
          <img src="../assets/imgpsh_fullsize_anim (5).png" height="200" />
          <h6 class="mt-1 titleYellow">ARTICLE</h6>
          <h6 class="font-weight-bold casestudyh6">
            How a Us start-up genrated 250LK USD revenue in 1 year from website.
          </h6>
        </div>
      </div>
      <div class="row">
        <Footer></Footer>
      </div>
    </div>
  </div>
</template>

<script>
import "@/assets/scss/style.scss";
import Work from "../components/Work.vue";
import Capabilities from "../components/Capabilities.vue";
import Footer from "../components/layouts/Footer.vue";

export default {
  components: {
    Work,
    Capabilities,
    Footer,
  },
  data: () => ({
    menuOpen: false,
    straOpen: false,
  }),
};
</script>
<style scoped>
.navbar {
  margin-right: 0px;
  background: transparent;
}

.description {
  letter-spacing: 0.5px;
  line-height: 2;
  font-size: 18px;
}

</style>
