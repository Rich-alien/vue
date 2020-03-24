<template>

    <div class="header-main">
		<p class="text">{{text}}</p>
		<p class = "sub-text">{{subtext}}</p>
		</div>

</template>

<script>
export default {
  data: function() {
    return {
				text: 'free psd web template',
				subtext: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua',
    }
  }
}
</script>

<style scoped>
p{
	margin: 0;
}

	.text{
		text-transform: uppercase;
		font-size: 61px;
		font-weight: 400;
		line-height: 32px;
		letter-spacing: 1.46px;
	}
	.header-main{
		margin-top: 115px;
		display: flex;
		align-items: center;
		flex-direction: column;
		
	}
	.sub-text{
		text-align: center;
		font-size: 24px;
		font-weight: 400;
		line-height: 42px;
		margin-top: 37px;
		max-width: 806px;
		opacity: 0.7;
	}
	@media (max-width: 886px) {
		.text{
			display: flex;
			text-align: center;
			font-size: 40px;
		}
	}

</style>