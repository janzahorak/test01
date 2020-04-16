<template>
  <div class="hero">
    <div class="hero__content">
      <h1>Chile <span class="red">y</span> limón</h1>
      <p>Tradiční mexická kuchyně Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hero {
  background-image: url('../assets/hero.jpg');
  background-size: cover;
  background-position: center center;
  height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.red {
  color: #ca1f1f;
}

h1 {
  font-size: 72px;
  color: white;
  margin: 0;
}

p {
  color: whitesmoke;
}

</style>
