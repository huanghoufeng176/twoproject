<template>
  <div class="tab-bar-item" @click="itemClick">
    <div v-if="!isActive"><slot name="tab-bar-icon"></slot></div>
    <div v-else><slot name="tab-bar-icon-active"></slot></div>
    <div :style="styleColor"><slot name="tab-bar-text"></slot></div>
  </div>
</template>

<script>
export default {
  props:{
    path:String,
    color:{
      type:String,
      default:'red'
    }
  },
  components:{},
  data(){
    return {
    }
  },
  created(){},
  mounted(){},
  watch:{},
  computed:{
    isActive(){
      return this.$route.path.indexOf(this.path)!==-1
    },
    styleColor(){
      return this.isActive?{color:this.color}:{}
    }
  },
  methods:{
    itemClick(){
      this.$router.push(this.path)
    }
  },
}
</script>
<style scoped>
  .tab-bar-item{
    flex: 1;
    text-align: center;
  }
</style>