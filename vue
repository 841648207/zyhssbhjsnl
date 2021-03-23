<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title></title>
		<script src="js/vue.js" type="text/javascript" charset="utf-8"></script>
	</head>
	<body>
		<div id="app">
			<p v-if="s>=90">优秀</p>
			<p v-if="s>=80 && s<90">良好</p>
			<p v-if="s>=70 && s<80">中等</p>
			<p v-if="s>=60 && s<70">及格</p>
			<p v-if="s<60">不及格</p>
			{{number}}
		</div>
		
		<script type="text/javascript">
			let new Vue({
				el:'#app',
				data(){
					s:'80',
					number:Math.floor(Math.random()*10),
				},
				methods:{
					
				}
			})
		</script>
	</body>
</html>
