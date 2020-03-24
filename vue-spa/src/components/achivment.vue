<template>
	<main class="achivment">
		<div class="container">
			<div class="achivment__container">
							<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon1.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name1}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>
					<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon2.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name2}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>
							<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon3.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name3}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>	
				</div>
				<div class="achivment__container">
<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon6.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name4}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>	
							<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon5.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name5}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>	
							<div class="achivment__item">
																<div class="img">
																	<img src="src/assets/icon4.png" alt="">
																</div>
															<div class="achivmen-text">
																<div class="achivment__name">{{name6}}</div>
																<div class="achivmen-title">{{text}}</div>
															</div>
											
							</div>	

				</div>
		</div>
	</main>
</template>

<script>
export default {
  data: function() {
    return {
				text:'Lorem ipsum dolor sit amet, adipisicing elit, sed do eiusmod tempor incididunt ut labore et',
				name1:'high resolution',
				name2:'photography',
				name3:'Editable layers',
				name4:'24/7 Support',
				name5:'powerfull theme',
				name6:'ttv',

    }
  }
}
</script>

<style scoped>

	.achivment{
		margin-top: 143px;
		background-color: #f7f9fd;
		
	}
	.achivment__item{
		margin-left: 60px;
		display: flex;
		justify-content: flex-end;
	}
	.achivment__name{
		text-transform: uppercase;
		color:#25365d;
		text-align: start;
		
	}
	.achivmen-title{
		margin-top: 29px;
		color:#5a5a5a;
	}
   .container{
  	width: 90%;
  	max-width: 1060px; 
  	margin: auto;
	}
	.achivment__container{
		padding-top: 143px;
		display: flex;
		justify-content:center;
	}
		.achivment__container:last-child{
		padding-top: 79px;
		padding-bottom: 131px;
	}
	.name-achivment{
		display: flex;
		justify-content: center;
		white-space:nowrap;
	}
.achivmen-text{
	padding-left: 34px;
	max-width: 244px;
}
@media (max-width:1058px) {
	.achivment__item{
		margin-left: 20px;
	}

}
@media (max-width:925px) {
	.achivment__item{
		margin-left: 20px;
	}
	.achivmen-text{
		padding-left: 15px;
	}
	.achivmen-title{
		margin-top: 15px;
	}

}
@media (max-width:862px) {
	.achivment__container{
		flex-direction: column;
		align-items: center;

	}
	.achivment__container:last-child{
		padding-top: 0px;
	}
	.achivment__item{
		padding-top: 30px;
	}
}
</style> 