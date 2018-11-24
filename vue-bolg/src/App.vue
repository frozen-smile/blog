<template>
  <div id="app">
  	<header>
  			<h1>博客站测试项目</h1>
  			<nav-header></nav-header>
  	</header>
  	
    <router-view></router-view>
    
    <footer>
    	
    </footer>
    
  </div>
</template>

<script>

import NavHeader from './components/NavHeader';
	
export default {
    name: 'app',
    data(){
  			return{
  				
  			}
    },
    components: {
    		'nav-header':NavHeader
    }
    
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
