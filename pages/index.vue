<template>
	<div>
		<MainpageAboutUs/>
		<MainpageSupport/>
		<MainpageCommunication/>
		<MainpageFuture/>
		<MainpageValuesCard/>
		<MainpageForYou/>
		<MainpageFaq/>
	</div>
</template>
<script setup>
definePageMeta({
	layout: 'mainpage'
})
</script>
<style lang="scss" scoped>
@import "../assets/scss/mainpage.scss";
.link__intro {
	z-index: 999;
	position: fixed;
	bottom: 30px;
	left: 20px;
	padding: 32px 52px;
	border-radius: 60px;
	font-family: 'Inter';
	font-weight: 600;
	@include adaptiv-size(24, 12, 12);
	@include adaptiv-height(36, 18, 18);
	text-transform: uppercase;
	color: #FFFFFF;
	background-color: #34057B;
	opacity: 0;
	transition: all .5s ease-in-out;
	cursor: pointer;
	@media(max-width: 1921px) {
		padding: 24px 39px;
	}
	@media (max-width: 1281px) { 
		padding: 16px 26px;
	}
	@media (max-width: 400px) {
		padding: 12px 14px;
		font-size: 10px;
	}
	@media (max-width:400px) {
		bottom: 20px;
		left: 15px;
	}
}
.link__intro:hover {
	background-color: #5A18BD;
}
</style>