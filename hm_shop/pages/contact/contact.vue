<template>
	<view class="contact">
		<image class="img" src="http://www.itcast.cn/2018czydz/images/gywmban.jpg"></image>
		<view class="info">
			<view @click="phone">联系电话：400-606-5500(点击拨打)</view>
			<view>联系地址：北京市大兴区科创十一街18号院</view>
		</view>
		<map class="map" :scale="scale" :longitude=" longitude" :latitude="latitude" :markers="markers"></map>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				longitude:116.570059,
				latitude:39.791678,
				scale:20,
				 markers:[
					 {
						longitude:116.570059,
						latitude:39.791678,
						 iconPath:'../../static/01.jpg',
						 width:30,
						 height:30
					 }
				 ]
			}
		},
		methods: {
			 phone(){
				 uni.makePhoneCall({
				 	phoneNumber:'400-606-5500'
				 })
			 }
		}
	}
</script>

<style lang="scss">
.contact{
	.img{
		width: 750rpx;
		height: 320rpx;
	}
	.info{
		padding: 10rpx 20rpx;
		font-size: 30rpx;
		view{
			line-height: 60rpx;
			border-bottom: 1px solid #eee;
		}
	}
	.map{
		width: 750rpx;
		height: 750rpx;
	}
}
</style>
