<main class="scroll">
	<div class="content">
		<slot />
	</div>
</main>

<style lang="scss">
	@import 'https://cdn.jsdelivr.net/gh/verdulife/utility-classes/dist/reset.css';
	@import 'https://cdn.jsdelivr.net/gh/verdulife/utility-classes/dist/utility-classes.css';
	@import url('https://fonts.googleapis.com/css2?family=Courier+Prime&display=swap');
	@import url('/fonts/vintage-ink.css');

	:root {
		--font-title: 'VintageInk';
		--font-text: 'Courier Prime';

		--color-pri: #002c91;
	}

	.scroll {
		background: url('/background.png') no-repeat center;
		background-size: cover;
	}

	.content {
		max-width: 600px;
		margin: 0 auto;
	}
</style>
