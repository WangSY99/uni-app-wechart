<template>
  <view class="content">
    <!-- 1 给view标签绑定点击事件 -->
    <view data-index="11" @click="handleClick('不想努力了！', $event)"
      >点击我试试1</view
    >
    <view data-index="haha" @click="handleClick(2, $event)">点击我试试2</view>
  </view>
</template>

<script>
export default {
  // 2在methods里面来定义事件的回调
  methods: {
    handleClick(a, event) {
      console.log(a);
      console.log(event);
      console.log(event.currentTarget.dataset.index);
      console.log(a, event.currentTarget.dataset.index);
    },
  },
};
</script>
    
<style lang="scss"></style>
