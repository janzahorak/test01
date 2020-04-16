<template>
  <section
    class="section"
    :class="{
      'section--reverse' : layoutReverse
      }"
  >
    <h2
      v-if="title"
    >
      {{ title }}
    </h2>
    <p
      v-if="perex"
    >
      {{ perex }}
    </p>

    <slot></slot>

  </section>
</template>

<script>

export default {
  name: 'Section',
  props: {
    title: {
      type: String
    },
    perex: {
      type: String
    },
    layoutReverse: {
      type: Boolean
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.section {
  padding: 40px 0;
  max-width: 1200px;
  margin: auto;
}

.section--reverse .grid1 {
  flex-direction: row-reverse;
}

p {
  margin-bottom: 40px;
}

</style>
