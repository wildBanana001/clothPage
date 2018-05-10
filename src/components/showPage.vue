<template>
	<div class="container">
		<div class="showOne">
			<span v-for="(item, index) in showOne" :key="index">
				<img :src="item.img">
			</span>
		</div>
		<div class="showTwo">
			<div class="top-title">FEATURE PRODUCTS</div>
			<div class="sec-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit ac lobortis lacus</div>
			<div class="btn">
				<span class="left"> &lt; </span>
				<span class="right"> &gt; </span>
			</div>
			<div class="showTwo-show">
				<div class="showImg">
					<span v-for="(item, index) in showTwo" :key=index>
						<img :src="item.img">
						<text>{{item.msg}}</text>
					</span>
					<div class="third-title"></div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>

export default{
	data() {
		return {
			showOne: [
				{
					img: require("../assets/show/showOne01.png")
				},{
					img: require("../assets/show/showOne02.png")
				},{
					img: require("../assets/show/showOne03.png")
				}
			],
			showTwo: [
				{
					img: require("../assets/show/showTwo01.jpg"),
					msg: "INCEPTOS ORCI HAC LIBERO"
				},{
					img: require("../assets/show/showTwo02.jpg"),
					msg: "INCEPTOS ORCI HAC LIBERO"
				},{
					img: require("../assets/show/showTwo03.jpg"),
					msg: "INCEPTOS ORCI HAC LIBERO"
				},{
					img: require("../assets/show/showTwo04.jpg"),
					msg: "INCEPTOS ORCI HAC LIBERO"
				}
			]
		}
	}
}

</script>

<style scoped>
	.container {
		height: 200vh;
		margin-top: 7vh;
	}
	.container .showOne {
		height: 37vh;
		text-align: center;
		border-bottom: 3px solid #ccc;
	}
	.container .showOne img {
		width: 21vw;
		height: 30vh;
		margin-right: 2vw;
	}
	.container .showTwo {
		height: 80vh;
		text-align: center;
		border-bottom: 3px solid #ccc;
	}
	.showTwo .top-title {
		margin-top: 6vh;
		font-size: 1.5em;
		font-weight: bold;
	}
	.showTwo .sec-title {
		margin-top: 2vh;
		font-size: .7em;
		color: gray;
	}
	.showTwo .btn {
		margin-top: 4vh;
	}
	.showTwo .btn span {
		width: 5vw;
		height: 5vh;
		border-radius: 50%;
		border: 1px solid darkslategray;
	}
	.showTwo .btn .left {
		margin-right: 1vw;
		padding: 4px 3px 4px 6px;
		
	}
	.showTwo .btn .right {
		padding: 4px 6px 4px 6px;
	}
	.showTwo .btn span:hover {
		color: orange;
		cursor: pointer;
		border: 1px solid orange;
	}
	.showTwo .showImg {
		margin-top: 5vh;
	}
	.showTwo img {
		width: 18vw;
		height: 42vh;
		margin-right: 2vw;
	}
	.showTwo .showImg text {

	}
</style>