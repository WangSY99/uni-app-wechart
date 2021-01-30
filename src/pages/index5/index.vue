<template>
  <view class="content">
    <!-- <imgBorder></imgBorder> -->
    <view> 子组件传递过来的路径：{{ src }} </view>
    <img-border @srcChange="handleSrcChange" :src="src1"></img-border>
    <img-border @srcChange="handleSrcChange" :src="src2"></img-border>
  </view>
</template>

<script>
//2 引入自定义组件
import imgBorder from "@/components/img-border";
export default {
  data() {
    return {
      src: "",
      src1:
        "https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201711%2F29%2F20171129145153_n8syc.jpeg&refer=http%3A%2F%2Fb-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1614234154&t=885bd5d16db5edc8d206dfa1e06655aa",
      src2:
        "https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201605%2F04%2F20160504175630_FcGsw.jpeg&refer=http%3A%2F%2Fb-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1614234154&t=3b59ed02af909b5de970fd87765a3a2f",
    };
  },
  //3注册组件
  components: {
    imgBorder: imgBorder,
  },
  methods: {
    handleSrcChange(e) {
      //  console.log("父组件的自定义事件被触发了");
      // console.log(e);
      this.src = e;
    },
  },
  //onLoad 页面加载完毕就会触发的生命周期
  onLoad() {
    console.log(this.baseurl);
    // 获取globaldata

    console.log(getApp().globalData.base);
  },
};
</script>
    
<style lang="scss"></style>
