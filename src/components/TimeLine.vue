<template>
  <main class="mdl-layout__content">
    <div class="page-content">
      <search></search>
      <card v-for="gif in gifs" :gif="gif" :key="gif.cid"></card>
    </div>
  </main>
</template>

<script>
import Search from './Search'
import Card from './Card'
import { mapGetters } from 'vuex'

export default {
  components: {
    Search,
    Card
  },
  computed: {
    ...mapGetters(['gifs'])
  }
}
</script>

<style>
  main {
    background-color: #f6f6f6;
    width: 100%;
    margin: 0 auto;
  }
  .page-content {
    display: flex;
    flex-direction: column;
  }
</style>
