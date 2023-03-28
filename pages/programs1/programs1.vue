<template>
	<view class="container1">
		<h1 class="name">项目名</h1>
		<image class="img1" :src="'../../static/home4.jpg'" mode=""></image>
		<p class="content">项目文案</p>
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

<style lang="scss">
	.container1 {
		justify-content: center;
		display: flex;
		align-items: center;
		border-radius: 15rpx;
		flex-direction: column;
	}

	.img1 {
		margin-top: 75rpx;
		border-radius: 15rpx;
		width: 560rpx;
		height: 400rpx;
	}

	.name {
		margin-top: 75rpx;
		display: block;
		font-size: 50rpx;
		font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
		background: -webkit-linear-gradient(90deg, rgba(4, 107, 182, 1) 0%, rgba(9, 88, 169, 1) 50%, rgba(23, 44, 137, 1) 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}

	.content {
		display: block;
		margin-top: 50rpx;
		font-size: 40rpx;
		font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
	}
</style>
