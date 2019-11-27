<template>
<div style="height: 900px">
    <v-container>
  <ContactForm class="pa-5 ma-5"/>
    </v-container>
</div>
</template>

<script>
import ContactForm from './ContactForm'
export default {
  name: 'Contact',
  components: {
    ContactForm
  }
}
</script>
