<script lang="ts">
	import Info from './components/Info/Info.svelte'
	import Form from './components/Form/Form.svelte'
	import NoticeBar from './components/NoticeBar/NoticeBar.svelte'
</script>

<main>
	<div class="greetings">
		<Info />
	</div>

	<div class="form">
		<NoticeBar />
		<Form />
	</div>
</main>

<style lang="scss">
	main {
		min-height: 100vh;
		display: flex;
		background-image: url('./images/bg-intro-desktop.png');
		background-color: hsl(0, 100%, 74%);
		width: 100%;

		@media screen and (min-width: 300px) and (max-width: 849px) {
			flex-direction: column;
		}
	}

	div.greetings {
		flex: 1;
		display: flex;
	}

	div.form {
		flex: 1;
		display: flex;
		justify-content: center;
		flex-direction: column;
		align-items: center;

		@media screen and (min-width: 300px) and (max-width: 499px) {
			margin: 0 1rem;
			padding: 2rem 0;
		}

		@media screen and (min-width: 500px) and (max-width: 849px) {
			padding: 5rem 0;
		}
	}
</style>
