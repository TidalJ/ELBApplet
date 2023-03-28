<template>
	<!-- 		<div class="box">
		<h1><span class="row" user-select selectable>Chao Jia</span>ng</h1>
		<text user-select selectable space="ensp" decode>sada &gt; sd a</text>
	</div> -->

	<!-- 	<view class="">
		<navigator url="../home/home" open-type="reLaunch">tiaozhuan</navigator>
	</view> -->

	<!-- 	<scroll-view class="scroll1" scroll-y="true" scroll-x>
		<view class="scrollgroup">
			<view class="item">123</view>
			<view class="item">123</view>
			<view class="item">123</view>
			<view class="item">123</view>
		</view>
	</scroll-view> -->
	<view class="">
		<view class="content1">
			<!-- <h1>About Us</h1> -->
			<image src="../../static/eastern.png" mode="heightFix"></image>

			<p class="content2">
				公司简介
			</p>

			<uni-section>
				<uni-link href="http://easternlightbuilding.com/" text="Browse the official website" color="#0958a9"
					showUnderLine="false" fontSize="20">官网</uni-link>
			</uni-section>

		</view>

		<view class="mainview">
			<button class="box" @click="callus">Call Us</button>
			<!-- <button class="box">Email Us</button> -->

		</view>
	</view>
</template>

<script>
	export default {
		methods: {
			callus() {
				wx.makePhoneCall({
					phoneNumber: '0405608808'
				})
			},

		}
	}
</script>

<style lang="scss">
	.content1 {
		text-align: center;
	}

	.mainview {
		width: 500rpx;
		text-align: center;
		display: flex;
		margin: 50rpx auto;
	}

	button {
		color: #ffffff;
		padding: 0.7em 1.7em;
		font-size: 30rpx;
		border-radius: 15rpx;
		background: rgb(4, 107, 182);
		background: -moz-linear-gradient(90deg, rgba(4, 107, 182, 1) 0%, rgba(9, 88, 169, 1) 50%, rgba(23, 44, 137, 1) 100%);
		background: -webkit-linear-gradient(90deg, rgba(4, 107, 182, 1) 0%, rgba(9, 88, 169, 1) 50%, rgba(23, 44, 137, 1) 100%);
		background: linear-gradient(90deg, rgba(4, 107, 182, 1) 0%, rgba(9, 88, 169, 1) 50%, rgba(23, 44, 137, 1) 100%);
		filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#046bb6", endColorstr="#172c89", GradientType=1);
		transition: all .3s;
		box-shadow: 2rpx 4rpx 6rpx #c5c5c5,
			-2rpx -4rpx 6rpx #ffffff;

	}

	button:active {
		color: #666;
		box-shadow: inset 5rpx 5rpx 12rpx #c5c5c5,
			inset -5rpx -5rpx 12rpx #ffffff;
	}

	.content2 {
		margin-bottom: 20rpx;
		// font-style: italic;
		font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
		font-size: 18px;
	}
</style>
