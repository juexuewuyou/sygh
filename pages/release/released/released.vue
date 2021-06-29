<template>
		<view class="release">
			<view :style="{height:gtHeight}"></view>
			<uni-nav-bar @click="back"  fixed left-icon="back" color="#999" title="发布论坛">
				<view slot="right" class="fb">
					<text class="fon-medium fon-8">发布</text>
				</view>
			</uni-nav-bar>
		</view>
</template>

<script>
	export default {
		data() {
			return {
				gtHeight:''
			}
		},
		methods: {
			//获取状态栏高度
			getHeight(){
				this.gtHeight=(uni.getSystemInfoSync().statusBarHeight)*2+'rpx'
			},
			back(){
				uni.redirectTo({url: '/pages/index/index'})
			}
		},
		onLoad(){
			this.getHeight()
		},
	}
</script>

<style lang="scss">
 // @import  "../../../static/css/released.scss"
</style>
