<template>
	<div class="register">
		<transition mode="out-in">
			<phone></phone>
			<password></password>
			<other-info></other-info>
		</transition>
	</div>
</template>

<script>
	import Vue from 'vue';
	new Vue({
		el: '#register',
		data: {
			view: 'phone'
		},
		components: {
			'phone': {
				template: '<input type="number">'
			},
			'password': {
				template: ''
			},
			'other-info': {
				template: ''
			}
		}
	});
</script>

<style>
	#register {
		margin-top: 100px;
	}
</style>