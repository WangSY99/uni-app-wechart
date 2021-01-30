<script>
	export default {
		//应用启动的时候就会触发
		onLaunch: function() {
			console.log('App Launch 应用启动')
		},
		//应用被看到了
		onShow: function() {
			console.log('App Show')
		},
		//应用被隐藏了
		onHide: function() {
			console.log('App Hide')
		},
		globalData:{
			base:"www.360.com"
		},
	}
</script>

<style>
	/*每个页面公共css */
</style>
