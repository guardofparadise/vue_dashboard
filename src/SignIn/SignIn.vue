<template>
	<div class="container">
	<div class="request">
	Don't have a Design+Code HQ account?
		<router-link class="request-a" to="/request">
			Request an account
		</router-link>
	</div>
		<div class="login">
			<img src="@/assets/DCHQ.svg" alt="alt">
			<h4>Sign into Design+Code HQ</h4>
			<input type="text" placeholder="E-mail">
			<input type="password" placeholder="Password">
			<button>Sign In</button>
			<router-link class="recover-a" to="/recover">Forgot your password?</router-link>
		</div>
	</div>
</template>

<script>
	export default {
		name: "SignIn"
	}	
</script>

<style scoped land="scss">
	.container {
		display: flex;
		justify-content: center;
		align-items: center;
		min-height: 100vh;
	}

	.login {
		width: 400px;
	}

	.request {
		position: absolute;
		top: 40px;
		right: 40px;
		color: rgba(255,255,255,.3);
	}

	.request-a {
		color: #fff;
		text-decoration: none;
	}

	h4 {
		line-height: 34px;
		font-size: 24px;
		text-align: center;
		color: #fff;
	}

	input {
		background: rgba(255,255,255,.2);
		border: 1px solid rgba(255,255,255,.2);
		box-sizing: border-box;
		border-radius: 4px;
		height: 60px;
		width: 100%;
		font-size: 20px;
		color: white;
		padding-left: 20px;
		margin-top: 20px;
	}

	button {
		background: #56ccf2;
		box-shadow: 0px 0px 20px rgba(0,0,0,.2);
		border-radius: 4px;
		border: none;

		height: 60px;
		width: 100%;
		font-size: 20px;
		color: #fff;
		margin-top: 20px;
		margin-bottom: 40px;
	}

	.recover-a {
		text-decoration: none;
		color: rgba(255,255,255,.2);
		
	}
</style>