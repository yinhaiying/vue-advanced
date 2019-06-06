<template>
  <div class="container">
    <Child :name = name :age = age></Child>
  </div>
</template>

<script>
import Child from './Child.vue'
export default {
  name:'Parent',
  data() {
    return {
      name:'刘亦菲',
      age:24
    }
  },
  components: {
    Child
  }
}
</script>

<style scoped lang="scss">

</style>
