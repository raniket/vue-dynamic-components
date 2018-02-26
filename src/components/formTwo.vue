<template>
<div>
  <form-helper>
    <div slot='form-header'>
        <h2>Form-Two contact us</h2>
        <p>fill this form to contact us.</p>
    </div>

    <div slot='form-field'>
        <input type="text" placeholder="YoUr EmAiL" required>
        <label for="message">Message</label>
        <input type="text" id='message' placeholder="Your message" required>
    </div>

    <div slot='form-controls'>
        <button v-on:click='handleSubmit'>Contact</button>
    </div>
  </form-helper>
</div>
</template>

<script>
import formHelper from './formHelper';

export default {
  
  components: {
    'form-helper': formHelper,
  },
  data() {
    return {};
  },
  methods: {
    handleSubmit: function() {
      alert("thanks for submitting form one & contacting us");
    }
  }
};
</script>

<style>
body {
  margin: 0;
  font-family: "Nunito SemiBold";
}
</style>