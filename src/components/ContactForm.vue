<template>
  <form>
    <v-text-field
      v-model="name"
      :error-messages="nameErrors"
      :counter="40"
      label="Nombre"
      required
      @input="$v.name.$touch()"
      @blur="$v.name.$touch()"
    ></v-text-field>
    <v-text-field
      v-model="email"
      :error-messages="emailErrors"
      label="Correo"
      required
      @input="$v.email.$touch()"
      @blur="$v.email.$touch()"
    ></v-text-field>
     <v-textarea
          name="input-7-1"
          label="Mensaje"
          value="Ingresá tu mensaje acá..."
          hint="Te contactaremos a la brevedad."
        ></v-textarea>
    <v-checkbox
      v-model="checkbox"
      :error-messages="checkboxErrors"
      label="Desea suscribirse a nuestro newsletter?"
      required
      @change="$v.checkbox.$touch()"
      @blur="$v.checkbox.$touch()"
    ></v-checkbox>

    <v-btn class="mr-4 brown lighten-3 white--text" @click="submit">Enviar</v-btn>
  </form>
</template>

<script>
export default {
  name: 'ContactForm'
}
</script>
