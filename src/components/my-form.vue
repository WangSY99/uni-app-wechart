<template>
  <view class="form">
    <view class="form_title">标题</view>
    <view class="form_content">内容</view>
    <slot></slot>
  </view>
</template>

<script>
export default {
  //onLoad在组件中使用没有效果
//  onLoad(){
//    console.log("myform onload");
//  },
 mounted(){
   console.log("myform onload 组件挂载完毕");
 }
}
</script>

<style>

</style>
