<template>
  <div>
    <keep-alive>
      <component v-bind:is="componentName"></component>
    </keep-alive>
    <button v-on:click="componentName = 'form-one'">Login</button>
    <button v-on:click="componentName = 'form-two'">Contact</button>
  </div>
</template>


<script>
  import formOne from './components/formOne.vue';
  import formTwo from './components/formTwo.vue';

  export default {
    components: {
      'form-one': formOne,
      'form-two': formTwo,
    },
    data(){
      return {
        componentName: 'form-two'
      }
    },
    methods: {

    }
  }
</script>

<style >
body{
  margin: 0;
  font-family: 'Nunito SemiBold';
}
</style>
