<template>
  <ul class="navigation">
    <li>home</li>
    <li>menu</li>
    <li>o nás</li>
    <li>kontakt</li>
  </ul>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
li {
  list-style: none;
}

.navigation {
  display: flex;
  justify-content: space-around;
  position: fixed;
  left: 0;
  right: 0;
}
</style>
