<template>
  <div class="nav-bar-item">
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
export default {
  components:{},
  data(){
    return {
    }
  },
  created(){},
  mounted(){},
  watch:{},
  computed:{},
  methods:{},
}
</script>
<style scoped>
  .nav-bar-item{
    height: 39px;
    background-color: pink;
    display: flex;
  }
  .left, .right{
    width: 60px;
    height: 39px;
    /* background-color: green; */
  }
  .center{
    flex: 1;
    text-align: center;
    line-height: 39px;
    color: white;
  }
</style>