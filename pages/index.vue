<template>
  <section class="container">
    <div>
      <logo/>
      <h1 class="title">Elmenus</h1>
      <h2 class="subtitle">Elmenus Web</h2>

    </div>
    <nuxt-link to="/polls">Polls</nuxt-link>
  </section>
</template>

<script lang='ts'>
import { Component, Vue } from 'nuxt-property-decorator';

import Logo from '@/components/Logo.vue';

@Component({
  components: {
    Logo
  }
})
export default class Index extends Vue {}
</script>

<style>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
