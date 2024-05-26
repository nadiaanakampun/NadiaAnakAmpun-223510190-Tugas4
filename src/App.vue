<template>
  <div id="app">
    <h1>Parent Component</h1>
    <slot-component>
      <emit-button @button-clicked="handleButtonClick"></emit-button>
    </slot-component>
    <p>{{ message }}</p>
  </div>
</template>

<script>
import SlotComponent from './components/SlotComponent.vue'
import EmitButton from './components/EmitButton.vue'

export default {
  name: 'App',
  components: {
    SlotComponent,
    EmitButton
  },
  data() {
    return {
      message: ''
    }
  },
  methods: {
    handleButtonClick(data) {
      this.message = data
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
