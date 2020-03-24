<template>
	<div class="container__button">
    <button class="button">{{btn}}</button>
		
		</div>
</template>

<script>
export default {
  data: function() {
    return {
        btn: 'Download',
    }
  }
}
</script>

<style scoped>

	.container__button{
		display: flex;
		margin-top: 60px;
		justify-content: center;
	}

	.button{
		border-radius: 28px;
		background-color: #25365d;
		color: #ffffff;
		font-size: 18px;
		font-weight: 700;
		line-height: 17px;
		outline: none;
		border: none;
		padding: 22px 55px 22px 39px;
		cursor: pointer;
	}
	.button:after{
		content: "";
		display: block;
		background-image: url("/src/assets/savefile.svg");
		width: 17px;
		height: 17px;
		float: left;
		
		margin-right: 18px;
	}
	.button:active{
		transform:translateY(4px) ;
	}
</style> 