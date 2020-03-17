<template>
	<div class="header">
		<!-- 如果图片在public目录直接用根目录 -->
		<img src="/favicon.ico" alt="">
		<span>NZ Music</span>
	</div>
</template>

<script>
	export default {
		
	}
</script>

<style lang="less" scoped>
	@import '../../style/index.less';
	.header{
		color: @yellow;
		font-size: @fs-l;
		display: flex;
		justify-content: center;
		align-items: center;
		.w(375);
		height:44px;
		img{
			width: 18px;
			height: 18px;
			margin-right: 10px;
		}
	}
</style>
