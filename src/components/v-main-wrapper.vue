<template>
    <div class="v-main-wrapper">
        <p>{{title}}</p>
        <v-catalog/>
        <v-cart/>
    </div>
</template>

<script>
import VCart from './v-cart'
import VCatalog from './v-catalog'

   export default {
      name: 'v-main-wrapper',
      components: {
            VCart,
            VCatalog
      },
      props: {},
      data() {
          return {
              title: 'Main wrapper'
          }
      },
      computed: {},
      methods: {},
      watch:{},
      mounted() {
          console.log('Hello i am alive!')
        }
    }
</script>

<style>
.v-main-wrapper {
    max-width: 300px;
    margin: 0 auto;
}
</style>


