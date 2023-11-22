<script>
	import teamPhoto from '$lib/assets/team-photo.png';
	import amee from '$lib/assets/amee.png';
	import bukavac from '$lib/assets/bukavac.png';
	import sandcrawler from '$lib/assets/sandcrawler.png';
	import masterChief from '$lib/assets/master chief.png';
</script>

<title>Utah Student Robotics</title>
<header>
	<img src={teamPhoto} id="background" alt="Background" />
	<h1>About</h1>
</header>
<main>
	<h2>We Are Utah Student Robotics</h2>
	<p>
		We are a student-lead and student-organized club, whose goal is to enhance members'
		understanding of robotics and provide practical engineering experience. Each year we compete in
		the NASA Robotic Mining Competition. Our efforts throughout the year culminate into one large
		complex robot. The Robot's sole purpose is off-world mining. A lot of research, design, assembly
		is provided by the team to support that purpose. Each robot we build is unique and thought must
		be put into how it will move, dig, automate, be powered, be shaped, etc.. The club is free to
		join and you may get a chance to come to Florida with select members of the team to represent
		our university in front of NASA scientists and heads of industry.
	</p>
	<h2>Bukavac</h2>
	<img src={bukavac} alt="Bukavac" />
	<p>
		Every year the team works hard to build a robot for NASA's Lunabotics Competition (formerly
		called The Robotic Mining Competition). We design a robot from the ground up taking into
		consideration power, autonomy, mechanical loads, and lots more. At the end of the year we go to
		Florida to compete against 50 other universities. The club offers students an opportunity to
		learn new aspects of engineering and to apply what they've learned in classes.
	</p>
	<h2>AMEE</h2>
	<img src={amee} alt="AMEE" />
	<p>
		AMEE stands for autonomous martian environment excavator. This robot features a front loading
		bucket with a four-wheel skid-steer system and runs on the Nvidia Jetson TX1 computer. At the
		2017 NASA Robotic Mining Competition, this robot collected the most material overall and took
		third place in the competition. This robot also won an innovation award with it's unique
		mechanism to change the center of mass. This is achieved by mounting the whole digging mechanism
		on a linear track and moving it forwards and backwards over the robot's frame. This is necessary
		because the the bucket on the front can be heavy enough to tip the robot forward when fully
		loaded.
	</p>
	<h2>SandCrawler</h2>
	<img src={sandcrawler} alt="SandCrawler" />
	<p>
		The Sandcrawler is called that because it resembles the jawa-piloted sandcrawlers from Tatooine
		in StarWars. It features a bucket ladder digging system, a conveyor belt for storage and
		dumping, and an Nvidia Jetson TX2 for its computer. This robot also claimed third place overall
		and an award for the use of a vibrator to reject dust from the collected material with the aid
		of many holes and slots that allow the dust to pass through.
	</p>
	<h2>Master Chief</h2>
	<img src={masterChief} alt="MasterChief" />
	<p>
		Master chief is a mysterious robot that no one on the current or last team has ever seen. The
		web-dev for the site was never given a description to this elusive specimen. It's believed that
		it haunts the circuitry of the current robots: shorting circuits and messing up tolerances.
		Pretty spooky if you ask me.
	</p>
</main>

<style>
	h1 {
		align-self: center;
		margin-top: min(14rem, 13vw);
		font-size: min(6rem, 10.8vw);
		color: whitesmoke;
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
	header {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	main {
		position: absolute;
		margin-top: min(36rem, 40vw);
		display: flex;
		flex-direction: column;
		align-items: center;
		width: calc(100vw - 2rem);
		padding-left: 1rem;
		padding-right: 1rem;
		padding-bottom: 7rem;
	}
	h2 {
		margin-top: min(1.5rem, 2.7vw);
		font-size: min(2rem, 6vw);
	}
	p {
		padding-top: min(1rem, 1.8vw);
		font-size: min(1.25rem, 3.6vw);
		max-width: 50rem;
	}
	h2 + img {
		width: min(25rem, 50vw);
		height: fit-content;
		background-color: hsl(0, 0%, 93%);
		border-radius: min(1rem, 1.8vw);
		border: 2px solid gray;
	}
</style>
