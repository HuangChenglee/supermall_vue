<template>
  <tab-bar>
      <tab-bar-item path="/home">
        <img src="~assets/img/tabbar/home.svg" alt="home" slot="img">
        <img src="~assets/img/tabbar/home_active.svg" alt="active_home" slot="activeImg">
        <div slot="text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img src="~assets/img/tabbar/category.svg" alt="category" slot="img">
        <img src="~assets/img/tabbar/category_active.svg" alt="active_category" slot="activeImg">
        <div slot="text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/shopcart">
        <img src="~assets/img/tabbar/shopcart.svg" alt="shopcart" slot="img">
        <img src="~assets/img/tabbar/shopcart_active.svg" alt="active_shopcart" slot="activeImg">
        <div slot="text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img src="~assets/img/tabbar/profile.svg" alt="profile" slot="img">
        <img src="~assets/img/tabbar/profile_active.svg" alt="active_profile" slot="activeImg">
        <div slot="text">我的</div>
      </tab-bar-item>
    </tab-bar>
</template>

<script>
import TabBar from 'components/common/tabbar/TabBar'
import TabBarItem from 'components/common/tabbar/TarBarItem'

export default {
  components:{
    TabBar,
    TabBarItem
  }
}
</script>

<style>
</style>