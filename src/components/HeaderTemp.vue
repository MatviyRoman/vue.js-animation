<template>
	<div class="button-order-wrap">
		<div class="button-order-inner">
			<button class="btn-order" id="btn-order" style="transform: translate(0px, 0px);">
				<span class="btn-order-background"></span>
				<span class="btn-order-text-wrap">
					<span class="btn-order-text">Замовити чистку</span>
				</span>
			</button>
		</div>
	</div>

	<header class="header" id="header">
		<div class="container">
			<div class="header-wrap">
				<div class="header-left">
					<div class="header-logo">
						<img src="/assets/image/logo.svg" alt="logo" width="92" height="25" />
					</div>
					<nav class="header-switcher">
						<span class="header-switcher-active">Дім</span>
						<a class="header-switcher-link" href="#">Офіс</a>
					</nav>
				</div>

				<nav class="header-menu">
					<ul class="menu">
						<li class="menu-item"><a href="#">Після ремонту</a></li>
						<li class="menu-item">
							<a href="#">Генеральне прибирання</a>
						</li>
						<li class="menu-item">
							<a href="#">Регулярне прибирання</a>
						</li>
						<li class="menu-item"><a href="#">Мийка вікон</a></li>
					</ul>
				</nav>

				<div class="header-right">
					<div class="header-tel-widget">
						<a class="phone-number" href="tel:+380674016977">+380 67 401 69 77</a>
						<span class="header-tel-delimiter">|</span>
						<span class="header-work">24/7</span>
					</div>
					<button class="btn-menu" id="menu" v-on:click="isHidden = !isHidden">
						<span></span>
						<span></span>
					</button>

					<div class="main-menu-wrap" v-if="!isHidden">
						<ul class="menu">
							<li class="menu-item"><a href="#">Після ремонту</a></li>
							<li class="menu-item">
								<a href="#">Генеральне прибирання</a>
							</li>
							<li class="menu-item">
								<a href="#">Регулярне прибирання</a>
							</li>
							<li class="menu-item"><a href="#">Мийка вікон</a></li>
						</ul>
					</div>

				</div>
			</div>
		</div>
	</header>
</template>

<script>
export default {
	name: 'HeaderTemp',

	names: "Menu",
	data() {
		return {
			isHidden: true
		}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import 'normalize.css/normalize.css';

a {
	text-decoration: none;
}

.header {
	display: flex;
	align-items: center;
	max-height: 70px;
	position: relative;
	z-index: 1;
	background-color: transparent;

	&-wrap {
		display: flex;
		justify-content: space-between;
		padding: 0 15px;
		max-height: 70px;
		height: 100%;

		@media (max-width: 991px) {
			padding: 10px 15px;
		}
	}

	a {
		color: #000;

		@media (max-width: 768px) {
			color: #000;
		}
	}

	&.is-sticky {
		position: fixed;
		top: 0;
		right: 0;
		left: 0;
		z-index: 1030;
		width: 100%;
		-webkit-animation: .95s ease-in-out 0s normal none 1 running fadeInDown;
		animation: .95s ease-in-out 0s normal none 1 running fadeInDown;
		-webkit-transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
		transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

		background: #FFFFFF;
		box-shadow: 0px 2px 14px rgba(0, 0, 0, 0.07);
		-webkit-box-shadow: 0px 2px 14px rgba(0, 0, 0, 0.07);
	}

	&-left {
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	&-logo {
		display: flex;
		align-items: center;
		margin-right: 25px;
	}

	&-switcher {
		background: #FFFFFF;
		border: 1px solid #E2E8F0;
		border-radius: 48px;
		max-width: 131px;
		min-width: 131px;
		width: 100%;
		max-height: 38px;
		height: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 3px 0;

		@media (max-width: 991px) {
			display: none;
		}

		@media (max-width: 425px) {
			display: flex;
		}

		&-active {
			font-family: 'TT Travels';
			font-style: normal;
			font-weight: 500;
			font-size: 14px;
			line-height: 110%;
			color: #FFFFFF;
			max-width: 55px;
			width: 100%;
			height: 34px;
			background: #5A30F0;
			border-radius: 34px;
			display: flex;
			justify-content: center;
			align-items: center;
			padding: 0 3px;
		}

		&-link {
			font-family: 'TT Travels';
			font-style: normal;
			font-weight: 500;
			font-size: 14px;
			line-height: 110%;
			color: #636C81;

			min-width: 55px;
			height: 34px;
			background: transparent;
			border-radius: 34px;

			display: flex;
			justify-content: center;
			align-items: center;
			text-decoration: none;
			padding: 0 3px;

			&:hover {
				background: #5a30f079;
				color: #fff;
			}
		}
	}

	&-menu {
		display: flex;

		.menu {
			display: flex;

			@media (max-width: 991px) {
				display: none;
			}
		}

		.menu-item {
			display: flex;
			align-items: center;

			a {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 500;
				font-size: 16px;
				line-height: 120%;
				display: flex;
				align-items: center;
				letter-spacing: 0.2px;
				color: #404040;
				transition: color 0.8s ease;

				&:hover {
					transition: color 0.8s ease;
					color: #5a30f0;
				}
			}
		}
	}

	&-right {
		display: flex;
		position: relative;

		.phone-number {
			font-family: 'TT Travels';
			font-style: normal;
			font-weight: 500;
			font-size: 16px;
			line-height: 120%;
			letter-spacing: 0.2px;
			color: #404040;
			white-space: nowrap;
		}

		.header-tel-widget {
			display: flex;
			align-items: center;

			@media (max-width: 425px) {
				display: none;
			}
		}

		.header-tel-delimiter {
			padding: 0 15px;
		}

		.header-work {
			font-family: 'TT Travels';
			font-style: normal;
			font-weight: 500;
			font-size: 16px;
			line-height: 120%;
			letter-spacing: 0.2px;
			color: #404040;
		}

		.btn-menu {
			margin-left: 37px;
			max-width: 20px;
			min-width: 20px;
			width: 100%;
			border: none;
			background-color: transparent;
			padding: 0;
			cursor: pointer;

			@media (max-width: 414px) {
				margin-left: 15px;
			}

			span {
				background-color: #404040;
				width: 100%;
				height: 2px;
				display: block;

				+span {
					margin-top: 8px;
				}
			}
		}

		.main-menu-wrap {
			position: absolute;
			top: 50px;
			right: 0;
			background-color: #fff;
			border: 1px solid #d0d0d0;
			border-radius: 5px;

			@media (max-width: 414px) {
				min-width: 290px;
			}

			.menu {
				display: flex;
				flex-direction: column;

				&-item {
					a {
						display: block;
						text-align: left;
						padding: 7px 5px;
						font-family: 'TT Travels';
						font-style: normal;
						font-weight: 500;
						font-size: 16px;
						line-height: 120%;
						display: flex;
						align-items: center;
						letter-spacing: 0.2px;
						color: #404040;

						&:hover {
							background-color: #5a30f0;
							color: #fff;
						}
					}
				}
			}
		}
	}
}

.button-order {
	&-wrap {
		position: absolute;
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
		pointer-events: none;
	}

	&-inner {
		height: 100%;
		position: relative;
		overflow: hidden;
	}

	&-invert {
		background: #09cdc8;
	}
}

.btn-order {
	transform: translate(0px, 0px);
	width: 195px;
	height: 195px;
	display: inline-flex;
	justify-content: center;
	align-items: center;
	letter-spacing: 0.03em;
	text-transform: uppercase;
	color: #fff;
	font-weight: 600;
	font-size: 18px;
	padding: 15px;
	line-height: 130%;
	position: fixed;
	left: 50%;
	bottom: 20px;
	margin: 0 0 0 -98px;
	z-index: 400;
	transform: scale(0);
	pointer-events: auto;
	transition: bottom .4s ease;
	border: none;
	background: transparent;
	padding: 0;
	box-shadow: none;
	cursor: pointer;

	transition: transform ease 1s, width ease 1s, height ease 1s;

	&:hover {
		width: 195px !important;
		height: 195px !important;
		transform: translate(0px, 0px) !important;

		transition: transform ease 1s, width ease 1s, height ease 1s;

		&::after {
			content: '';
			transform: scale(1);
			position: absolute;
			top: -40%;
			left: -40%;
			width: 180%;
			height: 180%;
			border: 2px solid #fff;
			border-radius: 50%;
			z-index: 2;
			pointer-events: none;
			opacity: .13;
			transition: transform .4s ease;
		}
	}


	&-background {
		transform: scale(0.77, 0.77);
		position: absolute;
		top: -15%;
		left: -15%;
		width: 130%;
		height: 130%;
		border-radius: 50%;
		background: #5a30f0;
		border: 1px solid rgba(255, 255, 255, 0.1);
		z-index: 4;
		pointer-events: none;
		transform: scale(.77);
		transition: background .4s ease;
	}

	&-text-wrap {
		transform: translate(0px, 0px);
		display: inline-flex;
		position: relative;
		z-index: 6;
		pointer-events: none;
	}

	&-text {
		display: inline-flex;
		position: relative;
		max-width: 100px;
		width: 100%;

		font-family: 'TT Travels';
		font-style: normal;
		font-weight: 500;
		font-size: 18px;
		line-height: 130%;
		align-items: center;
		text-align: center;
		letter-spacing: 0.03em;
		text-transform: uppercase;
		color: #FFFFFF;

		-webkit-animation: spin 10s linear infinite;
		-moz-animation: spin 10s linear infinite;
		animation: spin 10s linear infinite;
	}

	&::after {
		content: '';
		position: absolute;
		top: -40%;
		left: -40%;
		width: 180%;
		height: 180%;
		border: 2px solid #fff;
		border-radius: 50%;
		z-index: 2;
		pointer-events: none;
		opacity: .13;
		transform: scale(.5);
		transition: transform .4s ease;
	}
}

@-moz-keyframes spin {
	100% {
		-moz-transform: rotate(360deg);
	}
}

@-webkit-keyframes spin {
	100% {
		-webkit-transform: rotate(360deg);
	}
}

@keyframes spin {
	100% {
		-webkit-transform: rotate(360deg);
		transform: rotate(360deg);
	}
}
</style>
