<script>
	import background from '$lib/assets/snowy-mountains.jpg';
</script>

<title>Utah Student Robotics</title>

<img src={background} id="background" alt="Background" />
<h1>Utah Student</h1>
<h1>Robotics</h1>
<main>
	<h2>Who We Are</h2>
	<p>
		We are the University of Utah's own robotics team. The team began as a couple of students in the
		mining department wanting to compete in NASA's annual Robotic Mining Competition and has since
		flourished into the multi-disciplinary club that it is today, combining electrical, mechanical,
		computer, and mining expertise.
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
	main {
		position: absolute;
		margin-top: min(24rem, 43.2vw);
		display: flex;
		flex-direction: column;
		align-items: center;
		width: calc(100vw - 2rem);
		padding-top: min(1.5rem, 2.7vw);
        padding-left: 1rem;
        padding-right: 1rem;
	}
	h2 {
		font-size: min(2rem, 6vw);
	}
    p {
		padding-top: min(1rem, 1.8vw);
		font-size: min(1rem, 3.6vw);
        max-width: 50rem;
    }
</style>
