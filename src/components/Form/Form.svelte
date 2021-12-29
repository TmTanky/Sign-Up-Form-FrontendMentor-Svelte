<script lang="ts">
import { prevent_default } from "svelte/internal"

	let firstName = ''
	let lastName = ''
	let emailAdd = ''
	let password = ''

	const subtmitForm = () => {
		console.log(firstName)
	}
</script>

<form on:submit|preventDefault={subtmitForm}>
	<input type="text" bind:value={firstName} placeholder="First Name" name="firstName" />
	<input type="text" placeholder="Last Name" name="lastName" />
	<input type="email" placeholder="Email Address" name="email" />
	<input type="password" placeholder="Password" name="password" />
	<button> Claim your free trial </button>
	<p>
		By clicking the button, you are agreeing to our <span>
			Terms and Services
		</span>
	</p>
</form>

<style lang="scss">
	form {
		background-color: white;
		display: flex;
		flex-direction: column;
		min-width: 450px;
		padding: 2rem;
		border-radius: 10px;
		box-shadow: 0px 8px 0px 0px rgba(0, 0, 0, 0.2);
		input {
			padding: 0.8rem 1rem;
			margin: 10px 0;
			border-radius: 5px;
			border: solid 1px rgb(196, 194, 194);
			outline: none;

			&::placeholder {
				font-weight: bold;
				font-size: 12px;
			}

			&:focus {
				border: solid 1px hsl(248, 32%, 49%);
			}
		}

		button {
			padding: 0.8rem 1rem;
			background-color: hsl(154, 59%, 51%);
			color: white;
			text-transform: uppercase;
			border: none;
			outline: none;
			border-radius: 5px;
			margin-top: 10px;
			font-weight: 600;
			cursor: pointer;
			&:hover {
				background-color: hsl(154, 57%, 40%);
			}
		}

		p {
			font-size: 10px;
			text-align: center;
			margin-top: 10px;
			color: hsl(246, 25%, 77%);

			span {
				color: hsl(0, 100%, 74%);
				font-weight: bold;
				cursor: pointer;
			}
		}
	}
</style>
