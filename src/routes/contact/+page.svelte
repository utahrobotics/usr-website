<script>
	import chairs from '$lib/assets/chairs.png';
	import instagram from '$lib/assets/instagram.png';
	import discord from '$lib/assets/discord.png';
	import msteams from '$lib/assets/msteams.png';
</script>

<title>Contact Us | Utah Student Robotics</title>
<header>
	<img src={chairs} id="background" alt="Background" />
	<h1>Contact Us</h1>
</header>
<main>
	<div class="row">
		<h2>We have an</h2>
		<a href="https://www.instagram.com/utahstudentrobotics/"
			><img src={instagram} alt="Instagram" /></a
		>
		<h2>!</h2>
	</div>
	<p>
		We try to post about the events we hold, important meetings, and the general build progress of
		the current robot!
	</p>
	<div class="row">
		<h2>We also use</h2>
		<a href="https://discord.gg/2pZM469cxS"
			><img src={discord} alt="Discord" /></a
		>
	</div>
	<p>
		On Discord we post about announcements about social events and post videos of our robots doing
		stuff! You are free to join the server to keep up to date with what we do.
	</p>
	<div class="row" id="msteamsrow">
		<img src={msteams} alt="Microsoft Teams" />
		<h2>is how we get things done</h2>
	</div>
	<p>
		Most of the formal communication we do within and between sub-teams is done on Microsoft Teams.
		We hold all of our meetings here. If you would like to become a meaningful member of the team,
		the first step would be to join us here. Contact us either in-person, through discord, or
		through our email below!
	</p>
	<div class="row" id="msteamsrow">
		<h2>Lastly, we of course have an email</h2>
	</div>
	<p>
		Please contact us at <a href="mailto:utahstudentrobotics@gmail.com">utahstudentrobotics@gmail.com</a>
		if you are unable to use any of the above options.
	</p>
</main>

<style>
	h1 {
		margin-top: min(14rem, 13vw);
	}
	.row {
		display: flex;
		flex-direction: row;
		margin-top: min(1.5rem, 2.7vw);
		align-items: center;
	}
	.row > h2 {
		margin-top: 0px;
	}
	#background {
		position: absolute;
		z-index: -1;
		width: 100vw;
		filter: brightness(50%);
		object-fit: cover;
		height: min(36rem, 40vw);
		object-position: center -min(10rem, 18vw);
	}
	.row img {
		margin-left: min(1rem, 3vw);
		height: min(6rem, 12vw);
		width: fit-content;
	}
	#msteamsrow img {
		margin-left: 0px;
		margin-right: min(1rem, 3vw);
	}
	main {
		margin-top: min(36rem, 40vw);
	}
</style>
