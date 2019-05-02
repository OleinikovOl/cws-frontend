<template>
	<div class="register">
		<form action="" onsubmit="return false">
			<transition name="register" mode="out-in">
				<component :is="view"></component>
			</transition>
			<!-- <button id="phone_submit">Далее</button> -->
		</form>
	</div>
</template>

<script>
	export default{
		data: function() {
	return {
			view: 'phone'
		}
	},
		components: {
			'phone': {
				template: '<div class="input_group"><label for="phone">Номер телефона</label><input id="phone" name="phone" type="text"><button id="phone_submit">Далее</button></div>'
			},
			'sms_code': {
				template: '<div class="input_group"><label for="sms_code">Смс код</label><input id="sms_code" name="sms_code" type="text"></div>'
			},
			'other_info': {
				template: '<div class="input_group"><label for="first_name">Имя</label><input id="first_name" name="first_name" type="text"></div><div class="input_group"><label for="last_name">Фамилия</label><input id="last_name" name="last_name" type="text"></div><div class="input_group"><label for="city">Город</label><input id="city" name="city" type="text"></div>'
			}
		},
		methods: {
			click: function(view) {
				this.button.onclick = function(){
					alert('help');
				}
			},
		},
	};
</script>

<style scope>
	.register {
		margin-top: 100px;
	}
	.input_group label {
		display: inline-block;
	}
	.input_group input {
		display: block;
	}
	.component-fade-enter-active, .component-fade-leave-active {
		transition: opacity .3s ease;
	}
	.component-fade-enter, .component-fade-leave-to{
		opacity: 0;
	}
</style>