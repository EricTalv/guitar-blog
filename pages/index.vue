<template>
   <b-container>
        <b-jumbotron header="BootstrapVue" lead="Bootstrap v4 Components for Vue.js 2">
          <p>For more information visit our website</p>
        </b-jumbotron>

        <b-form-group
          horizontal
          :label-cols="4"
          description="Let us know your name."
          label="Enter your name"
        >
          <b-form-input v-model.trim="name" v-on:keyup.enter="showAlert2"></b-form-input>
        </b-form-group>

        <b-alert variant="success" :show="showAlert">Hello {{ name }}</b-alert>
      </b-container>
</template>

<script>
export default {

    data() {
      return {
      };
    },
  
}
</script>

<style>
</style>
