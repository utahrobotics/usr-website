<script>
	import background from '$lib/assets/snowy-mountains.jpg';
	import amee from '$lib/assets/amee.png';
	import bukavac from '$lib/assets/bukavac.png';
	import sandcrawler from '$lib/assets/sandcrawler.png';
	import masterChief from '$lib/assets/master chief.png';
</script>

<title>Utah Student Robotics</title>
<header>
	<img src={background} id="background" alt="Background" />
	<h1>Utah Student</h1>
	<h1>Robotics</h1>
</header>
<main>
	<h2>Who We Are</h2>
	<p>
		We are the University of Utah's own robotics team. The team began as a couple of students in the
		mining department wanting to compete in NASA's annual Robotic Mining Competition and has since
		flourished into the multi-disciplinary club that it is today, combining electrical, mechanical,
		computer, and mining expertise.
	</p>
	<h2>Our Robots</h2>
	<div class="images">
		<img src={bukavac} alt="Bukavac" />
		<img src={amee} alt="AMEE" />
	</div>
	<div class="images">
		<img src={sandcrawler} alt="SandCrawler" />
		<img src={masterChief} alt="MasterChief" />
	</div>
	<h2>What We Do</h2>
	<p>
		Every year the team works hard to build a robot for NASA's Lunabotics Competition (formerly
		called The Robotic Mining Competition). We design a robot from the ground up taking into
		consideration power, autonomy, mechanical loads, and lots more. At the end of the year we go to
		Florida to compete against 50 other universities. The club offers students an opportunity to
		learn new aspects of engineering and to apply what they've learned in classes.
	</p>
</main>

<style>
	h1 {
		align-self: center;
		margin-top: min(4rem, 7.2vw);
		font-size: min(6rem, 10.8vw);
		color: whitesmoke;
	}
	h1 + h1 {
		margin-top: 0px;
	}
	#background {
		position: absolute;
		z-index: -1;
		width: 100vw;
		filter: brightness(50%);
		object-fit: cover;
		height: min(24rem, 43.2vw);
		object-position: center -min(10rem, 18vw);
	}
	header {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	main {
		position: absolute;
		margin-top: min(24rem, 43.2vw);
		display: flex;
		flex-direction: column;
		align-items: center;
		width: calc(50vw - 1rem);
		padding-left: 1rem;
		padding-right: 1rem;
		padding-bottom: 7rem;
		align-self: center;
	}
	h2 {
		margin-top: min(1.5rem, 2.7vw);
		font-size: min(2rem, 6vw);
	}
	p {
		padding-top: min(1rem, 1.8vw);
		font-size: min(1.25rem, 3.6vw);
	}
	.images {
		display: flex;
		flex-direction: row;
		align-items: center;
		background-color: hsl(0, 0%, 93%);
		border-radius: min(1rem, 1.8vw);
		border: 2px solid gray;
	}
	.images img {
		width: 50%;
		height: fit-content;
	}
	.images img:last-child {
		border-left: 2px dashed gray;
	}
	.images + .images {
		margin-top: min(1.5rem, 2.7vw);
	}
</style>
