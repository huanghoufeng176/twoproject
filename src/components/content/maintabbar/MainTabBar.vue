<template>
  <div class="main-tab-bar">
    <tab-bar>
      <tab-bar-item path="/home">
        <img class="image" slot="tab-bar-icon" src="~assets/img/tabbar/home.svg" alt="">
        <img class="image" slot="tab-bar-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
        <div slot="tab-bar-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img class="image" slot="tab-bar-icon" src="~assets/img/tabbar/home.svg" alt="">
        <img class="image" slot="tab-bar-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
        <div slot="tab-bar-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img class="image" slot="tab-bar-icon" src="~assets/img/tabbar/home.svg" alt="">
        <!-- <img class="image" slot="tab-bar-icon-active" src="assets/img/tabbar/home_active.svg" alt=""> -->
        <img class="image" slot="tab-bar-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">

        <div slot="tab-bar-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/shopcart">
        <img class="image" slot="tab-bar-icon" src="~assets/img/tabbar/home.svg" alt="">
        <img class="image" slot="tab-bar-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
        <div slot="tab-bar-text">首页</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from 'components/common/tabbar/TabBar.vue'
import TabBarItem from 'components/common/tabbar/TabBarItem.vue'
export default {
  components:{
    TabBar,
    TabBarItem
  },
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
  .image{
    width: 24px;
    height: 24px;
  }
</style>