<template>
  <p>{{ text }}</p>
</template>

<script>
export default {
  name: 'TextComponent',
  props: {
    text: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
p {
  color: #333;
}
</style>
