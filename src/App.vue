<template>
  <div id="app">
    <vue-header></vue-header>
    <br><br>
    <time-line></time-line>
  </div>
</template>

<script>
import VueHeader from './components/Header'
import TimeLine from './components/TimeLine'
export default {
  components: {
    VueHeader,
    TimeLine
  }
}
</script>
