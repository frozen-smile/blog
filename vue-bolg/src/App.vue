<template>
  <div id="app">
  	<header>
  			<h1>博客站测试项目</h1>
  			
  	</header>
  	
    <router-view></router-view>
    
    <footer>
    	
    </footer>
    
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
