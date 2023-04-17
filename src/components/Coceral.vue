<template>
  <div class="coceral">
  	<div class="pc">
  		<nav class="sider-nav">
	      <ul>
	        <li>
	          <p>400-861-8089</p> 
	          <i class="oneline icon-6"></i>
	        </li>
	        <li id="top">
	          <p>Top</p>
	          <i class="icon-7"></i>
	        </li>
	      </ul>
	    </nav> 
		<div class="selection selection-1">
			<video class="video1" src="../assets/video_02.mp4" autoplay="" loop=""></video>
			<div class="con">
				<app-header></app-header>
			  	<div class="cont">
				  	<div class="cont_">
				  		<h1>打造民族力量的<strong>产业互联网商会</strong></h1>
				  	</div>
			  	</div>
			</div>
		  	<div class="cons">
		  		<div class="cons_">
		  			<h1 class="title">互联网商会</h1>
		  			<h4>跨界共赢，抱团前行</h4>
		  			<ul class="menu-list">
		  				<li v-for="(navs, index) in navData" v-bind:class="{'sel-btn': index == num}" @click="selNav(index)">{{navs}}
		  				</li>
		  			</ul>
		  			<div class="list-con">
		  				<div class="list-con_">
		  					<!-- <a href="#" target="_blank" data-id="1" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/19.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>桐乡市乌镇人家网络科技股份有限公司</h2>
		  								<p>国家5A级旅游景区——滴答小镇,一块古老神奇而又美丽非凡的土地,1300年建镇史的江南水乡古镇... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  					<a href="http://cm.smartmapdt.com" target="_blank" data-id="8" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/20.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>司马图(厦门)文化传媒有限公司</h2>
		  								<p>司马图（厦门）文化传媒有限公司，全力整合线下各渠道优势广告媒介资源，致力打造... …</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.fjmxtz.com/" data-id="18" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/17.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>福建省淼鑫投资管理有限公司</h2>
		  								<p>“顺风递”是一款基于顺风车司机及私家车主自身资源打造的一款顺风速递服务…</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://dq.chuangwuyun.com/" data-id="14" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/39.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>创物云（厦门）网络科技有限公司</h2>
		  								<p>拒绝“空气”，选择“大气”。让更多的人透过大气，认识区块链的本质！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.xingzuke.cn/" data-id="19" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/34.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>猩租客(厦门)网络科技有限公司</h2>
		  								<p>猩租客公寓综合管理系统，专注解决传统公寓的痛点和难题，推出具备行业领先水平的智能物联服务平台... …</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.youyiyoula.com" target="_blank" data-id="4"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/37.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>悠游天下（厦门）文旅有限公司</h2>
		  								<p>悠易游综合旅游服务平台，值得信赖的创意趣味旅游平台！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="#" target="_blank" data-id="21"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/38.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门市佰中晟传媒有限公司</h2>
		  								<p>快快用人—综合快速用工服务平台！为有技能、有时间的你提供创造价值的平台；</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  					<a href="http://www.chuangwuyun.com/" target="_blank" data-id="20"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/24.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>创物云(厦门)网络科技有限公司</h2>
		  								<p>AI创物云电销机器人是一款通过精准语言平台，群呼潜在客户群体，并模拟销售专员沟通进行信息筛选的人工智能语音机器人。</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://yitaojin.emapgo.com.cn" target="_blank" data-id="2" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/22.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>易图通科技（北京）有限公司</h2>
		  								<p>易图通科技（北京）有限公司成立于2004年3月，拥有导航电子地图制作... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.chuangwuyun.com/ys" target="_blank" data-id="8" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/35.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>司马图(厦门)影视广告有限公司</h2>
		  								<p>以定位创新影视传播思维，助力新时代品牌变革；帮助众多强势品牌抢占和巩固品类领导者的位置，让品牌成为顾客优先选择！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://iots.lanmaxiot.com" data-id="5" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/18.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>宁波蓝密码物联网科技有限公司</h2>
		  								<p>蓝密码致力于净化水研究，提出智能+物联网+净水服务新模式。</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://wy.chuangwuyun.com/wy/#/" data-id="14" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/36.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门沃云商学文化传播有限公司</h2>
		  								<p>我们是“服务创业者，链接投资人”的沃云企业。“一切为创业者服务”是沃云企业的初衷理念</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.xinhongt.com" target="_blank" data-id="4" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/33.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门欣宏途网络科技有限公司</h2>
		  								<p>欣宏途旅游，整合境内外优质旅游产品及周边服务资源，通过社交网络所形成的人际脉络形成新的行为冲动和内在</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://abc.smartmapdt.com/ymyhh" data-id="12" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/16.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>越麦越红火（厦门）餐饮管理</h2>
		  								<p>越麦越红火餐饮管理有限公司，是一家特许经营专业从事麻辣小吃的大型连锁企业…</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.zsrenguan.com" target="_blank" data-id="5" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/23.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门中生仁管健康管理有限公司</h2>
		  								<p>中生仁管——中国首个共享中医健康管理平台，秉持用中医和協世界... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="#" target="_blank" data-id="3" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/25.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>都来用（厦门）科技有限公司</h2>
		  								<p>都来用微商城，撬动万亿市场的财富之门，帮助线下实体解决线上商城搭建... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="7" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/26.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>紫杉科技有限公司</h2>
		  								<p>紫杉科技致力于新零售微型商业综合体的智能集成专利设备的研发与推广... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="14" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/27.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>上海小儿朗信息科技有限公司</h2>
		  								<p>小二郎学堂云集国内外知名教育家、思想家、企业家各产业专家与6亿爱学习... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  					<a href="http://xth.smartmapdt.com" target="_blank" data-id="13" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/28.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门携艇网络科技有限公司</h2>
		  								<p>携艇会是一家专业打造中国领先的游艇、邮轮会籍服务预订平台，致力发展... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="" target="_blank" data-id="15" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/29.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门巨轮肽生物科技有限公司</h2>
		  								<p>巨轮肽生物科技是一家带着使命而诞生的企业，他的出现旨在为... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="16" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/30.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>速借易(厦门)科技有限公司</h2>
		  								<p>速借易是一家高科技网络信息金融服务公司。公司致力打造0门槛... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="3" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/31.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>铭记一心(福州)科技有限公司</h2>
		  								<p>旨在帮助实体产业加上互联网的双翼，打破过去实体产业与互联网难... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="9" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/32.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>快乐客(厦门)智能科技有限公司</h2>
		  								<p>泉州快乐客农业科技有限公司经营范围包括：农业技术研发；销售：农... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  				</div>
		  			</div>
		  		</div>
		  	</div>
			<app-footer></app-footer>
		</div>
	</div>
	<div class="mob">		
		<div class="selection selection-1">
			<img class="video1" src="../assets/video_02.gif">
			<div class="con">
				<app-header></app-header>
			  	<div class="cont">
				  	<div class="cont_">
				  		<h1>打造全行业领先的<br/><strong>产业联盟互联网商会</strong></h1>
				  	</div>
			  	</div>
			</div>
		  	<div class="cons">
		  		<div class="cons_">
		  			<h1 class="title">互联网商会</h1>
		  			<h4>跨界共赢，抱团前行</h4>
		  			<div class="menu-lists">
			  			<ul class="menu-list">
			  				<li v-for="(navs, index) in navData" v-bind:class="{'sel-btn': index == num}" @click="selNav(index)">{{navs}}
			  				</li>
			  			</ul>
		  			</div>
		  			<div class="list-cons">
	  					<!-- <a href="#" target="_blank" data-id="1" class="list_div">
	  						<div class="list_bg">
	  							<img src="../assets/19.jpg" alt="">
	  						</div>
	  						<div class="list_div_con">
	  							<div class="list_div_con_">
	  								<h2>桐乡市乌镇人家网络科技股份有限公司</h2>
	  								<p>国家5A级旅游景区——滴答小镇,一块古老神奇而又美丽非凡的土地,1300年建镇史的江南水乡古镇... ...</p>
	  							</div>
	  						</div>
	  						<div class="list_div_bottom">
	  							<a href="">Read more</a>
	  							<i class="icon-next"></i>
	  						</div>
	  					</a> -->
		  					<a href="http://cm.smartmapdt.com" target="_blank" data-id="8" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/20.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>司马图(厦门)文化传媒有限公司</h2>
		  								<p>司马图（厦门）文化传媒有限公司，全力整合线下各渠道优势广告媒介资源，致力打造... …</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.fjmxtz.com/" data-id="18" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/17.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>福建省淼鑫投资管理有限公司</h2>
		  								<p>“顺风递”是一款基于顺风车司机及私家车主自身资源打造的一款顺风速递服务…</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://dq.chuangwuyun.com/" data-id="14" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/39.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>创物云（厦门）网络科技有限公司</h2>
		  								<p>拒绝“空气”，选择“大气”。让更多的人透过大气，认识区块链的本质！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.xingzuke.cn/" data-id="19" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/34.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>猩租客(厦门)网络科技有限公司</h2>
		  								<p>猩租客公寓综合管理系统，专注解决传统公寓的痛点和难题，推出具备行业领先水平的智能物联服务平台... …</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.youyiyoula.com" target="_blank" data-id="4"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/37.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>悠游天下（厦门）文旅有限公司</h2>
		  								<p>悠易游综合旅游服务平台，值得信赖的创意趣味旅游平台！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="#" target="_blank" data-id="21"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/38.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门市佰中晟传媒有限公司</h2>
		  								<p>快快用人—综合快速用工服务平台！为有技能、有时间的你提供创造价值的平台；</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  					<a href="http://www.chuangwuyun.com/" target="_blank" data-id="20"class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/24.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>创物云(厦门)网络科技有限公司</h2>
		  								<p>AI创物云电销机器人是一款通过精准语言平台，群呼潜在客户群体，并模拟销售专员沟通进行信息筛选的人工智能语音机器人。</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://yitaojin.emapgo.com.cn" target="_blank" data-id="2" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/22.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>易图通科技（北京）有限公司</h2>
		  								<p>易图通科技（北京）有限公司成立于2004年3月，拥有导航电子地图制作... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.chuangwuyun.com/ys" target="_blank" data-id="8" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/35.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>司马图(厦门)影视广告有限公司</h2>
		  								<p>以定位创新影视传播思维，助力新时代品牌变革；帮助众多强势品牌抢占和巩固品类领导者的位置，让品牌成为顾客优先选择！</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://iots.lanmaxiot.com" data-id="5" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/18.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>宁波蓝密码物联网科技有限公司</h2>
		  								<p>蓝密码致力于净化水研究，提出智能+物联网+净水服务新模式。</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://wy.chuangwuyun.com/wy/#/" data-id="14" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/36.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门沃云商学文化传播有限公司</h2>
		  								<p>我们是“服务创业者，链接投资人”的沃云企业。“一切为创业者服务”是沃云企业的初衷理念</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.xinhongt.com" target="_blank" data-id="4" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/33.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门欣宏途网络科技有限公司</h2>
		  								<p>欣宏途旅游，整合境内外优质旅游产品及周边服务资源，通过社交网络所形成的人际脉络形成新的行为冲动和内在</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://abc.smartmapdt.com/ymyhh" data-id="12" target="_blank" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/16.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>越麦越红火（厦门）餐饮管理</h2>
		  								<p>越麦越红火餐饮管理有限公司，是一家特许经营专业从事麻辣小吃的大型连锁企业…</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="http://www.zsrenguan.com" target="_blank" data-id="5" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/23.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门中生仁管健康管理有限公司</h2>
		  								<p>中生仁管——中国首个共享中医健康管理平台，秉持用中医和協世界... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="#" target="_blank" data-id="3" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/25.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>都来用（厦门）科技有限公司</h2>
		  								<p>都来用微商城，撬动万亿市场的财富之门，帮助线下实体解决线上商城搭建... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="7" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/26.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>紫杉科技有限公司</h2>
		  								<p>紫杉科技致力于新零售微型商业综合体的智能集成专利设备的研发与推广... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="14" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/27.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>上海小儿朗信息科技有限公司</h2>
		  								<p>小二郎学堂云集国内外知名教育家、思想家、企业家各产业专家与6亿爱学习... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  					<a href="http://xth.smartmapdt.com" target="_blank" data-id="13" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/28.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门携艇网络科技有限公司</h2>
		  								<p>携艇会是一家专业打造中国领先的游艇、邮轮会籍服务预订平台，致力发展... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<!-- <a href="" target="_blank" data-id="15" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/29.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>厦门巨轮肽生物科技有限公司</h2>
		  								<p>巨轮肽生物科技是一家带着使命而诞生的企业，他的出现旨在为... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="16" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/30.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>速借易(厦门)科技有限公司</h2>
		  								<p>速借易是一家高科技网络信息金融服务公司。公司致力打造0门槛... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="3" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/31.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>铭记一心(福州)科技有限公司</h2>
		  								<p>旨在帮助实体产业加上互联网的双翼，打破过去实体产业与互联网难... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a>
		  					<a href="#" target="_blank" data-id="9" class="list_div">
		  						<div class="list_bg">
		  							<img src="../assets/32.jpg" alt="">
		  						</div>
		  						<div class="list_div_con">
		  							<div class="list_div_con_">
		  								<h2>快乐客(厦门)智能科技有限公司</h2>
		  								<p>泉州快乐客农业科技有限公司经营范围包括：农业技术研发；销售：农... ...</p>
		  							</div>
		  						</div>
		  						<div class="list_div_bottom">
		  							<a href="">Read more</a>
		  							<i class="icon-next"></i>
		  						</div>
		  					</a> -->
		  			</div>
		  		</div>
		  	</div>
			<app-footer></app-footer>
		</div>
		<div id="tops" class="tops"></div>
	</div>
  </div>
</template>

<script>
import Header from './Header'
import Footer from './Footer'
export default {
  name: 'Coceral',
  data () {
    return {
    	navData: ['ALL', '特色小镇', '大数据', '电商', '旅游', '大健康', '物联网', '新零售', '新传媒', '新农业', '文创', '医疗', '餐饮', '游艇', '教育', '生物科技', '互联网金融', '众创空间', '新快递', '智慧公寓', '智能科技', '同城互助', '会务', '古玩艺术'],
    	selShow: false,
    	num: 0,
    }
  },
  created() {
  },
  methods: {
    slideDown() {
      let downHeight = document.documentElement.clientHeight || document.body.clientHeight;
      window.scrollTo(0, downHeight);
      this.slideShow = true;
    },
    selNav(index) {
    	this.num = index;
    }
  },
  components: {
    'app-header': Header,
    'app-footer': Footer
  },
  mounted() {
  	// 返回顶部
    $('#top, #tops').on('click', function() {
    	$('html, body').animate({scrollTop: '0px'}, 800);
    });

  	$(window).scroll(function() {
	　　 var scrollTop = $(this).scrollTop();
	　　 var scrollHeight = $(document).height();
	　　 var windowHeight = $(this).height();

		if(scrollTop < scrollHeight / 9) {
			$('#tops').css({
				'display': 'none'
			});
		} else {
			$('#tops').css({
				'display': 'block'
			});
		}
	});

	$('.menu-list li').on('click', function() {
		var ind = $(this).index();

		for (var i = 0; i < $('.list-con .list_div, .list-cons .list_div').length; i++) {
			var id = $('.list-con .list_div, .list-cons .list_div').eq(i).attr('data-id');
			if(ind == id) {
				$('.list-con .list_div, .list-cons .list_div').eq(i).css({
					'display': 'inline-block'
				});
			} else if(ind == '0') {
				$('.list-con .list_div, .list-cons .list_div').css({
					'display': 'inline-block'
				});
			} else {
				$('.list-con .list_div, .list-cons .list_div').eq(i).css({
					'display': 'none'
				});
			}
		}
	});

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.video1 {
	    position: relative;
	    left: 0;
	    top: 0;
	    z-index: 0;
	    width: 100%;
	    height: 42.59vh;
	    -o-object-fit: fill;
	    object-fit: fill;
	}
	/*selection-1*/
	.selection-1 {
		height: auto;
		background: #f6f6f6;
	}
	.selection-1 .con {
		position: absolute;
		left: 0;
		top: 0;
		width: 100%;
		height: 42.59vh;
		background: rgba(0, 0, 0, 0.6);
	}
	
	.selection-1 .cont {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100vw;
		height: 8vw;
		color: #FFFFFF;
		text-align: center;
		line-height: 2.34vw;
		font-size: 1.3vw;
	}
	.selection-1 .cont h1 {
		margin: 0 auto;
		color: #FFFFFF;
		text-align: center;
		line-height: 4.53vw;	
		font-size: 2.86vw;
		font-family: 'PingFangSC-Semibold';
	}
	.selection-1 .cont h1 strong {
		color: #5BB8DE;
		font-family: 'PingFangSC-Semibold';
	}
	.selection-1 .cons h4 {
		margin-top: 7.96vh;
		color: #000000;
		text-align: left;
		line-height: 1.82vw;
		font-size: 1.3vw;
		font-family: 'PingFangSC-Light';
	}
	.selection-1 .cons {
		display: flex;
		justify-content: center;
		align-items: center;
		margin-bottom: 7.22vh;
		background: #fff;
	}
	.selection-1 .cons_ {
		width: 75vw;
		margin-top: 13.43vh;
	}
	.selection-1 .cons_ .menu-list {
		margin-top: 3.24vh;
		margin-bottom: 7.04vh;
	}
	.selection-1 .cons_ .menu-list li {
		display: inline-block;
		margin-right: 0.25vw;
		margin-bottom: 0.25vw;
		width: 7.08vw;
		height: 3.33vw;
		color: #000000;
		text-align: center;
		line-height: 3.33vw;
		font-size: 1.04vw;
		font-family: 'PingFangSC-Light';
		background: #F5F5F5;
		cursor: pointer;
	}
	.selection-1 .cons_ .menu-list .sel-btn {
		color: #fff;
		background: #333333;
	}

	.selection-1 .list_div {
		display: inline-block;
		width: 21.98vw;
		margin-right: 3.13vw;
		margin-bottom: 3.13vw;
		background: #FFFFFF;
		cursor: pointer;
		border: 1px solid #EDEDED;
	}
	.selection-1 .list-con {
		overflow: hidden;
		width: 100%;
	}
	.selection-1 .list-con_ {
		width: 110%;
	}
	.selection-1 .list_bg {
		overflow: hidden;
		width: 100%;
		height: 14.32vw;
	}
	.selection-1 .list_bg img {
		display: block;
		width: 100%;
		height: 100%;
		-webkit-transition: all .8s;
    	transition: all .8s;
	}
	.selection-1 .list_bg:hover img {
		-webkit-transform: scale(1.4);
	    transform: scale(1.4);
		-webkit-transition: all .8s;
    	transition: all .8s;
	}
	.selection-1 .list_div_con_ {
		width: 100%;
	}
	.selection-1 .list_div_con h2 {
		width: 100%;
		margin-bottom: 1.48vh;
		color: #000000;		
		font-family: 'PingFangSC-Regular';
		font-size: 1.3vw;
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
	}
	.selection-1 .list_div_con p {
		width: 100%;
		color: #7F7F7F;
		line-height: 1.56vw;
		font-family: 'PingFangSC-Light';
		font-size: 0.94vw;
		overflow : hidden;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 2;
		-webkit-box-orient: vertical;
	}
	.selection-1 .list_div_con {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 17.81vw;
		height: 10.74vw;
		margin: 0 auto;
		border-bottom: 1px solid #EEEEEE;
	}
	.selection-1 .list_div_bottom {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 17.81vw;
		height: 5.1vw;
		margin: 0 auto;
	}
	.selection-1 .list_div_bottom a {
		flex: 1;
		font-size: 0.94vw;
	}
	.selection-1 .list_div_bottom i {
		font-size: 1vw;
	}
	.selection-1 .list_div_bottom a:hover {
		color: #000;
	}
	.selection-1 .list-con {
		margin-bottom: 21.11vh;
	}
	


	@media screen and (max-width: 750px) {
		.mob {
			display: block;
		}
		.video1 {
		    width: 200%;
		}

		/*selection-1*/
		.selection-1 {
			height: auto;
		}
		.selection-1 .con {
			height: 42.59vh;
		}
		
		.selection-1 .cont {
			width: 100vw;
			height: 20vh;
			color: #FFFFFF;
			text-align: center;
			line-height: 2.34vw;
			font-size: 1.3vw;
		}
		.selection-1 .cont h1 {
			line-height: 12.53vw;	
			font-size: 8vw;
		}
		.selection-1 .cons h4 {
			margin-top: 7.96vh;
			line-height: 8.82vw;
			font-size: 4.8vw;
		}
		.selection-1 .cons_ {
			width: 86vw;
			margin-top: 13.43vh;
		}
		.selection-1 .menu-lists {
			overflow: hidden;
			width: 100%;
		}
		.selection-1 .cons_ .menu-list {
			width: 110%;
			margin-top: 3.24vh;
			margin-bottom: 7.04vh;
		}
		.selection-1 .cons_ .menu-list li {
			margin-right: 0.53vw;
			margin-bottom: 0.53vw;
			width: 28.27vw;
			height: 12vw;
			line-height: 12vw;
			font-size: 3.73vw;
		}

		.selection-1 .list_div {
			width: 85.8vw;
			margin-right: 0;
			margin-bottom: 6.67vw;
		}
		.selection-1 .list-cons {
			width: 100%;
			margin-bottom: 10.64vh;
		}
		.selection-1 .list_bg {
			width: 100%;
			height: 56.8vw;
		}
		.selection-1 .list_div_con_ {
			width: 100%;
		}
		.selection-1 .list_div_con h2 {
			margin-bottom: 1.5vh;
			font-size: 4.8vw;
		}
		.selection-1 .list_div_con p {
			line-height: 6.56vw;
			font-size: 3.8vw;
		}
		.selection-1 .list_div_con {
			width: 75vw;
			height: 35.6vw;
		}
		.selection-1 .list_div_bottom {
			width: 75vw;
			height: 20vw;
		}
		.selection-1 .list_div_bottom a {
			font-size: 4.8vw;
		}
		.selection-1 .list_div_bottom i {
			font-size: 3.2vw;
		}
		
		
	}

	@media screen and (min-width: 751px) {

	}
</style>
