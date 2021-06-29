<template>
	<view class="index">
		<!-- 搜索栏 -->
		<view class="tosearch">
			<uni-easyinput @focus="tosearch" :inputBorder="false" prefixIcon="search" v-model="value"
				placeholder="搜索您想查找的内容" placeholderStyle="color:#999999;font:500 14rpx PingFang-SC-Medium" :clearable="false" class="inputbgc">
				
			</uni-easyinput>
			<view>
				<image model="widthFix" style="width:42rpx;height:46rpx;margin:8rpx 38rpx 0 38rpx" src="../../static/image/icon/icon_news.png"
					mode="scaleToFill"></image>
			</view>
		</view>
		<!-- 搜索栏结束 -->

		<!-- 轮播图 -->
		<view class="banner">
			<view class="uni-padding-wrap" >
				<view class="page-section swiper" >
					<view class="page-section-spacing">
						<swiper class="swiper" 
						:indicator-dots="indicatorDots" 
						:autoplay="autoplay"
						:interval="interval" 
						:duration="duration" 
						circular="true" 
						indicator-active-color="#FFF"
						indicator-color="#FFD0C2"
						
						>
							<swiper-item>
								<view class="swiper-item" style="width: 690rpx;height:300rpx;">
									<image style="width: 690rpx;height:300rpx;" src="../../static/image/carousel/carousel_1.png"
										mode="widthFix"></image>
								</view>
							</swiper-item>
							<swiper-item>
								<view class="swiper-item" style="width: 690rpx;height:300rpx;overflow: hidden;">
									<image style="width: 690rpx;height:300rpx" src="../../static/image/carousel/carousel_1.png"
										mode="widthFix"></image>
								</view>
							</swiper-item>
							<swiper-item>
								<view class="swiper-item overhidden" style="width: 690rpx;height:300rpx;overflow: hidden;">
									<image style="width: 690rpx;height:300rpx" src="../../static/image/carousel/carousel_1.png"
										mode="widthFix"></image>
								</view>
							</swiper-item>
						</swiper>
					</view>
				</view>
			</view>
		</view>
		<!-- 轮播图结束 -->
		<!-- 模块导航 -->
		<view class="models">
			<view>
				<view>
					<image src="../../static/image/models/model_kj.png" mode="widthFix"></image>
				</view>
				<text>会计</text>
			</view>
			<view>
				<view>
					<image src="../../static/image/models/model_gwy.png" mode="widthFix"></image>
				</view>
				<text>公务员</text>
			</view>
			<view>
				<view>
					<image src="../../static/image/models/model_jszg.png" mode="widthFix"></image>
				</view>
				<text>教师资格</text>
			</view>
			<view>
				<view>
					<image src="../../static/image/models/model_jsj.png" mode=""></image>
				</view>
				<text>计算机</text>
			</view>
			<view>
				<view>
					<image src="../../static/image/models/model_all.png" mode=""></image>
				</view>
				<text>全部</text>
			</view>
		</view>
		<!-- 模块导航结束 -->
		<!-- 课程分类-->
		<view class="titlesbox">
			<text style="font:500 1rem 'PingFang-SC-Medium';color:#333">课程分类</text>
			<view class="titleitem" style="flex: 1;">
				<view class="tleft">
					<view>
						<image style="width:322rpx;height:412rpx" src="../../static/image/modelbox/box_mf.png" mode="widthFix"></image>
					</view>
				</view>
				<view class="tright">
					<view class="ritem">
						<image style="width: 344rpx;height:196rpx;" src="../../static/image/modelbox/box_st.png" mode="heightFix"></image>
					</view>
					<view class="ritem">
						<image style="width: 344rpx;height:196rpx;" src="../../static/image/modelbox/box_gh.png" mode="heightFix"></image>
					</view>
				</view>
			</view>
		</view>
		<!-- 课程分类结束 -->
		<!-- 信息资讯 -->
		<view class="ifcf">
			<view class="ititle">
				<text style="font:500 1rem 'PingFang-SC-Medium';color:#333">信息资讯</text>
				   <view style=" display: flex;justify-content: space-between;align-items: center;">
					   <text style="color:#999;font:500 1rpx 'PingFang-SC-Medium';margin-right:8rpx">查看全部
					   </text>
					  <view class="ricon"></view>
				   </view>
			</view>	
			<!-- 内容填充 -->
			<view class="icontainer">
				<view class="ileft">
					<view style="width:212rpx;height:180rpx">
						<image style="width:212rpx;height:180rpx" src="../../static/image/ititles/ilist.png" mode="scaleToFill"></image>
					</view>
				</view>
				<view class="iright">
					<view class="iitem">
						<text style="font:bold 1rem'PingFang-SC-Bold';color:#333;padding:14rpx">全国计算机一级考试 考试指导题目参考</text>
						<text style="font:500 0.5rem 'PingFang-SC-Medium';color:#999">10:54</text>
					</view>
					<view class="iitem ">
						<view  class="rightbottom">
							<view style="margin-left:14rpx;width:48rpx;height:48rpx">
								<image style="width:48rpx;height:48rpx" src="../../static/image/ititles/icon_avatar.png" mode="scaleToFill	"></image>
							</view>
							<text>会计指导</text>
						</view>
						<!-- 下 -->
						<view class="righthand">
							<view class="rightbottom">
								<view style="width:30rpx;height:28rpx">
									<image style="width:30rpx;height:28rpx" src="../../static/image/ititles/icon_checkLove.png" mode="scaleToFill"></image>
								</view>
								<text>2003</text>
							</view>
							<view class="rightbottom" style="margin-left:20rpx">
								<view>
									<image style="width:33rpx;height:22rpx" src="../../static/image/ititles/icon_look.png" mode="scaleToFill"></image>
								</view>
								<text>1005</text>
							</view>
						</view>
						<!-- 下 -->
					</view>
				</view>
			</view>
			<!-- 内容填充结束 -->
			<view class="icontainer">
				<view class="ileft">
					<view style="width:212rpx;height:180rpx">
						<image style="width:212rpx;height:180rpx" src="../../static/image/ititles/ilist.png" mode="scaleToFill"></image>
					</view>
				</view>
				<view class="iright">
					<view class="iitem">
						<text style="font:bold 1rem'PingFang-SC-Bold';color:#333;padding:14rpx">全国计算机一级考试 考试指导题目参考</text>
						<text style="font:500 0.5rem 'PingFang-SC-Medium';color:#999">10:54</text>
					</view>
					<view class="iitem ">
						<view  class="rightbottom">
							<view style="margin-left:14rpx;width:48rpx;height:48rpx">
								<image style="width:48rpx;height:48rpx" src="../../static/image/ititles/icon_avatar.png" mode="scaleToFill	"></image>
							</view>
							<text>会计指导</text>
						</view>
						<!-- 下 -->
						<view class="righthand">
							<view class="rightbottom">
								<view style="width:30rpx;height:28rpx">
									<image style="width:30rpx;height:28rpx" src="../../static/image/ititles/icon_checkLove.png" mode="scaleToFill"></image>
								</view>
								<text>2003</text>
							</view>
							<view class="rightbottom" style="margin-left:20rpx">
								<view>
									<image style="width:33rpx;height:22rpx" src="../../static/image/ititles/icon_look.png" mode="scaleToFill"></image>
								</view>
								<text>1005</text>
							</view>
						</view>
						<!-- 下 -->
					</view>
				</view>
			</view>
			<view class="icontainer">
				<view class="ileft">
					<view style="width:212rpx;height:180rpx">
						<image style="width:212rpx;height:180rpx" src="../../static/image/ititles/ilist.png" mode="scaleToFill"></image>
					</view>
				</view>
				<view class="iright">
					<view class="iitem">
						<text style="font:bold 1rem'PingFang-SC-Bold';color:#333;padding:14rpx">全国计算机一级考试 考试指导题目参考</text>
						<text style="font:500 0.5rem 'PingFang-SC-Medium';color:#999">10:54</text>
					</view>
					<view class="iitem ">
						<view  class="rightbottom">
							<view style="margin-left:14rpx;width:48rpx;height:48rpx">
								<image style="width:48rpx;height:48rpx" src="../../static/image/ititles/icon_avatar.png" mode="scaleToFill	"></image>
							</view>
							<text>会计指导</text>
						</view>
						<!-- 下 -->
						<view class="righthand">
							<view class="rightbottom">
								<view style="width:30rpx;height:28rpx">
									<image style="width:30rpx;height:28rpx" src="../../static/image/ititles/icon_checkLove.png" mode="scaleToFill"></image>
								</view>
								<text>2003</text>
							</view>
							<view class="rightbottom" style="margin-left:20rpx">
								<view>
									<image style="width:33rpx;height:22rpx" src="../../static/image/ititles/icon_look.png" mode="scaleToFill"></image>
								</view>
								<text>1005</text>
							</view>
						</view>
						<!-- 下 -->
					</view>
				</view>
			</view>
		</view>
		<!-- 信息资讯结束 -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value: '',
				indicatorDots: true,
				autoplay: true,
				interval: 3000,
				duration: 500,
				data:[{
					id:1,
					title:'全国计算机一级考试 考试指导题目参考',
					time:'10:54',
					userName:'会计指导',
					zaan:'2003',
					look:'1005'
					}
				]
			}
		},
		onLoad() {

		},
		methods: {
			tosearch() {
				uni.navigateTo({
					url: './search/search'
				})
			}
		}
	}
</script>

<style lang="scss">
   @import "../../static/css/index.scss"
</style>
