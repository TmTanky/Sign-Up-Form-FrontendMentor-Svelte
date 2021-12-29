<form action="">
	<input type="text" placeholder="First Name" name="firstName" />
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
		min-width: 400px;
		padding: 1.5rem;
		border-radius: 10px;
		box-shadow: 0px 8px 0px 0px rgba(0, 0, 0, 0.493);

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
		}

		p {
			font-size: 10px;
			text-align: center;
			margin-top: 10px;

			span {
				color: hsl(0, 100%, 74%);
				font-weight: bold;
			}
		}
	}
</style>