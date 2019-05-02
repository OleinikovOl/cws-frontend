<template>
	<div class="register">
		<transition id="register" mode="out-in">
			<register></register>
		</transition>
	</div>
</template>

<script>
	export default({
		el: 'register',
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