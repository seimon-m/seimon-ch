<script>
	import logo from '$lib/assets/favicon.png';
	import simon from '$lib/assets/simon-gross.webp';
</script>

<svelte:head>
	<title>Simon Müller</title>
	<html lang="en" />
</svelte:head>

<div class="main">
	<div class="text">
		<h1>Hey, I'm Simon</h1>
		<p>I'm currently working on a new portfolio website.</p>
		<a href="mailto:hey@seimon.ch">Get in touch</a>
	</div>

	<div class="image">
		<img class="simon" alt="Portrait of Simon Müller" src={simon} />
	</div>
	<div class="links">
		<a class="mail" href="mailto:hey@seimon.ch">
			<img alt="The project logo" src={logo} />
		</a>
		<a class="linkedin" href="https://www.linkedin.com/in/seimon-m">
			<img alt="The project logo" src={logo} />
		</a>
		<a class="twitter" href="https://twitter.com/seimon_m">
			<img alt="The project logo" src={logo} />
		</a>
	</div>
</div>

<style>
	.main {
		height: 100vh;
		width: 100vw;
		padding: 20px;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.image {
		margin: 30px;
	}

	.links {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}

	.links > a {
		margin: 30px;
	}

	.links > a > img {
		width: 40px;
		height: 40px;
	}

	.simon {
		max-width: 80vw;
	}
</style>
