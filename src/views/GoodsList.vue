<template>
  <div>
      这是商品列表页面
      <router-link to="/goods/title">显示商品标题</router-link>
       <router-link to="/goods/image">显示商品图片</router-link>
        <router-link v-bind:to="{name:'cart',params:{cartId:123}}">跳转到购物车页面</router-link>
      <div>
         <router-view></router-view>
      </div>
      <button @click="jump">button-转购物车</button>
  </div>
</template>

<script>
export default {
      data () {
        return {
          msg:"hellow Vue"
        }
      },
      methods: {
        jump(){
          this.$router.push({path:'cart?goodsId=123'})
        }
      }
}
</script>

<style>

</style>