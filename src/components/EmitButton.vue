<template>
  <div>
    <h3>Emit Button Component</h3>
    <button-component @click="emitEvent"></button-component>
  </div>
</template>

<script>
import ButtonComponent from './ButtonComponent.vue'

export default {
  name: 'EmitButton',
  components: {
    ButtonComponent
  },
  methods: {
    emitEvent() {
      this.$emit('button-clicked', 'Button was clicked!')
    }
  }
}
</script>

<style scoped>
h3 {
  color: #35495e;
}
</style>
