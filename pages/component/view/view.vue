<template>
	<view>
		<page-head title="view"></page-head>
		
	</view>
</template>
<script>
	export default {
		data() {
			return {
				show: false,
				mode: 'date'
			}
		},
		onLoad() {
			this.$api.classifyLeft({type:1}).then((res) => {
				console.log('123',res);
			})
		}
	}
</script>

<style>
	.flex-item {
		width: 33.3%;
		height: 200rpx;
		text-align: center;
		line-height: 200rpx;
	}

	.flex-item-V {
		width: 100%;
		height: 150rpx;
		text-align: center;
		line-height: 150rpx;
	}

	.text {
		margin: 15rpx 10rpx;
		padding: 0 20rpx;
		background-color: #ebebeb;
		height: 70rpx;
		line-height: 70rpx;
		text-align: center;
		color: #777;
		font-size: 26rpx;
	}

	.desc {
		/* text-indent: 40rpx; */
	}

	.flex-pc {
		display: flex;
		justify-content: center;
	}
</style>
