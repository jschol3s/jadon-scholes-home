<template>
<div class="contact-section">
  <div class="content">
    <h2 class="content-head is-center">Hey, Let's chat.</h2>
  </div>
  <div class="pure-g">
    <div class="l-box-lrg pure-u-1 pure-u-md-2-5">
      <form class="pure-form pure-form-stacked" v-if='creating' @submit.prevent='sendMessage'>
        <fieldset>

          <label for="name">Your Name</label>
          <input v-model="name" type="text" placeholder="Your Name">


          <label for="email">Your Email</label>
          <input v-model="email" type="email" placeholder="Your Email">

          <label for="message">Your Message</label>
          <input v-model="message" type="text" placeholder="Your Message">

          <button @click="sendMessage(name, email, message)" type="submit" class="pure-button">Send</button>
        </fieldset>
      </form>
      <div v-else>
        <h3>Thanks for the message!</h3>
        <p>I will get back to you shortly 😊</p>
      </div>
    </div>

    <div class="l-box-lrg pure-u-1 pure-u-md-3-5">
      <h4>Contact Me</h4>
      <p>
        Have a job offer? Need a website? Just want to say hi? Feel free to reach out.
      </p>

      <h4>More Information</h4>
      <p>
        I'm based in Utah, and would prefer jobs and clients within the area. <br>
        However, I'm open to any outreach. I check my email and social media accounts frequently, <br>
        and I'll get back to you as soon as possible. Thanks!
      </p>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'create',
  data() {
    return {
      creating: true,
      name: '',
      email: '',
      message: '',
    }
  },
  methods: {
    toggleForm() {
      this.creating = !this.creating;
    },
    sendMessage() {
      this.$root.$data.sendMessage(this.name, this.email, this.message);
      this.creating = false;
    },
  }
}
</script>


<style>
.content-section {
  color: #93a8ac;
}

.pure-form label {
  margin: 1em 0 0;
  font-weight: bold;
  font-size: 100%;
}

.pure-form input[type] {
  border: 2px solid #ddd;
  box-shadow: none;
  font-size: 100%;
  width: 100%;
  margin-bottom: 1em;
}
</style>
