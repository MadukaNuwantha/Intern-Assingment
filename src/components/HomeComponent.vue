<template>
  <div class="container-fluid">
    <div class="container bg-white rounded p-5">
      <h2 class="pb-4">Shape Finder</h2>
      <div class="row">
        <div class="col">
          <img
            src="../assets/Square.png"
            alt=""
            class="img-thumbnail"
            v-on:click="(id = '01'), (name = 'Square')"
          />
        </div>
        <div class="col">
          <img
            src="../assets/Circle.png"
            alt=""
            class="img-thumbnail"
            v-on:click="(id = '02'), (name = 'Circle')"
          />
        </div>
        <div class="col">
          <img
            src="../assets/Triangle.png"
            alt=""
            class="img-thumbnail"
            v-on:click="(id = '03'), (name = 'Triangle')"
          />
        </div>
      </div>
      <div class="row p-5 text-start">
        <div class="col">
          <label for="shape-name" class="form-lable">Selected Shape Name</label>
          <input
            id="shape-name"
            class="form-control"
            type="text"
            v-model="name"
          />
        </div>
        <div class="col">
          <label for="shape-id" class="form-lable">Selected Shape ID</label>
          <input id="shape-id" class="form-control" type="text" v-model="id" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "home-component",
  data() {
    return {
      id: null,
      name: null,
    };
  },
};
</script>
<style>
</style>