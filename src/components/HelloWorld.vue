<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1>
    <h2>Essential Links</h2> -->
		
		<header>vue测试</header>
		<!-- <img src="./assets/logo.png" style="width:100px;height:100px;"> -->
		<footer>
			<ul class="navTab">
				<li><router-link to="/" active-class="active">主页</router-link></li>
				<li><router-link to="/HelloWorld/home" active-class="active">首页</router-link></li>
				<li><router-link to="/HelloWorld/about" active-class="active">关于</router-link></li>
				<li><router-link to="/HelloWorld/other" active-class="active">其他</router-link></li>
			</ul>
		</footer>
		<router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
// 	beforeRouteEnter (to, from, next) {
// 		console.log('组建内的守卫',to,from,window.location.hash)
// 		next(vm=>{
// 			console.log('组建实例:',vm)
// 		})
//     // 在渲染该组件的对应路由被 confirm 前调用
//     // 不！能！获取组件实例 `this`
//     // 因为当守卫执行前，组件实例还没被创建
//   },
//   beforeRouteUpdate (to, from, next) {
//     // 在当前路由改变，但是该组件被复用时调用
//     // 举例来说，对于一个带有动态参数的路径 /foo/:id，在 /foo/1 和 /foo/2 之间跳转的时候，
//     // 由于会渲染同样的 Foo 组件，因此组件实例会被复用。而这个钩子就会在这个情况下被调用。
//     // 可以访问组件实例 `this`
// 		next()
//   },
//   beforeRouteLeave (to, from, next) {
//     // 导航离开该组件的对应路由时调用
//     // 可以访问组件实例 `this`
// 		console.log('離開')
// 		next()
//   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.navTab {
		/* margin-top:44px; */
		}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
