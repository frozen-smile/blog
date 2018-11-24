<template>
	<header>
		<ul>
			<li>首页</li>
			<li>
				归档
				<div class="hoverList">
					<p>技术</p>
					<p>随笔</p>
				</div>
			</li>
			<li>
				相册
				<div class="hoverList">
					<p>风景</p>
					<p>生活</p>
				</div>
			</li>
			<li>留言板</li>
			<li>
				推荐
				<div class="hoverList">
					<p>电影</p>
					<p>书籍</p>
					<p>音乐</p>
					<p>漫画</p>
				</div>
			</li>
		</ul>
	</header>
	
</template>

<script>
export default {
  name: 'header',
  data (){
  	
  },
  mounted: {
  	
  }
  
}
</script>

<style scoped="scoped" lang="scss">
header{
	ul{
		max-width: 800px;
		display: flex;
		justify-content: space-around;
		font-size: 18px;
		font-weight: bold;
		margin: 0 auto;
		list-style: none;
		li{
			cursor: pointer;
			position: relative;
			
			.hoverList{
				width: 100px;
				overflow: hidden;
				height: 0;
				text-align: center;
				position: absolute;
				top: auto;
				left: 50%;
				z-index: 999;
				/*display: none;*/
				
				box-shadow: 0 0 15px rgba(180, 180, 180, 0.7);
				transform: translateX(-50%);
				background: white;
				border: 1px solid gold;
				transition: all 1.5s ease-in-out;
				p{
					line-height: 40px;
					font-weight: normal;
					margin: 0;
				}
				p:hover{
					background: skyblue;
					color: white;
				}
			}
			
		}
		li:hover .hoverList{
			/*display: block;*/
			height: auto;
		}
	}
}	
	
</style>