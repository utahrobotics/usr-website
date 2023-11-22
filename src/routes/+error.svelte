<script>
	import { browser } from '$app/environment';
	import { goto } from '$app/navigation';
	import { page } from '$app/stores';

	if (browser) {
		console.log($page.status);
		goto('/');
	}
</script>

<title>Utah Student Robotics</title>

<noscript>
	<h1>{$page.error?.message ?? ''}</h1>

	<style>
		h1 {
			align-self: center;
			margin-top: min(4rem, 7.2vw);
			font-size: min(6rem, 10.8vw);
		}
	</style>
</noscript>
