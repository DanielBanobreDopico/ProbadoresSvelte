<script>
	async function getNotifications () {
		const result = await Notification.requestPermission();
		console.log('Notification permission request', result);
		if (result === 'granted') {
			const title = 'First notification'
			const options = {
				body: 'You can get notifications now.',
				icon: 'favicon.svg'
			}
			new Notification(title, options);
		}
	};
</script>

<main>
	<h1>Svelte PWA example</h1>
	<button on:click={getNotifications}>Get notifications</button>
</main>

<style>
</style>