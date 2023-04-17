<template>
  	<header>
	  	<div class="pc">
		    <div class="cont">
				<a class="logo" @click="jump" ><img src="../assets/1.svg" alt=""></a>
				<div class="nav-btn-con">
					<div @click="isShow" class="nav-btn"></div>
				</div>	
				<div class="nav" v-if="selShow">
					<div class="nav_bg" v-show="selShow"></div>
					<div class="nav-btn_">
						<div class="nav-btn-con_">
							<div @click="isShow" class="nav-btn-sel"></div>
						</div>
					</div>
				  	<nav>
				  		<ul>
							<li v-for="(navs, index) in navData" v-bind:class="{'btn_sel': index == num}" @click="selMenus(index)">
				              <router-link :to="navs.links">{{navs.tit}}</router-link>
				            </li>
				            <li>
				            	<a href="http://www.xpaik.com" target="_blank">猩派客</a>
				            </li>
				            <li class="backstage">
				              <a href="http://add.smartmapdt.com/mall/home" target="_blank">后台登录</a>
				            </li>
				  		</ul>
				  	</nav>
				</div>
		  	</div>
	  	</div>
	  	<div class="mob">
	  		<div class="cont">
				<a class="logo" @click="jump" ><img src="../assets/1.svg" alt=""></a>
				<div class="nav-btn-con">
					<div @click="isShow" class="nav-btn"></div>
				</div>	
				<div class="nav" v-if="selShow" @click="isShow">
				  	<nav>
				  		<ul>
							<li v-for="(navs, index) in navData" v-bind:class="{'btn_sel': index == num}" @click="selMenus(index)">
				              <router-link :to="navs.links">{{navs.tit}}</router-link>
				            </li>
				            <li>
				            	<a href="http://www.xpaik.com">猩派客</a>
				            </li>
				            <li>
				              <a href="">后台登录</a>
				            </li>
				  		</ul>
				  		<div class="hot">
				            <p>全国统一客户热线：</p>
				            <h2>400-861-8089</h2>
				        </div>
				  	</nav>
				</div>
		  	</div>
	  	</div>
    </header>
</template>

<script>
let storage = window.sessionStorage;
export default {
  name: 'Header',
  data () {
    return {
    	navData: [
	        {tit: '首页', links:'/'},
	        {tit: '互联网商会', links:'/Coceral'},
        ],
      	num: '',
      	selShow: false
    }
  },
  created: function() {
    if(storage['selNumsmart']) {
      this.num = storage['selNumsmart'];
    } else {
      this.num = 0;
    };
  },
  methods: {
    selMenus(index) {
      storage['selNumsmart'] = index;
      this.selShow = false;
    },
    isShow() {
      //点击：左侧菜单栏 收起-展开
      this.selShow = ! this.selShow;
    },
    jump() {
      storage['selNumsmart'] = 0;
      this.selShow = false;
      this.$router.push({path: '/'});
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	header {
		display: flex;
		justify-content: center;
		height: 10.36vw;
	}
	.pc {
		display: flex;
		width: 90%;
	}
	.cont {
		display: inline-flex;
		align-items: center;
		width: 100%;
	}
	.logo {
		width: 16.57vw;
		cursor: pointer;
	}
	.logo img {
		display: block;
		width: 100%;
	}
	.nav-btn-con {
		width: 80%;
		cursor: pointer;
	}
	.nav-btn-con .nav-btn {
		float: right;
		width: 5.94vw;
		height: 2.34vw;
		margin-top: -2vw;
		background: url('../assets/2.svg') center center no-repeat;
		background-size: 100% 100%;
	}
	
	.nav {
		position: absolute;
		left: 0;
		top: 0;
		width: 100%;
		height: 100vh;
		z-index: 9999;
	}
	
	.nav-btn_ {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 10.36vw;
		margin-bottom: 5vh;
		cursor: pointer;
	}
	.nav-btn_ .nav-btn-sel {
		float: right;
		width: 5.94vw;
		height: 2.34vw;
		margin-top: -2vw;
		background: url('../assets/3.svg') center center no-repeat;
		background-size: 100% 100%;
	}
	.nav-btn-con_ {
		width: 88%;
	}
	
	nav ul {
		padding-left: 16.91vw;
	}
	nav li {
		display: block;
		margin-bottom: 5vh;
	}
	nav li a {
		color: #000;
		font-size: 2.34vw;
		font-family: 'PingFangSC-Light';
		-webkit-transition: font-size 0.2s;
      	transition: font-size 0.2s;
	}
	nav a {
		display: block;
		line-height: 2.76vw;
		cursor: pointer;
	}
	nav .btn_sel a {
		color: #5BB8DE;
		font-size: 2.86vw;
		font-family: 'PingFangSC-Semibold';
	}
	nav .backstage {
		padding-top: 6.85vh;
	}
	@media screen and (max-width: 750px) {
		.pc {
			display: none;
		}
		.mob {
			display: flex;
			width: 90%;
		}
		header {
			height: 22.36vw;
		}
		.cont {
			display: inline-flex;
			align-items: center;
			width: 100%;
		}
		.logo {
			flex: 1;
			width: 40.95vw;
			cursor: pointer;
		}
		.nav-btn-con {
			width: 52%;
		}
		.nav-btn-con .nav-btn {
			float: right;
			width: 22.67vw;
			height: 9.07vw;
			margin-top: -2vw;
		}
		.nav {
			position: absolute;
			left: 0;
			top: 0;
			width: 100%;
			height: 100vh;
			background: rgba(0, 0, 0, 0.65);
			z-index: 9999;
		}
		nav {
			width: 62.93vw;
			height: 100vh;
			background: #fff;
		}
		nav ul {
			padding-top: 14.33vh;
			padding-left: 9.07vw;
		}
		nav li {
			margin-bottom: 6.5vh;
		}
		nav p {
	      margin-bottom: 1.05vh;
	      color: #797979;
	      font-size: 3.2vw;
	    }
	    nav h2 {
	      color: #000000;
	      line-height: 6.67vw;
	      font-size: 6.67vw;
	      font-family: 'PingFangSC-Semibold';
	    }
	    nav .hot {
	      position: absolute;
	      left: 9.2vw;
	      bottom: 7.95vh;
	    }
	    nav li a {
	    	line-height: 7.33vw;
			font-size: 5.33vw;
		}
		nav .btn_sel a {
			font-size: 6.67vw;
		}

	}

	@media screen and (min-width: 751px) {
		.nav_bg {
			position: absolute;
			right: 0;
			top: 0;
			width: 100vw;
			height: 100vh;
			background: rgba(228, 228, 226, 0.95);
			z-index: -1;
			-webkit-animation: scaleIn 2s ease-in-out;
	    	animation: scaleIn 2s ease-in-out;
		}
		nav {
			height: 100%;
			-webkit-animation: opac 2s ease-in-out;
	    	animation: opac 2s ease-in-out;
		}


		nav li a:hover {
			color: #5BB8DE;
			font-size: 2.86vw;
			font-family: 'PingFangSC-Semibold';
			-webkit-transition: font-size 0.2s;
      		transition: font-size 0.2s;
		}


		@-webkit-keyframes scaleIn {
		    0% {
		    	width: 0vw;
		    	height: 0vw;
		    	border-radius: 50%;
		        -webkit-transform: scale(1);
		        -moz-transform: scale(1);
		        -ms-transform: scale(1);
		        -o-transform: scale(1);
			    transform: scale(1);
		    }
		    10% {
		    	width: 10vw;
		    	height: 10vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale(10);
		        -moz-transform: scale(10);
		        -ms-transform: scale(10);
		        -o-transform: scale(10);
			    transform: scale(10);
		    }
		    20% {
		    	width: 20vw;
		    	height: 20vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale(20);
		        -moz-transform: scale(20);
		        -ms-transform: scale(20);
		        -o-transform: scale(20);
			    transform: scale(20);
		    }
		    30% {
		    	width: 30vw;
		    	height: 30vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale320);
		        -moz-transform: scale(30);
		        -ms-transform: scale(30);
		        -o-transform: scale(30);
			    transform: scale(30);
		    }
		    50% {
		    	border-radius: 50%;
		        -webkit-transform: scale(50);
		        -moz-transform: scale(50);
		        -ms-transform: scale(50);
		        -o-transform: scale(50);
			    transform: scale(50);
		    }
		    60% {
		    	border-radius: 50%;
		        -webkit-transform: scale(60);
		        -moz-transform: scale(60);
		        -ms-transform: scale(60);
		        -o-transform: scale(60);
			    transform: scale(60);
		    }
		    100% {
		    	width: 100vw;
		    	height: 100vh;
		    	border-radius: 0;
		        -webkit-transform: scale(100);
		        -moz-transform: scale(100);
		        -ms-transform: scale(100);
		        -o-transform: scale(100);
			    transform: scale(100);
		    }
		}
		@keyframes scaleIn {
		    0% {
		    	width: 0vw;
		    	height: 0vw;
		    	border-radius: 50%;
		        -webkit-transform: scale(1);
		        -moz-transform: scale(1);
		        -ms-transform: scale(1);
		        -o-transform: scale(1);
			    transform: scale(1);
		    }
		    10% {
		    	width: 10vw;
		    	height: 10vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale(10);
		        -moz-transform: scale(10);
		        -ms-transform: scale(10);
		        -o-transform: scale(10);
			    transform: scale(10);
		    }
		    20% {
		    	width: 20vw;
		    	height: 20vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale(20);
		        -moz-transform: scale(20);
		        -ms-transform: scale(20);
		        -o-transform: scale(20);
			    transform: scale(20);
		    }
		    30% {
		    	width: 30vw;
		    	height: 30vw;
		    	border-radius: 50%;
		    	-webkit-transform: scale320);
		        -moz-transform: scale(30);
		        -ms-transform: scale(30);
		        -o-transform: scale(30);
			    transform: scale(30);
		    }
		    50% {
		    	border-radius: 50%;
		        -webkit-transform: scale(50);
		        -moz-transform: scale(50);
		        -ms-transform: scale(50);
		        -o-transform: scale(50);
			    transform: scale(50);
		    }
		    60% {
		    	border-radius: 50%;
		        -webkit-transform: scale(60);
		        -moz-transform: scale(60);
		        -ms-transform: scale(60);
		        -o-transform: scale(60);
			    transform: scale(60);
		    }
		    100% {
		    	width: 100vw;
		    	height: 100vh;
		    	border-radius: 0;
		        -webkit-transform: scale(100);
		        -moz-transform: scale(100);
		        -ms-transform: scale(100);
		        -o-transform: scale(100);
			    transform: scale(100);
		    }
		}

		
		@-webkit-keyframes opac {
		    0% {
				opacity: 0;
		    }
		    100% {
				opacity: 1;
		    }
		}
		@keyframes opac {
		    0% {
				opacity: 0;
		    }
		    100% {
				opacity: 1;
		    }
		}
	}
</style>
