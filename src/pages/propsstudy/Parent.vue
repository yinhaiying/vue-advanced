<template>
  <div class="container">
    <Child @onClick = 'handleClick' :age = age :type = type>
      <div>这是通过slot插入的一段话</div>
    </Child>
  </div>
</template>

<script>
import Child from './Child.vue'
export default {
  name:'Parent',
  data() {
    return {
      name:'hello',
      age:24,
      type:'success'
    }
  },
  components: {
    Child
  },
  methods:{
    handleClick(value){
      alert(value)
    }
  }
}
</script>

<style scoped lang="scss">

</style>
