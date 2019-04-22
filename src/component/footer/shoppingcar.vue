<template>
	<div class="shoppingcar">
		<div v-if="flag">
			<loading></loading>
		</div>
		<header>
			购物车
			<div class="empty">
				<span><img src="../../../img/清空.png" alt=""></span>
			</div>
		</header>
		<div class="no-login">
			<img src="../../../img/ic_no_login.1938a8b.png" alt="">
			<p>还没有登录</p>
			<p>还等什么，快去注册登录吧~</p>
			<router-link to="" class="login">
				去登录
			</router-link>
		</div>
		<v-footer></v-footer>
	</div>
</template>

<script>
export default{
	data(){
		return{
			flag:true
		}
	},
	methods:{
		
	},
	mounted(){
		this.flag=false
	}
}
</script>

<style>
header{
	border-bottom: 1px solid #ccc;
    width: 100%;
    height: 50px;
    line-height: 50px;
    background-color: #fff;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 99;
    color: #3c4347;
    font-size: 1.4rem;
    text-align: center;
}
.empty{
	position: absolute;
    right: 0;
    top: 0;
    width: 15%;
    height: 50px;
    font-size: 1.2rem;
    text-align: center;
    padding-right: 3%;
}
.empty img{
	width: 40%;
}
.shoppingcar .no-login{
	padding-top: 30%;
	text-align: center;
}
.shoppingcar .no-login img{
	width: 30%;
}
.shoppingcar .no-login p{
	margin: 10px 0;
}
.shoppingcar .login{
	width: 30%;
    background: #ff4f39;
    height: 30px;
    line-height: 30px;
    border-radius: 20px;
    display: inline-block;
    margin-top: 10px;
    color: #fff;
}
</style>