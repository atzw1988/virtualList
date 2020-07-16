<template>
  <div class="list" @scroll="handleScroll">
    <div class="item" v-for="(item, index) in list" :key="index">
      <div class="content">第{{index + 1}}条{{item}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    click (e) {
      console.log(e)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
