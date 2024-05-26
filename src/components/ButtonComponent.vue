<template>
  <button @click="handleClick">Click me</button>
</template>

<script>
export default {
  name: 'ButtonComponent',
  methods: {
    handleClick() {
      this.$emit('click')
    }
  }
}
</script>

<style scoped>
button {
  background-color: #42b983;
  border: none;
  color: white;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
