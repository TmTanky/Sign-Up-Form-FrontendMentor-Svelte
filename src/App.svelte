<script lang="ts">
	import Form from './components/Form/Form.svelte'
</script>

<main>
	<div class="greetings">
		<div class="info">
			<h1>Learn to code by watching others</h1>
			<p>
				See how experience developers solve problems in real-time. Watching
				scripted tutorials is great, but understanding how developers think is
				invaluable.
			</p>
		</div>
	</div>

	<div class="form">
		<Form />
	</div>
</main>

<style lang="scss">
	main {
		min-height: 100vh;
		display: flex;
		background-image: url('./images/bg-intro-desktop.png');
		background-color: hsl(0, 100%, 74%);
	}

	div.greetings {
		flex: 1;
		display: flex;
		justify-content: center;
		flex-direction: column;

		.info {
			margin: 0 10rem;

			h1 {
				color: white;
				font-size: 40px;
			}
			p {
				margin-top: 15px;
				color: white;
			}
		}
	}

	div.form {
		flex: 1;
		/* background-color: hsl(0, 100%, 74%); */
		display: flex;
		justify-content: center;
		flex-direction: column;
		align-items: center;
	}
</style>
