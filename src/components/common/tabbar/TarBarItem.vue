<template>
  <div class="tabbar-item" @click="changePath()" :style="activedStyle">
      <div v-if="isActiced">
        <slot name="activeImg"></slot>
      </div>
      <div v-else>
        <slot name="img"></slot>
      </div>
      <div>
        <slot name="text"></slot>
      </div>
  </div>
</template>

<script>
export default {
  props:{
    path:String,
    activedColor: {
      type: String,
      default: '#ff5777'
    }
  },
  data() {
    return {
    }
  },
  methods: {
    changePath(){
      this.$router.push(this.path)
    }
  },
  computed: {
    isActiced(){
      return this.path === this.$route.path
    },
    activedStyle(){
      return this.isActiced? {color: this.activedColor} : {}
    }
  },
}
</script>

<style>
  .tabbar-item {
    flex: 1;
  }
  .tabbar-item img {
    height: 24px;
    width: 24px;
    vertical-align: middle;
    margin: 3px 0;
  }
  .active{
    color: var(--color-tint);
  }
</style>