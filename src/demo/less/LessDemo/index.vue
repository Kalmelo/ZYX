<template>
	<div>
		<h1>这里是less 案例</h1>
		<hr>
		<div class="demo">
			
			
		</div>
		<div class="test">
			<p>
				<span></span>
			</p>
		</div>
	</div>
</template>

<script>
	export default{
		
	}
</script>

<style lang="less" scoped="">
// 1rem = 37.5
@import '../../../style/index.less';
	.demo{
		.w(187.5); //width:5rem
		height: 100px;
		background: pink;
	}
	//lang 选用哪种预处理语言   
	//scoped 样式和作用域  只有在该组件和子组件可以使用
	//变量使用@
	//简单的计算
	//mixin 混合 css中的函数 可以实现对央视的封装
	@width:100px;
	@height:@width+100px;
	@color:green;
	
	.hehe(@borderColor,@w){
		border: @w solid @borderColor;
		border-radius: 30px;
	}
	.test{
		background: @color;
		width: @width;
		height: @height;
		.hehe(15px,pink);
		p{
			background: yellow;
			height: 40px;
			span{display: inline-block;
			width: 20px;
			background: purple;
			height: 20px;
				
			}
		}
	}
</style>
