<template>
	<footer class="footer">
		@
		<a href="https://roman.matviy.pp.ua" class="copyright">{{
				url_name
		}}</a>
	</footer>
</template>

<script scoped>
export default {
	name: 'FooterTemp',
	props: {
		url_name: String,
	},
};
</script>

<style lang="scss" scoped>
.footer {
	padding: 20px 15px;
	color: #fff;
	background-color: #42b983;

	.copyright {
		color: #fff;
		text-decoration: none;
		font-family: 'TT Travels';
		font-style: normal;
		font-weight: 500;
		font-size: 24px;
		line-height: 130%;
		text-align: center;
	}
}
</style>
