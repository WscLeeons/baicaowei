<template>
	<div class="my">
		<header>
			<div class="top">
				<router-link to="" class="login">
					<div>
						<img src="img/none_head.png" alt="">
					</div>
					<p>
						登录 / 注册>
					</p>
				</router-link>
			</div>
			<div class="bottom">
				<router-link to="">
					<p>0</p>
					<p>味豆</p>
				</router-link>
				<router-link to="">
					<p>0</p>
					<p>优惠券</p>
				</router-link>
			</div>
		</header>
		<div class="content">
			<div class="indent">
				<div class="top">
					<p>我的订单</p>
					<span>查看全部订单<i></i></span>
				</div>
				<div class="bottom">
					<router-link to="">
						<img src="img/boot.png" alt="">
						<p>待付款</p>
					</router-link>
					<router-link to="">
						<img src="img/car.png" alt="">
						<p>待发货</p>
					</router-link>
					<router-link to="">
						<img src="img/box.png" alt="">
						<p>待收获</p>
					</router-link>
					<router-link to="">
						<img src="img/msg.png" alt="">
						<p>待评价</p>
					</router-link>
					<router-link to="">
						<img src="img/smile.png" alt="">
						<p>退款/售后</p>
					</router-link>
				</div>
			</div>
			<div class="function">
				<div class="top">
					<p>常用功能</p>
				</div>
				<div class="bottom">
					<router-link to="">
						<img src="img/huangguan.png" alt="">
						<p>会员中心</p>
					</router-link>
					<router-link to="">
						<img src="img/shangcheng.png" alt="">
						<p>味豆商城</p>
					</router-link>
					<router-link to="">
						<img src="img/dizhi.png" alt="">
						<p>地址管理</p>
					</router-link>
					<router-link to="">
						<img src="img/shoucang.png" alt="">
						<p>收藏</p>
					</router-link>
					<router-link to="">
						<img src="img/help.png" alt="">
						<p>帮助中心</p>
					</router-link>
				</div>
			</div>
		</div>
		<v-footer></v-footer>
	</div>
</template>

<script>
	
</script>

<style>
.my header{
	background: url(../../assets/u_bg.png) no-repeat;
	background-size: 100% auto;
}
.my header .top{
	padding: 10% 8%;
}
.my header .top div{
	width: 60px;
	height: 60px;
}
.my header .top .login{
	display: flex;
}
.my header .top p{
	flex: 1;
	color: #fff;
    line-height: 3rem;
    padding-left: 1rem;
    font-size: 1.4rem;
}
.my header .bottom{
	padding: 10px 0;
    width: 92%;
    margin: 0 auto;
    border-radius: 10px;
    background: #fff;
    z-index: 3;
    display: flex;
}
.my header .bottom a{
	flex: 1;
	text-align: center;
}
.my header .bottom a:nth-child(2){
	border-left: 1px solid #e5e5e5;
}
.my header .bottom p{
	font-size: 1.3rem;
	line-height: 2rem;
	color: #666;
}
.my .content{
	padding-bottom: 60px;
}
.my .content .indent,.my .content .function{
	width: 92%;
	margin: 10px auto 0;
	border-radius: 10px;
	background: #fff;
	overflow: hidden;
}
.my .indent .top,.my .function .top{
	display: flex;
	border-bottom: 1px solid #ededed;
    background: #fff;
    padding: 0 4%;
    height: 45px;
    line-height: 45px;
}
.my .indent .top p{
	flex: 1;
	color: #333;
    font-size: 1.3rem;
}
.my .indent .top span{
	flex: 1;
	color: #999;
    width: 55%;
    text-align: right;
}
.my .indent .top i{
	width: 15px;
    height: 45px;
	float: right;
	display: inline-block;
	background: url(../../assets/right2.png) no-repeat 100%;
	background-size: 70%;
}
.my .indent .bottom{
	height: auto;
    line-height: 25px;
    background: #fff;
    padding: 15px 0;
	text-align: center;
}
.my .indent .bottom::after{
	content: '';
	display: block;
	clear: both;
}
.my .indent .bottom a{
	float: left;
	width: 20%;
}
.my .indent .bottom img{
	width: 30%;
}
.my .indent .bottom p{
	color: #666;
    font-size: 1.2rem;
}
.my .function .top p{
	flex: 1;
    color: #333;
    font-size: 1.3rem;
}
.my .function .bottom{
	padding: 15px 0 1px;
	height: auto;
    line-height: 25px;
    background: #fff;
}
.my .function .bottom::after{
	content: '';
	display: block;
	clear: both;
}
.my .function .bottom a{
	float: left;
	width: 25%;
	text-align: center;
	margin-bottom: 15px;
}
.my .function .bottom img{
	width: 40%
	;
}
.my .function .bottom p{
	color: #666;
    font-size: 1.2rem;
}
</style>