<template>
  <section id="get-in-touch" class="overflow-hidden">
    <v-row class="info white--text" no-gutters>
      <v-col class="hidden-sm-and-down" md="6">
        <v-img :src="require('@/assets/contact.png')" height="100%" />
      </v-col>

      <v-col class="pa-5" cols="12" md="6">
        <base-bubble-1 />

        <base-heading class="mb-5">
          Conversemos
        </base-heading>

        <v-sheet color="transparent" max-width="600">
          <v-text-field
            color="info"
            label="Name"
            solo
            flat
            type="text"
            v-model="name"
            name="name"
            placeholder="Your Name"
          />

          <v-text-field
            color="info"
            label="Email"
            solo
            flat
            type="email"
            v-model="email"
            name="email"
            placeholder="Your Email"
          />

          <!-- <v-text-field color="info" label="Subject" solo flat /> -->

          <v-textarea
            color="info"
            label="Message"
            solo
            flat
            name="message"
            v-model="message"
            cols="30"
            rows="5"
            placeholder="Message"
          />

          <base-btn>Send</base-btn>
        </v-sheet>
      </v-col>
    </v-row>
  </section>
</template>

<script>
import emailjs from 'emailjs-com';
export default {
  name: 'GetInTouch',
  data() {
    return {
      name: '',
      email: '',
      message: '',
    };
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm(
          'service_sv2o3bn',
          'template_urnejgp',
          e.target,
          'user_bge1OFYxdvz0FHi1VDgnX',
          {
            name: this.name,
            email: this.email,
            message: this.message,
          }
        );
      } catch (error) {
        console.log({ error });
      }
      // Reset form field
      this.name = '';
      this.email = '';
      this.message = '';
    },
  },
};
</script>
