<template>
  <view class="content">
    <!-- 2 使用数据{{msg}} -->
    <view>{{ msg }}</view>
    <view>{{ money }}</view>
    <view>{{ isRich }}</view>
    <view>{{ person.name }}</view>
    <view>{{ person.skill }}</view>
    <!-- 在标签上通过属性的方式来使用数据 -->
    <view :data-color="color">color</view>
    <view>========================</view>
    <view>
      <!-- list 通过view标签来显示 -->
      <view
      v-for="(item) in list"
      :key="item.id"
      >
      {{item.id}} -- {{item.text}}
      </view>
    </view>
  </view>
</template>

<script>
export default {
  // 1 data 定义数据
  data() {
    return {
      //存放数据
      msg: "黑马程序员-广州中心",
      //数字
      money: 10000,
      //bool类型
      isRich: false,
      //对象
      person: {
        name: "孙悟空",
        skill: "72变",
      },
      // 颜色
      color:"aqua",
      //数组
      list:[
        {
          id:0,
          text:"苹果"
        },
        {
          id:1,
          text:"香蕉"
        },
        {
          id:2,
          text:"樱桃"
        }
      ]
    };
  },
};
</script>
    
<style lang="scss"></style>
