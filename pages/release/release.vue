<template>
		<view class="release">
			<view :style="{height:gtHeight}"></view>
			<uni-nav-bar  fixed left-icon="back" color="#999" title="发布论坛">
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
		onLoad(){
			
		}
	}
</script>

<style lang="scss">
</style>
