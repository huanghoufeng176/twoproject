<template>
  <div class="tab-bar">
    <slot></slot>
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
  .tab-bar{
    height: 49px;
    background-color: #f6f6f6;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    display: flex;
    box-shadow: 0 -1px 1px rgba(100,100,100,0.1);
  }
</style>