<template>
	<div class="container">
		<div class="main">
			<img src="@/assets/image-equilibrium.jpg" alt="nft image">
			
			<div class="overlay">
				<img src="@/assets/icon-view.svg" alt="view icon">
				<div class="blue-overlay"></div>	
			</div>

			<h3 class="nft-title">Equilibrium #3429</h3>
			<p class="nft-description">Our equilibrium collection promotes balance and calm.</p>
			<div class="nft-infos">
				<div class="nft-price">
					<img src="@/assets/icon-ethereum.svg" alt="eth icon" />	
					<h4 class="price-amount">0.041 ETH</h4>
				</div>
				<div class="nft-time-left">
					<img src="@/assets/icon-clock.svg" alt="">
					<p>3 days left</p>
				</div>
			</div>
		</div>
		<hr>
		<div class="creator">
			<img src="@/assets/image-avatar.png" alt="user avatar" />
			<p>Creation of <b>Jules Wyvern</b></p>
		</div>
	</div>
</template>

<script setup>
	
</script>

<style lang="scss">

	.container {
		
		--padding-card:20px;

		position: absolute;
		top: 0;
		left: 50vw;
		transform: translate(calc(-50%), 5vh);

		background-color: hsl(216, 50%, 16%);
		padding: var(--padding-card);

		width: 320px;

		border-radius: 20px;

		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.main { 

		h3 {
			display: flex;
			color:white;

			cursor: pointer;

			&:active {
				color: hsl(178, 100%, 50%);
			}
		}

		p {
			display: flex;
			text-align: left;
		}

		&>img {

			cursor: pointer;

			& + .overlay {
				img {
					position: absolute;
					margin-top: -52%;
					margin-left: -6%;

					display: none;
				}

				div {

					cursor: pointer;

					transform: translateY(calc(-101%));

					position: absolute;

					width:320px;
					height:320px;

					background-color: hsl(178, 100%, 50%);
					opacity: 0.5;

					border-radius: 20px;

					display: none;

				}
			}

			width: 320px;
			border-radius: 20px;

			&:active {

				cursor: pointer;

				& + .overlay {
					div {
						display: block;
					}

					img {
						display: inline;
					}
				}

			}
		}

	}

	.nft-infos {

		display: flex;
		flex-direction: row;
		justify-content: space-between;

		.nft-price {
			
			img {
				width: 8px;
				height: 15px;
			}

			h4 {
				color: hsl(178, 100%, 50%);
				font-weight: 400;
			}

			display: flex;
			flex-direction: row;
			gap: 10px;
			align-items: center;

		}

		.nft-time-left {
			
			img {
				width: 15px;
				height: 15px;
			}

			display: flex;
			flex-direction: row;
			gap: 10px;
			align-items: center;
		}
	}

	hr {
		width: 100%;
		color: hsl(215, 32%, 27%);
	}

	.creator {

		display: flex;
		flex-direction: row;

		justify-content: flex-start;
		align-items:center;
		gap: 10px;

		img {
			width: 30px;
			border: 1px solid white;
			border-radius: 999px;
		}

		p {
			font-weight: 400;
		}

		b {

			cursor: pointer;

			color: white;
			font-weight: 400;

			&:active {
				color: hsl(178, 100%, 50%);
			}
		}

	}

	p {
		color: hsl(215, 51%, 70%);
	}

</style>