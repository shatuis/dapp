<template>
  <div id="app">
    <template>
    <section>
        <b-field>
            <b-checkbox>Basic</b-checkbox>
        </b-field>
        <b-field>
            <b-checkbox v-model="checkbox">
                {{ checkbox }}
            </b-checkbox>
        </b-field>
        <b-field>
            <b-checkbox v-model="checkboxCustom"
                true-value="Yes"
                false-value="No">
                {{ checkboxCustom }}
            </b-checkbox>
        </b-field>
        <b-field>
            <b-checkbox :indeterminate="true">
                Indeterminate
            </b-checkbox>
        </b-field>
        <b-field>
            <b-checkbox disabled>Disabled</b-checkbox>
        </b-field>
    </section>
</template>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>
<script>
    export default {
        data() {
            return {
                checkbox: false,
                checkboxCustom: 'Yes'
            }
        }
    }
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
