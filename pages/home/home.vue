<template>
	<view class="container1">

		<!-- 		<form action="" @submit="onsubmit">
			<view class="row">
				<input type="text" name="username" id="" v-model="message.username">
			</view>

			<view class="row">
				<textarea name="content" id="" cols="30" rows="10" v-model="message.content"></textarea>
			</view>

			<radio-group name="gender">
				<label>
					<radio value="男" /><text>nan</text>
				</label>
				<label>
					<radio value="女" /><text>nv</text>
				</label>
			</radio-group>

			<view class="box">
				<button form-type="reset">reset</button>
				<button form-type="submit" type="primary">submit</button>
			</view>
			{{message.username}}
		</form> -->

		<view class="title">
			<!-- <img src="https://git.weixin.qq.com/jc395478/ELBApplets/blob/master/static/home1.jpg" alt="" srcset=""> -->
			<image class="img1" src="../../static/eastern.png" mode="heightFix"></image>
			<h1 class="programname">主营类别</h1>

		</view>

		<view class="img">
			<view class="" hover-class="imghover">
				<image class="first" :src="'../../static/home1.jpg'" mode="" @click="toprogram1"></image>
			</view>

			<view class="" hover-class="imghover">
				<image :src="'../../static/home2.jpg'" mode="" @click="toprogram2"></image>
			</view>

			<view class="" hover-class="imghover">
				<image :src="'../../static/home3.jpg'" mode="" @click="toprogram3"></image>
			</view>

			<view class="" hover-class="imghover">
				<image :src="'../../static/home4.jpg'" mode="" @click="toprogram4"></image>
			</view>

		</view>

		<view class="foot">
			<image class="footimg2" src="../../static/eastern.png" mode="heightFix"></image>
			<image class="footimg1" src="../../static/member.png" mode="heightFix"></image>
		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				content: [1, 2, 3, 4],
				title: "abc",
				message: {
					username: "",
					tel: "",
					content: ""
				}
			}
		},
		methods: {
			toprogram() {
				uni.navigateTo({
					url: "/pages/programs1/programs1",
				})
			},
			toprogram1() {
				uni.navigateTo({
					url: "/pages/programs1/programs1"
				})
			},
			toprogram2() {
				uni.navigateTo({
					url: "/pages/programs2/programs2"
				})
			},
			toprogram3() {
				uni.navigateTo({
					url: "/pages/programs3/programs3"
				})
			},
			toprogram4() {
				uni.navigateTo({
					url: "/pages/programs4/programs4"
				})
			},
			onsubmit(e) {
				console.log(e);
			}
		}
	}
</script>

<style lang="scss">
	.container1 {
		display: flex;
		flex-direction: column;
	}

	image {
		border-radius: 15rpx;
		margin-top: 50rpx;
		width: 560rpx;
		height: 400rpx;
	}

	input,
	textarea {
		border: 1px solid black;
	}

	.first {
		margin-top: 300rpx;
	}

	.img {
		display: flex;
		justify-content: center;
		flex-direction: column;
		margin: 0 auto;
		flex-wrap: wrap;
		transition: 0.3s;
	}

	.title {
		position: absolute;
	}

	.img1 {
		position: absolute;
		top: 30rpx;
		height: 150rpx;
	}

	.programname {
		display: flex;
		position: absolute;
		width: 350rpx;
		height: 100rpx;
		top: 100rpx;
		left: 225rpx;
	}

	.pro {
		align-items: center;
		justify-content: center;
		margin-left: 30rpx;
		display: inline-block;
		position: absolute;
		margin-top: 125rpx;
		line-height: 100%;
	}

	h1 {
		font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
		font-size: 70rpx;
		// font-style: italic;
		background: -webkit-linear-gradient(90deg, rgba(4, 107, 182, 1) 0%, rgba(9, 88, 169, 1) 50%, rgba(23, 44, 137, 1) 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}

	.foot {
		margin-top: 100rpx;
		padding: 0rpx;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.footimg1 {
		height: 125rpx;
		margin: 0 auto;
	}

	.footimg2 {
		height: 150rpx;
		margin: 0 auto;
	}
</style>
