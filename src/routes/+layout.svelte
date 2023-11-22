<nav>
	<a href="/about">About</a>
	<a href="/sponsors">Sponsors</a>
	<a href="/contact">Contact Us</a>
</nav>
<a href="/" id="home">
	<img src="/favicon.png" alt="Utah Student Robotics Logo" />
</a>
<div id="vspacer" />
<div id="page">
	<slot />
</div>
<style>
	:global(*) {
		margin: 0px;
		padding: 0px;
		font-family: 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans',
			'Helvetica Neue', sans-serif;
	}
	#vspacer {
		height: min(4rem, 13.33vw);
	}
	#page {
		display: flex;
		flex-direction: column;
	}
	nav {
        z-index: 10;
		position: fixed;
		display: flex;
		flex-direction: row;
		justify-content: flex-end;
		background-color: hsl(0, 0%, 93%);
		width: 100vw;
		padding-top: min(1rem, 3.33vw);
		padding-bottom: min(1rem, 3.33vw);
		font-size: min(1.5rem, 5vw);
		gap: min(2.5rem, 6.5vw);
	}
	nav a {
		text-decoration: none;
		color: rgba(0, 0, 0, 0.5);
	}
	nav a:hover {
		text-decoration: none;
		color: rgba(0, 0, 0, 0.8);
	}
	nav a:visited {
		text-decoration: none;
	}
	nav a:last-child {
		margin-right: min(2rem, 3.6vw);
	}
	#home {
        z-index: 11;
		position: fixed;
		background-color: hsl(0, 0%, 93%);
		margin-left: min(2rem, 3.6vw);
		padding: min(0.8rem, 1.44vw);
		border-radius: 7rem;
	}
	#home img {
		width: min(7rem, 17vw);
	}
</style>
