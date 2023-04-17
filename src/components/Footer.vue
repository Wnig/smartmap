<template>
  <footer>
  	<div class="pc">
	  	<div class="footer">
	  		<h1>TEL：400-861-8089 / 0592-5917068<span>|</span>ADD：厦门市思明区观音山商务营运中心18号4层<span>|</span> E-mail：smartmap@smartmapdt.com</h1>
	  		<p>Copyright © 2012-2018 Smartmapdt.All Rights Reserved 闽ICP备16018304号-1</p>
	  	</div>
  	</div>
  	<div class="mob">
  		<h4>ADD：厦门市思明区观音山商务营运中心18号4层<br/>
			TEL：400-861-8089 / 0592-5917068<br/>
			E-mail：smartmap@smartmapdt.com</h4>
	  	<p>Copyright © 2012-2018 Smartmapdt.All Rights Reserved<br/>
		   闽ICP备16018304号-1</p>
  	</div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	footer {
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		height: 13.06vh;
		background: #292929;
	}
	h1 {
		margin-bottom: 1.3vh;
		color: #7A7A7A;
		text-align: center;
		font-family: 'PingFangSC-Light';
		font-size: 0.94vw;
	}
	h1 span {
		display: inline-block;
		width: 3vw;
		text-align: center;
	}
	p {
		color: #464646;
		text-align: center;
		font-size: 0.63vw;
		font-family: 'PingFangSC-Light';
	}
	.mob {
		display: none;
	}

	@media screen and (max-width: 750px) {
		.mob {
	      	display: block;
	    }

		footer {
			height: 23.99vh;
		}

		h4 {
			margin-bottom: 1.8vh;
			color: #7A7A7A;
			font-family: 'PingFangSC-Light';
			font-size: 3.73vw;
		}
		p {
			color: #444444;
			font-size: 2.67vw;
			font-family: 'PingFangSC-Light';
		}
	}

</style>
