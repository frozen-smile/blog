<template>
	<div class="page1">
		<h1>第一个页面</h1>
		<h2>{{msg}}</h2>
		<home-button></home-button>
		
		<ul>
			<li v-for="(n,index) in evenNumbers" :key="index">{{ n }}</li>
		</ul>
		
	</div>
	
</template>

<script>
	
import HomeButton from './HomeButton';

export default{
	name: 'Page1',
	data (){
		return {
			msg:'通过路由切换组件',
			numbers: [ 1, 2, 3, 4, 5 ],
		}
	},
	components: {
		'home-button':HomeButton
	},
	computed: {
	  evenNumbers: function () {
	    return this.numbers.filter(function (number) {
	      return number % 2 === 0
	    })
	  }
	}
}
</script>

<style>
	
</style>