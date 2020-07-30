<template>
  <div>
    <v-text-field v-model="name" label="Name" />
    <v-text-field v-model="codeNumber" label="Code Number" minlength="4" maxlength="4" />
    <v-btn @click="send">
      Send
    </v-btn>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: '',
      codeNumber: ''
    }
  },
  methods: {
    send () {
      alert(this.name + '\n' + this.codeNumber)
      this.name = ''
      this.codeNumber = ''
    }
  }
}
</script>
