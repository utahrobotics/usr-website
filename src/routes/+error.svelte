<script>
	import { browser } from '$app/environment';
	import { page } from '$app/stores';

	if (browser) {
		console.log($page.status);
	}
</script>

<title>Utah Student Robotics</title>

<h1>{$page.error?.message ?? ''}</h1>

<style>
	h1 {
		align-self: center;
		margin-top: min(4rem, 7.2vw);
		font-size: min(6rem, 10.8vw);
	}
	h1 + h1 {
		margin-top: 0px;
	}
</style>
