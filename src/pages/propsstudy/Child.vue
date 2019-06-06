<template>
  <div class="container">
    姓名：{{name}}
    年龄：{{age}}
  </div>
</template>

<script>
export default {
  name:'Child',
  props:['name','age'],
  data() {
    return {
      
    }
  },
  components: {

  }
}
</script>

<style scoped lang="scss">

</style>
