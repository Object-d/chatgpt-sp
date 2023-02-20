<template>
	<view class="container">
		<tn-button @click="jumpAsk">提问</tn-button>
		
		<view>
			
		</view>
	</view>
</template>

<script>
	import chatMixin from '../../../mixins/chat.js'
	export default {
		mixins: [chatMixin],
		
		methods: {
			jumpAsk() {
				uni.navigateTo({
					url: '/pages/ask/index'
				})
			}
		}
	}
</script>

<style lang="scss" scoped>
	
</style>
