<template>
	
	<div class="home">
		<h1>这里按时间展示各种文档</h1>
		<div class="article">
			<h2>标题</h2>
			<p>摘要</p>
		</div>
		
		<dialog></dialog>
	</div>
</template>

<script>
</script>

<style scoped="scoped" lang="scss">
	.home{
		max-width: 800px;
		margin: 0 auto;
		margin-top: 40px;
		height: 1000px;
		border: 1px solid lightgray;
		.article{
			text-align: left;
			padding-left: 50px;
			border: 1px solid gray;
		}
	}
</style>