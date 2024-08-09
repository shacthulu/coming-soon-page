<script>
	let email = '';

	function handleSubmit() {
		console.log('Email submitted:', email);
		email = '';
	}
</script>

<div class="background">
	<div class="overlay">
		<div class="content">
			<h1>Something Exciting is Coming</h1>
			<p class="description">We're working hard to bring you something amazing. Stay tuned for updates!</p>
			<!-- <div class="form-container">
				<form on:submit|preventDefault={handleSubmit} class="form">
					<input bind:value={email} placeholder="Enter your email" type="email" required />
					<button type="submit">Notify Me</button>
				</form>
				<p class="disclaimer">We'll never share your email. Promise.</p>
			</div> -->
		</div>
	</div>
</div>

<style>
	:global(body) {
		font-family: 'Inter', sans-serif;
		margin: 0;
		padding: 0;
	}

	.background {
		background-image: url('/background.png');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		min-height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.overlay {
		background-color: rgba(0, 0, 0, 0.5);
		width: 100%;
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 2rem;
	}

	.content {
		max-width: 60rem;
		text-align: center;
		color: white;
	}

	h1 {
		font-family: 'Inter', sans-serif;
		font-size: 2.5rem;
		font-weight: 700;
		margin-bottom: 8;
	}

	.description {
		font-size: 1rem;
		margin-bottom: 1.5rem;
		font-weight: 400;
	}

	.form {
		display: flex;
		gap: 0.5rem;
	}

	input,
	button {
		height: 2.5rem;
		font-size: 0.875rem;
		font-family: 'Inter', sans-serif;
	}

	input {
		flex: 1;
		padding: 0 0.75rem;
		border: none;
		border-radius: 4px;
		font-weight: 400;
	}

	button {
		padding: 0 1rem;
		background-color: rgba(255, 255, 255, 0.9);
		color: #000;
		border: none;
		border-radius: 4px;
		cursor: pointer;
		font-weight: 500;
		transition: all 0.3s ease;
	}

	button:hover {
		background-color: #fff;
		box-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
	}

	.disclaimer {
		margin-top: 0.5rem;
		font-size: 0.75rem;
		opacity: 0.8;
		font-weight: 400;
	}
</style>
