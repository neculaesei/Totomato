<template>
  <div class="app-history">
    <div v-for="n in completedSessionsCount" class="circle"></div>
    <div class="circle current"></div>
  </div>
</template>

<script>
export default {
  name: 'app-history',
  props: [
    'completedSessionsCount'
  ],
  data: function () {
    return {}
  },
  methods: {}
}
</script>

<style scoped>
  .app-history {
    position: fixed;
    bottom: 40px;
    width: 100%;
  }
  .circle {
    width: 16px;
    height: 16px;
    background: #fc5455;
    display: inline-block;
    margin-right: 10px;
    border-radius: 20px;
  }
  .circle.current {
    background: #ccc;
  }
</style>