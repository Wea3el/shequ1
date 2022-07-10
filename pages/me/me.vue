<template>
	<view>
		<view class= "flex align-center p-2" hover-class="bg-light">
			<image src="../../static/Dr. Von Neumann.jpeg"
			style="width: 100rpx;height : 100rpx;"
			class = "rounded-circle"></image>
			<view class ="flex flex-column flex-1 px-2">
				<text class="font-lg font-weight-bold text-dark">昵称</text>
				<text class = "font text-muted">总帖子10  今日发帖0</text>
				
			</view>
			<text class = "iconfont uni-icon-arrowright"></text>
		</view>
		
		<view class ="flex align-center px-3 py-2">
			<view class ="flex-1 flex flex-column align-center justify-center"
			v-for="(item,index) in myData":key="index">
				<text class = "font-lg font-weight-bold">{{item.num}}</text>
				<text class = "font text-muted">{{item.name}}</text>
			</view>		
		</view>
		
		<view class ="p-3 py-2">
			<image src ="../../static/Dr. Von Neumann.jpeg" mode="aspectFill"
			style="height:170px; width: 100%" class = "rounded"></image>
		</view>
		
		<uni-list-item title="浏览历史" showExtraIcon>
			<text slot ="icon" class="iconfont uni-icon-arrowdown"></text>
		</uni-list-item>
		<uni-list-item title="社区认证">
			<text slot ="icon" class="iconfont uni-icon-arrowdown"></text>
		</uni-list-item>
		<uni-list-item title="审核帖子">
			<text slot ="icon" class="iconfont uni-icon-arrowdown"></text>
		</uni-list-item>
		<view>
			<button class="bg-main text-white" style ="border-radius: 50rpx;border:0;" type="primary">退出登录</button>
		</view>
	</view>
</template>

<script>
	import uniListItem from'@/uni-ui/uni-list-item/uni-list-item.vue'
	export default {
		components: {
			uniListItem
		},
		data() {
			return {
				myData:[{
					name: "帖子",
					num:1,
					
				},{
					name: "动态",
					num:1
				},{
					name: "评论",
					num:2
				},{
					name: "粉丝",
					num:1
				}]
			}
		},
		onNavigationBarButtonTap(){
			uni.navigateTo({
				url: '../user-set/user-set'
			});
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
