<script>
	import logo from '$lib/assets/favicon.png';
	import simon from '$lib/assets/simon-gross.webp';
</script>

<svelte:head>
	<title>Simon Müller</title>
	<html lang="en" />
</svelte:head>

<div class="main">
	<h1>Hey, I'm Simon</h1>
	<div class="card">
		<div class="image">
			<img class="simon" alt="Portrait of Simon Müller" src={simon} />
		</div>
		<div class="text">
			<p>This site is under heavy development.</p>
			<p>For now, just get in touch:</p>
		</div>
		<div class="links">
			<a class="mail" href="mailto:hey@seimon.ch">
				<img alt="Mail Logo" src={logo} />
			</a>
			<a class="linkedin" href="https://www.linkedin.com/in/seimon-m">
				<img alt="Linkedin Logo" src={logo} />
			</a>
		</div>
	</div>
</div>

<style>
	.main {
		height: 100vh;
		width: 100vw;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	h1 {
		position: absolute;
	}

	.card {
		/* From https://css.glass */
		background: rgba(255, 255, 255, 0.2);
		border-radius: 16px;
		box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
		backdrop-filter: blur(5px);
		-webkit-backdrop-filter: blur(5px);
		border: 1px solid rgba(255, 255, 255, 0.3);
		/* width: 80vw; */
		/* height: 100vh; */
		margin: 20px;
		padding: 10px;
	}

	.image {
		margin: 30px;
	}

	.links {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		margin: 20px;
	}

	.links > a {
		margin: 0px 30px;
	}

	.links > a > img {
		width: 40px;
		height: 40px;
	}

	.simon {
		max-width: 80vw;
		max-height: 55vh;
		border-radius: 16px;
	}
</style>
