<template>
  <view class="content">
    <!-- 2 使用数据{{msg}} -->
    <view>{{ msg }}</view>
    
    
  </view>
</template>

<script>
export default {
  // 1 data 定义数据
  data () {
    return {
      //存放数据
      msg: "黑马程序员-广州中心",
      //数字
      money:10000,
      //bool类型
      isRich:false,
      //对象
      person:{
        name:"孙悟空",
        skill:"72变",

      }
    };
  },
};
</script>
    
<style lang="scss"></style>
