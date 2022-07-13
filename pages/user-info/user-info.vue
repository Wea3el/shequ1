<template>
	<view>
		<uni-list-item title="头像"
		<image slot="right" src= "../../static/Dr. Von Neumann.jpeg" 
		style="width: 150rpx;height: 150rpx; "
		class="rounded-circle"></image>></uni-list-item>
		<uni-list-item title="昵称"></uni-list-item>
		<uni-list-item title="性别"></uni-list-item>
		<uni-list-item title="生日"></uni-list-item>
		<uni-list-item title="情感"></uni-list-item>
		<uni-list-item title="职业"></uni-list-item>
		<uni-list-item title="家乡"></uni-list-item>
		
		<view class ="py-2 px-3">
			<button class="bg-main text-white" style ="border-radius: 50rpx;border:0;" 
			type="primary" @click="submit">完成</button>
		</view>
		
	</view>
</template>

<script>
	import uniListItem from '@/uni-ui/uni-list-item/uni-list-item.vue'
	export default {
		components:{
			uniListItem
		
		},
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
