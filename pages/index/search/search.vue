<template>
	<view class="search">
		<!-- 搜索栏 -->
		<view class="tosearch">
			<uni-easyinput  
			:inputBorder="false" 
			prefixIcon="search" 
			v-model="value" 
			placeholder="搜索课程 / 帖子 / 老师"
			placeholderStyle="color:#999999" 
			:clearable="false">
				</uni-easyinput>
			<view style="color:#999;font-size: 0.75rem;" @click="">
				<navigator animation-type="pop-out" animation-duration="300" open-type="navigateBack" style="width:60rpx;height:46rpx;margin:8rpx 26rpx 0 38rpx">取消</navigator>
			</view>
		</view>
		<!-- 搜索栏结束 -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value:''
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss">
  .search{
	  padding: 0 30rpx;
	  .tosearch {
		padding:20rpx 0;
	  	display: flex;
	  	justify-content: space-between;
	  	align-items: center;
	  };
  }
</style>
