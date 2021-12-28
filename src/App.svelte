<script lang="ts">
</script>

<main>
	<div class="greetings">
		<h1>Learn to code by watching others</h1>
		<p>
			See how experience developers solve problems in real-time. Watching
			scripted tutorials is great, but understanding how developers think is
			invaluable
		</p>
	</div>

	<div class="form">
		<form action="">
			<input type="text" placeholder="First Name" name="firstName" />
			<input type="text" placeholder="Last Name" name="lastName" />
			<input type="email" placeholder="Email Address" name="email" />
			<input type="password" placeholder="Password" name="password" />
      <button> Claim your free trial </button>
		</form>
	</div>
</main>

<style>
	* {
		box-sizing: border-box;
		margin: 0;
		padding: 0;
	}

	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
			Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	}

  input {
    padding: 0.8rem 1rem;
    margin: 10px 0;
    border-radius: 5px;
    border: solid 1px rgb(196, 194, 194);
    outline: none;
  }

  button {
    padding: 0.8rem 1rem;
    background-color: lightgreen;
    color: white;
    text-transform: uppercase;
    border: none;
    outline: none;
    border-radius: 5px;
    margin-top: 10px;
  }

	main {
		min-height: 100vh;
		background-color: red;
		display: flex;
	}

	div.greetings {
		flex: 1;
		display: flex;
		justify-content: center;
		flex-direction: column;
	}

	div.form {
		flex: 1;
		background-color: blue;
		display: flex;
		justify-content: center;
		flex-direction: column;
    align-items: center;
	}

	form {
		background-color: yellow;
		display: flex;
		flex-direction: column;
    width: 400px;
    padding: 1.5rem;
    border-radius: 10px;
	}
</style>
