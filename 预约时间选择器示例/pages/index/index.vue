<template>
	<view class="wrapper">
	
			<times @change="getTime" :intervalTime="intervalTime"
			:appointStartTime="appointStartTime" :appointEndTime="appointEndTime" :appointPosNum="appointPosNum"
			:startTime="startTime" :appoTime="appoTime" :endTime="endTime"></times>
	</view>
</template>

<script>
	import times from '@/components/pretty-times/pretty-times.vue'
	export default {
		components: {
		    times
		},
		data() {
			return {
				startTime:'09:00:00',
				endTime:'19:00:00',
				intervalTime: 30,
				appointStartTime: 1,
				appointEndTime: 7,
				appointPosNum: 3,
				appoTime:[{"date":"2021-05-06","time_id":"16:30","used_pos_num":1},{"date":"2021-05-07","time_id":"17:00","used_pos_num":2}]
			}
		},
	
		methods: {
			getTime(e) {
				console.log(e)
			},
			
			
		}
	}
</script>

<style>
</style>
