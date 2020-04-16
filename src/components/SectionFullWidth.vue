<template>
  <section class="section">
    <div class="section__content">
        <slot></slot>
    </div>
  </section>
</template>

<script>

export default {
  name: 'Section'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.section {
    background-image: url('../assets/banner.jpg');
    background-size: cover;
    background-position: center center;
}

.section__content {
  padding: 40px 0;
  max-width: 1200px;
  margin: auto;
}

p {
  margin-bottom: 40px;
}

</style>
