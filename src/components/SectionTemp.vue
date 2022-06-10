<template>
	<section class="main-section">
		<div class="max-container">
			<div class="main-wrap">
				<div class="main-wrap__left">
					<div class="article-title-wrap">
						<h1 class="article-title">
							<p>Чистка</p>
							<p>квартир</p>
							<p>у Києві</p>
						</h1>
						<p class="article-subtitle">
							Ми приберемо у вас вдома чи в офісі. Наведемо чистоту після ремонту та проведемо генеральну
							прибирання.
						</p>
					</div>
				</div>
				<div class="main-wrap__right">
					<div class="article-image-wrap">
						<img class="img" :src="`${publicPath}assets/image/top.png`">
					</div>
				</div>
			</div>
		</div>
	</section>

	<section class="clear-section">
		<div class="container">
			<div class="clear-wrapper">
				<div class="clear-card" id="card1">
					<div class="clear-card__first">
						<h3 class="clear-card__title">Ретельно<br>відібраний<br>персонал</h3>
						<img class="img" src="assets/image/image1.png">
					</div>
					<div class="clear-card__second">
						<h4 class="clear-card__title">Перед тим, як взяти на роботу, ми співбесідуємо та перевіряємо
							персонал. Кожен клінер проходить навчання за підсумком якого пише тест та здає
							іспит.
							Зі 100 кандидатів ми беремо приблизно 5.</h4>
					</div>
				</div>
				<div class="clear-card" id="card2">
					<div class="clear-card__first">
						<h3 class="clear-card__title">Якісна<br>еко-хімія</h3>
						<img class="img" src="assets/image/image2.png">
					</div>
					<div class="clear-card__second">
						<h4 class="clear-card__title">Перед тим, як взяти на роботу, ми співбесідуємо та перевіряємо
							персонал. Кожен клінер проходить навчання за підсумком якого пише тест та здає
							іспит.
							Зі 100 кандидатів ми беремо приблизно 5.</h4>
					</div>
				</div>
				<div class="clear-card" id="card3">
					<div class="clear-card__first">
						<h3 class="clear-card__title">Контролюємо<br>якість</h3>
						<img class="img" src="assets/image/image3.png">
					</div>
					<div class="clear-card__second">
						<h4 class="clear-card__title">Перед тим, як взяти на роботу, ми співбесідуємо та перевіряємо
							персонал. Кожен клінер проходить навчання за підсумком якого пише тест та здає
							іспит.
							Зі 100 кандидатів ми беремо приблизно 5.</h4>
					</div>
				</div>
				<div class="clear-card" id="card4">
					<div class="clear-card__first">
						<h3 class="clear-card__title">Працюємо<br>цілодобово</h3>
						<img class="img" src="assets/image/image4.png">
					</div>
					<div class="clear-card__second">
						<h4 class="clear-card__title">Перед тим, як взяти на роботу, ми співбесідуємо та перевіряємо
							персонал. Кожен клінер проходить навчання за підсумком якого пише тест та здає
							іспит.
							Зі 100 кандидатів ми беремо приблизно 5.</h4>
					</div>
				</div>
			</div>
		</div>
	</section>

	<section class="howWork-section">
		<div class="container">
			<div class="howWork-wrapper" id="block1">
				<div class="howWork-wrapper__left">
					<h2 class="howWork-wrapper__left-text">Як ми прибираємо</h2>
				</div>
				<div class="howWork-wrapper__right">
					<h2 class="howWork-wrapper__right-text">Клінер приїжджає в призначений час з усім необхідним і
						відразу
						приступає до справи. Вам
						залишається
						тільки оцінити результат.</h2>
				</div>
			</div>
		</div>

		<div class="howWork-wrapper howWork-wrapper__bottom project" id="mySection">
			<div class="howWork-wrapper__menu">
				<h2 class="howWork-wrapper__menu-text">Як ми прибираємо</h2>

				<ul class="menu">
					<li class="menu-item active" data-elem="slide1"><span>→</span> Кухня</li>
					<li class="menu-item" data-elem="slide2">Кімнати</li>
					<li class="menu-item" data-elem="slide3">Ванна</li>
					<li class="menu-item" data-elem="slide4">Прихожа</li>
				</ul>
			</div>

			<div class="howWork-wrapper__image active" id="slide1">
				<img src="/assets/image/bg1.png" alt="name">
				<!-- підлога -->
				<div class="point" id="point0" style="top: 90%;left: 25%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Миємо підлогу</div>
					</div>
				</div>
				<!-- витяжка -->
				<div class="point" id="point1" style="top: 33%;left: 33%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо фасади витяжки</div>
					</div>
				</div>
				<!-- плитка -->
				<div class="point" id="point2" style="top: 57%;left: 25%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо плиту</div>
					</div>
				</div>
				<!-- холодильник -->
				<div class="point" id="point3" style="top: 45%;left: 60%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо холодильник</div>
					</div>
				</div>
				<!-- умивальник -->
				<div class="point" id="point4" style="top: 64%;left: 77%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо умивальник</div>
					</div>
				</div>
				<!-- поверхня -->
				<div class="point" id="point5" style="top: 75%;left: 55%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо поверхню</div>
					</div>
				</div>
				<!-- мебель -->
				<div class="point" id="point6" style="top: 60%;left: 44%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо мебель</div>
					</div>
				</div>
			</div>
			<div class="howWork-wrapper__image" id="slide2">
				<img src="/assets/image/bg1.png" alt="name">
				<!-- підлога -->
				<div class="point" id="point0" style="top: 90%;left: 25%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Миємо підлогу</div>
					</div>
				</div>
				<!-- витяжка -->
				<div class="point" id="point1" style="top: 33%;left: 33%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо фасади витяжки</div>
					</div>
				</div>
				<!-- плитка -->
				<div class="point" id="point2" style="top: 57%;left: 25%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо плиту</div>
					</div>
				</div>
				<!-- холодильник -->
				<div class="point" id="point3" style="top: 45%;left: 60%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо холодильник</div>
					</div>
				</div>
				<!-- умивальник -->
				<div class="point" id="point4" style="top: 64%;left: 77%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо умивальник</div>
					</div>
				</div>
				<!-- поверхня -->
				<div class="point" id="point5" style="top: 75%;left: 55%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо поверхню</div>
					</div>
				</div>
				<!-- мебель -->
				<div class="point" id="point6" style="z-index: 3;top: 60%;left: 44%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо мебель</div>
					</div>
				</div>
			</div>
			<div class="howWork-wrapper__image" id="slide3">
				<img src="/assets/image/bg2.png" alt="name">
				<!-- зеркало -->
				<div class="point" id="point7" style="top: 25%;left: 30%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо зеркало</div>
					</div>
				</div>
				<!-- меблі -->
				<div class="point" id="point8" style="top: 85%;left: 43%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо меблі</div>
					</div>
				</div>
				<!-- унітаз -->
				<div class="point" id="point9" style="top: 90%;left: 60%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо унітаз</div>
					</div>
				</div>
				<!-- ваннну -->
				<div class="point" id="point10" style="top: 85%;left: 80%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо ванну</div>
					</div>
				</div>
				<!-- плитку -->
				<div class="point" id="point11" style="top: 45%;left: 65%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо плитку</div>
					</div>
				</div>
			</div>
			<div class="howWork-wrapper__image" id="slide4">
				<img src="/assets/image/bg2.png" alt="name">
				<!-- зеркало -->
				<div class="point" id="point7" style="top: 25%;left: 30%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо зеркало</div>
					</div>
				</div>
				<!-- меблі -->
				<div class="point" id="point8" style="top: 85%;left: 43%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо меблі</div>
					</div>
				</div>
				<!-- унітаз -->
				<div class="point" id="point9" style="top: 90%;left: 60%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо унітаз</div>
					</div>
				</div>
				<!-- ваннну -->
				<div class="point" id="point10" style="top: 85%;left: 80%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо ванну</div>
					</div>
				</div>
				<!-- плитку -->
				<div class="point" id="point11" style="top: 45%;left: 65%;">
					<img class="plus" src="/assets/image/plus.png">
					<div class="point-wrap">
						<div class="point-wrap-content">Чистимо плитку</div>
					</div>
				</div>
			</div>

		</div>

	</section>
</template>

<script>
//GSAP
import gsap from 'gsap';
// get other plugins:
// import ScrollTrigger from "gsap/ScrollTrigger";
// import Flip from "gsap/Flip";
// import Draggable from "gsap/Draggable";

gsap.config({
	// nullTargetWarn: false,
	// trialWarn: false,
});

export default {
	name: 'SectionTemp',
	props: {
		msg: String,
	},

	data() {
		return {
			publicPath: process.env.BASE_URL
		}
	}
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.main {
	&-section {
		height: 100vh;
		overflow: hidden;
		margin-top: -70px;

		@media (max-width: 991.99px) {
			height: auto;
		}

		@media (max-width: 768px) {
			width: 100%;
			min-height: 555px;
			height: 50vh;
		}
	}

	&-wrap {
		display: flex;
		flex-direction: row-reverse;
		flex-wrap: wrap;

		&__left,
		&__right {
			width: 50%;

			@media (max-width: 991.99px) {
				width: 100%;
				min-height: 100vh;
				height: 100%;
			}

			@media (max-width: 768px) {
				width: 100%;
				min-height: 555px;
				height: 50vh;
				height: 100%;
				overflow: hidden;
			}
		}

		&__left {
			position: relative;

			@media (max-width: 991.99px) {
				position: absolute;
			}

			.article-title-wrap {
				position: absolute;
				top: calc(50% - 10px);
				left: 50%;
				transform: translate(-50%, -50%);

				max-width: 401px;
				width: 100%;

				@media (max-width: 991.99px) {
					background-color: #fff9;
					padding: 10px;
					border-radius: 8px;
					max-width: 290px;
					width: 100%;
				}
			}

			.article-title {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 400;
				font-size: 76px;
				line-height: 110%;
				color: #404040;
				text-align: left;
				margin: 0 0 30px;

				@media (max-width: 991.99px) {
					text-align: center;
					font-size: 50px;
				}

				p {
					margin: 0;
					text-align: inherit;
				}
			}

			.article-subtitle {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 400;
				font-size: 18px;
				line-height: 140%;
				color: #404040;
				text-align: left;
				max-width: 397px;
				margin: 0;

				@media (max-width: 991.99px) {
					text-align: center;
				}
			}
		}

		&__right {
			.article-image-wrap {
				height: 100vh;

				@media (max-width: 768px) {
					width: 100%;
					min-height: 70vh;
					height: 100%;
				}

				.img {
					width: 100%;
					height: 100vh;
					object-fit: cover;

					@media (max-width: 768px) {
						width: 100%;

						min-height: 555px;
						height: 50vh;
					}
				}
			}
		}
	}
}

.clear {
	&-section {
		padding-top: 73px;
		padding-bottom: 50px;
	}

	&-wrapper {
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
	}

	&-card {
		max-width: 300px;
		width: 300px;
		max-height: 328px;
		min-height: 328px;
		height: 100%;
		margin: 0 20px 40px;
		background: #F3F6FB;
		border-radius: 8px;
		position: relative;

		@media (max-width: 991.99px) {
			margin: 0 10px 20px;
		}

		&__title {
			font-family: 'TT Travels';
			font-style: normal;
			font-weight: 500;
			font-size: 24px;
			line-height: 130%;
			text-align: center;
			color: #404040;
			z-index: 1;
		}

		&__first {
			position: absolute;
			width: 100%;
			height: 100%;

			.clear-card__title {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 500;
				font-size: 24px;
				line-height: 130%;
				text-align: center;
				color: #404040;
				position: absolute;
				top: 20px;
				left: 50%;
				transform: translateX(-50%);
				position: relative;
				z-index: 2;
				margin: 0;
			}

			img {
				object-fit: cover;
				height: 100%;
				width: 100%;
				position: absolute;
				top: 0;
				left: 0;
				z-index: 1;
			}
		}

		&__second {
			height: 100%;
			width: 100%;
			position: absolute;
			top: 0;
			left: 0;
			display: none;
			background: #5A30F0;
			border-radius: 9px;
		}

		&:hover {
			.clear-card__first {
				.clear-card__title {
					display: none;
				}

				img {
					-webkit-animation-name: fadeOut;
					animation-name: fadeOut;
					-webkit-animation-duration: 2s;
					animation-duration: 2s;
					-webkit-animation-fill-mode: both;
					animation-fill-mode: both;
				}
			}

			.clear-card__second {
				display: block;

				.clear-card__title {
					padding: 30px;
					margin: 0;
					font-family: 'TT Travels';
					font-style: normal;
					font-weight: 400;
					font-size: 16px;
					line-height: 140%;
					color: #FFFFFF;
					text-align: left;
				}
			}
		}
	}
}

@-webkit-keyframes fadeOut {
	0% {
		opacity: 1;
	}

	100% {
		opacity: 0;
	}
}

@keyframes fadeOut {
	0% {
		opacity: 1;
	}

	100% {
		opacity: 0;
	}
}

.howWork {
	&-section {
		padding-top: 100px;

		@media (max-width: 991.99px) {
			padding-top: 10px;
		}
	}

	&-wrapper {
		display: flex;
		padding-bottom: 52px;

		@media (max-width: 991.99px) {
			flex-direction: column;
			align-content: center;
		}

		&__left,
		&__right {
			width: 50%;

			@media (max-width: 991.99px) {
				width: 100%;
				display: flex;
				justify-content: center;
			}

			&-text {
				text-align: left;
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 400;
				font-size: 44px;
				line-height: 120%;
				color: #404040;
				padding: 0 15px;
				position: relative;
			}
		}

		&__right {

			&-text {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 400;
				font-size: 18px;
				line-height: 140%;
				color: #404040;
				max-width: 414px;
			}
		}

		&__bottom {
			padding-bottom: 50px;
			height: 100vh;
			overflow: hidden;
			position: relative;

			@media (max-width: 991px) {
				padding-bottom: 0;
				height: 1000px;
			}
		}

		&__menu {
			background: #5A30F0;
			max-width: 20vw;
			min-width: 20vw;
			padding: 35px 53px;
			position: relative;
			z-index: 2;
			left: -40vw;

			@media (max-width: 991.99px) {
				max-width: 100%;
				left: auto;
			}

			&-text {
				font-family: 'TT Travels';
				font-style: normal;
				font-weight: 500;
				font-size: 16px;
				line-height: 130%;
				color: #FFFFFF;
				text-align: left;
				margin-bottom: 200px;

				@media (max-width: 991.99px) {
					display: none;
				}
			}

			.menu {
				@media (max-width: 991.99px) {
					max-width: 100%;
					// display: flex;
					// justify-content: center;
					// flex-direction: column;
					// align-content: center;
				}

				&-item {
					font-family: 'TT Travels';
					font-style: normal;
					font-weight: 400;
					font-size: 44px;
					line-height: 120%;
					color: #FFFFFF;
					opacity: 0.7 !important;
					text-align: left;
					width: 100%;
					margin-bottom: 22px;

					&.active,
					&:hover {
						font-family: 'TT Travels';
						font-style: italic;
						font-weight: 400;
						font-size: 44px;
						line-height: 120%;
						color: #FFFFFF;
						opacity: 1 !important;
						cursor: pointer;
					}
				}
			}
		}

		&__image {
			max-width: 75vw;
			width: 100%;
			position: relative;
			left: -10vw;

			transform: translateX(-4%);
			display: none;

			@media (max-width: 991px) {
				left: auto;
				transform: none;
				min-height: 598px;
				height: 100%
			}

			+.howWork-wrapper__image {
				display: none;
				left: auto !important;
				overflow: hidden;
			}

			.point {
				position: absolute;
				top: 50%;
				left: 50%;
				width: 30px;
				height: 30px;
				border-radius: 100%;
				background: #5A30F0;
				display: flex;
				align-items: center;
				justify-content: center;
				z-index: 4;
				cursor: pointer;
				opacity: 0;

				.plus {
					max-width: 17px;
					width: 100%;
					max-height: 17px;
					height: 100%;
					transform: rotate(0deg);
					transition: transform 1s ease;
				}

				@media (max-width: 991px) {
					&#point0 {
						top: 94% !important;
						left: 30% !important;
					}
				}

				@media (max-width: 768px) {
					&#point0 {
						top: 85% !important;
						left: 25% !important;
					}

					&#point1 {
						left: 25% !important;
					}

					&#point7 {
						left: 25% !important;
					}

					&#point8 {
						left: 35% !important;
					}

					&#point10 {
						left: 85% !important;
					}

					&#point11 {
						left: 75% !important;
					}
				}

				@media (max-width: 700px) {
					&#point4 {
						left: 85% !important;
					}

					&#point5 {
						left: 65% !important;
					}
				}

				@media (max-width: 525px) {
					&#point1 {
						left: 15% !important;

						.point-wrap {
							left: 80px;

							&::before {
								left: 5%;
							}
						}
					}

					&#point2 {
						left: 15% !important;

						.point-wrap {
							left: 80px;

							&::before {
								left: 5%;
							}
						}
					}

					&#point4 {
						left: 90% !important;

						.point-wrap {
							left: -80px;

							&::before {
								left: 95%;
							}
						}
					}

					&#point7 {
						left: 15% !important;

						.point-wrap {
							left: 80px;

							&::before {
								left: 5%;
							}
						}
					}

					&#point8 {
						left: 25% !important;

						.point-wrap {
							left: 80px;

							&::before {
								left: 5%;
							}
						}
					}

					&#point10 {
						left: 90% !important;

						.point-wrap {
							left: -80px;

							&::before {
								left: 95%;
							}
						}
					}

					&#point11 {
						left: 80% !important;

						.point-wrap {
							left: -80px;

							&::before {
								left: 95%;
							}
						}
					}
				}

				@media (max-width: 414px) {
					&#point0 {
						top: 87% !important;
						left: 10% !important;

						.point-wrap {
							left: 80px;

							&::before {
								left: 5%;
							}
						}
					}

					&#point1 {
						left: 5% !important;
					}

					&#point2 {
						left: 5% !important;
					}

					&#point3 {
						left: 75% !important;

						.point-wrap {
							left: -75px;

							&::before {
								left: 90%;
							}
						}
					}

					&#point7 {
						left: 5% !important;
					}

					&#point8 {
						left: 15% !important;
						top: 78% !important;
					}

					&#point9 {
						top: 80% !important;
						left: 65% !important;
					}

					&#point10 {
						top: 80% !important;
					}
				}

				.point-wrap {
					opacity: 0;
					// pointer-events: none;
					display: none;
					border-radius: 2px;
				}

				&.active {
					.plus {
						transform: rotate(45deg);
						transition: transform 1s ease;
					}

					.point-wrap {
						position: absolute;
						bottom: 100%;
						left: 0;
						width: 182px;
						margin: 0 0 0 -76px;
						transition: opacity .4s;
						padding: 0;
						opacity: 1;
						pointer-events: auto;
						background-color: #fff;
						display: block;

						&::before {
							content: '';
							position: absolute;
							display: block;
							width: 0;
							height: 0;
							border-style: solid;
							border-width: 4px 4px 0 4px;
							border-color: #fff transparent transparent transparent;
							left: 50%;
							bottom: -4px;
							margin: 0 0 0 -4px;
						}

						&-content {
							font-family: 'TT Travels';
							font-style: normal;
							font-weight: 500;
							font-size: 13px;
							line-height: 130%;
							text-align: center;
							color: #636C81;
							display: flex;
							justify-content: center;
							align-items: center;
							padding: 10px;
						}
					}
				}

				&::before {
					content: '';
					position: absolute;
					display: block;
					top: 0;
					left: 0;
					background: #5A30F0;
					width: 30px;
					height: 30px;
					flex: 0 0 30px;
					border-radius: 50%;
					animation: pulse 2s infinite normal both;
					z-index: -1;
					opacity: 0;
					pointer-events: none;
				}
			}

			&.active {
				display: block;
				overflow: hidden;

				.point {
					-webkit-animation: display-none-transition 7s both;
					animation: display-none-transition 7s both;
				}

				img {
					animation-duration: 2s;
					animation-name: slidein;
				}
			}

			&.fixed {
				display: block;
				position: absolute;
				z-index: 1;
				transform: translateX(-50%);
				height: 100vh;
				right: 0;
				width: 80vw;
				left: auto !important;

				@media (max-width: 991px) {
					width: 100vw;
					max-height: 598px;
					height: 100%;
					bottom: 0;
					transform: translateX(0%);
				}
			}

			@media (max-width: 991.99px) {
				max-width: 100%;
			}

			img {
				width: 100%;
				height: 100%;
				object-fit: cover;
			}
		}
	}
}

@-webkit-keyframes display-none-transition {
	0% {
		opacity: 0;
	}

	to {
		opacity: 1;
	}
}

@keyframes display-none-transition {
	0% {
		opacity: 0;
	}

	to {
		opacity: 1;
	}
}

@-webkit-keyframes pulse {
	0% {
		opacity: .9;
		transform: scale(1);
	}

	to {
		opacity: 0;
		transform: scale(2);
	}
}

@keyframes pulse {
	0% {
		opacity: .9;
		transform: scale(1);
	}

	to {
		opacity: 0;
		transform: scale(2);
	}
}

@-webkit-keyframes slidein {
	from {
		transition: all .2s ease-in-out;
		transform: scale(1.3);
	}

	to {
		transition: all .2s ease-in-out;
		transform: scale(1);
	}
}

@keyframes slidein {
	from {
		transition: all .2s ease-in-out;
		transform: scale(1.3);
	}

	to {
		transition: all .2s ease-in-out;
		transform: scale(1);
	}
}
</style>
