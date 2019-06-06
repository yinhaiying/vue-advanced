<template>
  <div class="container">
    姓名：{{name}}
    年龄：{{age}}
    <button @click ="$emit('onClick','自定义事件')" :class = "type">点击</button>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name:'Child',
  props:{
    name:{
      type:String,
      require:true
    },
    age:{
      type:Number
    },
    type:{
      validator:function(value){
        return (['success','warning','primary'].indexOf(value)) > -1
      }
    }
  },
  data() {
    return {
      
    }
  },
  methods:{
    HanldeClick(){
      
    }
  }
}
</script>

<style scoped lang="scss">

</style>
