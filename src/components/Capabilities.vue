<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-4"></div>
      <div>
        <h1 class="text-center font-weight-bold mx-auto capability-color">
          CAPABILITIES
        </h1>
        <div class="mt-5 mb-4">
          <div>
            <h5 @click="straOpen = !straOpen">Strategy</h5>
            <h6 v-show="straOpen">Test | Test1 | Test2</h6>
          </div>
          <div>
            <h5 @click="designOpen = !designOpen">Design</h5>
            <h6 v-show="designOpen">
              Design1 | Design2 | Design3 | Design4 | Design5
            </h6>
          </div>
          <div>
            <h5 @click="digitalOpen = !digitalOpen">Digital</h5>
            <h6 v-show="digitalOpen">
              Design1 | Design2 | Design3 | Design4 | Design5
            </h6>
          </div>
          <div>
            <h5 @click="marketingOpen = !marketingOpen">Marketing</h5>
            <h6 v-show="marketingOpen">
              Design1 | Design2 | Design3 | Design4 | Design5
            </h6>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    straOpen: false,
    designOpen: false,
    digitalOpen: false,
    marketingOpen: false,
  }),
};
</script>
<style scoped>
.capability-color {
  color: rgb(227, 177, 12);
}
</style>
