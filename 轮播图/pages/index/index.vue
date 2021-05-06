<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>

	        <bw-swiper :swiperList="bannerList"  :swiperType="true" style="width:100%"></bw-swiper>
 
	</view>
	
</template>

<script>
	import bwSwiper from '@/components/bw-swiper/bw-swiper.vue'

	export default {
		  components: {bwSwiper},
		data() {
			return {
				title: 'Hello',
				autoplay:true,
				bannerList:[
					{img:"http://1812.img.pp.sohu.com.cn/images/blog/2009/11/18/18/8/125b6560a6ag235.jpg",
					text:"落雨",
					
					},
					{
						img:"http://1812.img.pp.sohu.com.cn/images/blog/2009/11/18/18/8/125b6560a6ag214.jpg",
						text:"阿斯蒂芬",
					
					},{
					img:"https://ossweb-img.qq.com/images/lol/web201310/skin/big25011.jpg",
					text:"乖哈是",
					
					},
					
					]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
