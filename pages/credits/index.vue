<template>
	<view class="container">
		<view class="top">
			<!-- <u-image width="100%" height="350rpx" :src="topSrc"></u-image> -->
			<view class="sign-info">
				<!-- <u-avatar :src="headSrc" size="large" class="headSrc"></u-avatar> -->
				<view class="break">
					|
				</view>
				<view class="sign-duration">
					<label style="font-size: 30rpx;">丽尔维美网络部</label>
					<view style="font-size: 25rpx;margin-top:15rpx;">
						<label style="margin-left:10rpx;">坚持2天</label> <label style="margin-left:10rpx;">4小时前签到</label>
					</view>
				</view>
			</view>
		</view>
		<view class="tongji">
			<view class="sign-count">
				<view class="sign-count-top">
					<view>
						<!-- <u-icon name="calendar" color="#fd4835" size="40rpx"></u-icon> -->
						<label style="margin-left:10rpx;font-size: 35rpx;">签到统计</label>
					</view>
					<view style="margin-left:251rpx;font-size: 28rpx;">
						查看签到记录 >>
					</view>
				</view>
				<view style="margin-top:10rpx;">
					<<!-- u-table font-size="40" color="#9D9D9D" align="center">
						<u-tr>
							<u-td>一</u-td>
							<u-td>二</u-td>
							<u-td>三</u-td>
							<u-td>四</u-td>
							<u-td>五</u-td>
							<u-td>六</u-td>
							<u-td>日</u-td>
						</u-tr>
						<u-tr>
							<u-td><label><u-icon name="checkmark-circle" color="#9D9D9D" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle" color="#9D9D9D" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle" color="#9D9D9D" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle" color="#9D9D9D" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle-fill" color="#FD4835" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle-fill" color="#FD4835" size="50"></u-icon></label></u-td>
							<u-td><label><u-icon name="checkmark-circle" color="#9D9D9D" size="50"></u-icon></label></u-td>
						</u-tr>	
					</u-table -->>
				</view>
				
			</view>
		</view>
		
		<view class="tongji">
			<view class="sign-content">
				<text decode="true" selectable="true">{{content}}</text>		
			</view>
		</view>
	</view>


</template>



<script>
	export default {
		data() {
			return {
				topSrc: 'http://lewm.xyz/attachment/images/2/2020/08/pq6xCu96ScX6383z6p67896Qb578I6.jpg',
				headSrc: 'https://thirdwx.qlogo.cn/mmopen/vi_32/PiajxSqBRaEIHSp1OkUh7IIcWKicbP1xcvnGMaCQKMnVsUf6nemBcASAUEE40RApbwHCmz8rXntoTcIWmV9mfBVw/132',
				content:'朝着一个目标不停的向前，不断努力的付出，哪怕你现在的人生是从零开始，你都可以做得到。早安！让梦想照进现实，才是当下最应该做的事情！',
				musicSrc:'http://lewm.xyz/mp4/qifengle.mp3',
				avatarSrc:'https://thirdwx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTIrNE2NFhpubQaPX6qD0urZHn9iaIicr3aA9PdTrbJMWiaTTqsug3eSkRsiaXswC4Vic4ibqags3OX21IMA/132'
			}
		},
		methods: {

		},
		 components: {
		 }
	}
</script>
<style lang="scss">
	.container {
		display: flex;
		flex-direction: column;
		// background-color: $u-bg-color;

		.top {
			width: 100%;
			height: 350rpx;

			.sign-info {
				width: 100%;
				height: 160rpx;
				border-radius: 50rpx;
				background:rgba(255,255,255,0.6);
				position: absolute;
				display: flex;
				flex-direction: row;
				top: 200rpx;

				.headSrc {
					margin-top:10rpx;
					margin-left: 40rpx;
				}

				.break {
					color: #4e4e4e;
					font-size: 90rpx;
					margin-left: 15rpx;
				}

				.sign-duration {
					margin-left: 15rpx;
					// background-color: $u-type-success;
					width: 100%;
					height: 100rpx;
					margin-top: 20rpx;
					display: flex;
					flex-direction: column;
					color: #4e4e4e;
				}
			}
		}

		.tongji {
			margin: 20rpx 20rpx;
			width: 95%;
			height: 250rpx;
			background-color: #FFFFFF;
			
			.sign-count {
				// background:#FFF;
				// background-color: $u-type-success;
				width: 92%;
				height: 200rpx;
				margin: 20rpx 30rpx;

				.sign-count-top {
					display: flex;
					flex-direction: row;

				}
			}
			.sign-content {
				// background:#FFF;
				// background-color: $u-type-success;
				width: 92%;
				margin: 20rpx 30rpx;
				font-size: 30rpx;
			}
		}
		
		.kongbai{
			height: 160rpx;
			color:#999999;
			text-align: center;
		}
		.bottom{
			width: 100%;
			height: 100rpx;
			background-color: #FFFFFF;	
			position: fixed;
			bottom: 0;
			.bottom-icon{
				width: 97%;
				height:90rpx;
				display: flex;
				flex-direction: row;
				margin:10rpx 10rpx;
				.bottom-me{
					width:72%;
					height:80rpx;
					background-color:#1F8FF3;
					margin-left: 18rpx;
					border-radius: 10rpx;
					text-align: center;
					line-height: 80rpx;
					font-size: 40rpx;
					color:#FFFFFF;
					font-weight: bold;
					letter-spacing: 7rpx;
				}
				.bottom-icon-goto{
					width:30%;
					height:80rpx;
					display: flex;
					flex-direction: row;
				}
			}	
		}
	}
</style>
