<header>
	<div class="column">
		<div class="logo">
			Elgato Timestamps <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256"
				><rect width="256" height="256" fill="none" /><polygon
					points="136 32 232 128 136 224 136 176 72 176 72 80 136 80 136 32"
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="16"
				/><line
					x1="40"
					y1="176"
					x2="40"
					y2="80"
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="16"
				/></svg
			>
			YouTube Chapters Converter
		</div>
		<nav aria-label="Main navigation">
			<a href="#how-to-use">How To Use</a>
			<a href="https://github.com/StephenGunn/repo" target="_blank" rel="noopener noreferrer"
				>View Source</a
			>
		</nav>
	</div>
</header>

<style>
	header {
		border-bottom: 1px solid var(--border);
		padding: 0.75rem 0;
	}

	header .column {
		display: flex;
		justify-content: space-between;
	}

	.logo {
		display: flex;
		align-items: center;
		font-size: 1rem;
		font-weight: bold;
		color: var(--primary);
		gap: 0.5rem;
	}

	.logo svg {
		width: 1.2rem;
		height: 1.2rem;
		position: relative;
		top: 2px;
		color: var(--accent);
	}

	nav {
		display: flex;
		gap: 1rem;
		align-items: center;
	}

	nav a {
		display: inline-flex;
		align-items: center;
		text-decoration: none;
		color: var(--text);
		background: var(--secondary);
		padding: 0.5rem 1rem;
		font-weight: 500;
		border-radius: 0.24rem;
	}
</style>
