<template>
    <section>
        <b-button @click="clickMe">Click Me</b-button>
    </section>
</template>


<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

