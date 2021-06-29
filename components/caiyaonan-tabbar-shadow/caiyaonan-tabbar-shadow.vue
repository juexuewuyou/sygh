<template>
	<view>
		<view class="box-shadow">
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style>
	.box-shadow{
		position: fixed;
		bottom: 0;
		/* #ifdef APP-PLUS */
		height: 1px;
		/* #endif */
		/* #ifdef H5 */
		height: 60px;
		/* #endif */
		width: 100%;
		box-shadow: 0px 0px 5px #b5b5b5 ;
	}
</style>
