<template>
	<view class="index">
		<view class="tn-flex">
			<tn-avatar text="图鸟"></tn-avatar>
			<view>
				<text>{{name}}</text>
				<view>
					<text>积分：{{count}}</text>
					<tn-button @click="jumpCredits">获取积分</tn-button>
				</view>
			</view>
		</view>
		
		<view class="btn-view-ans">
			给我答案
		</view>
		
		<view>
			<view class="btn-view-ans">
				答案库
			</view>
			<view class="btn-view-ans">
				使用教程
			</view>
		</view>
		
		
		<text>加入微信群</text>
	</view>
</template>

<script>
	export default {
		components: {

		},
		data() {
			return {
				name: "andy",
				count: 50
			}
		},
		onLoad(options) {

		},
		onPageScroll(e) {},
		onReachBottom() {},
		methods: {
			jumpCredits() {
				
			}
		}
	}
</script>

<style lang="scss" scoped>
	.index {
		overflow: hidden;
		height: 100%;
	}

	.custom-tabbar-page {
		height: calc(100vh - (100rpx + env(safe-area-inset-bottom) / 2));
	}
</style>
