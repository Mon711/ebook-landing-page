<script>
	import { goto } from "$app/navigation";


	let { children, ...props } = $props();

	async function onclick() {
		try {
			const response = await fetch('/api/checkout', {
				method: 'POST',
				headers: {
					'Content-Type': 'application/json'
				}
			});

			if (!response.ok) {
				// Handle error
				console.error('Failed to create checkout session');
				return;
			}

			const { url } = await response.json();
			// Redirect to the Stripe checkout page returned by the API
			window.location.href = url;
		} catch (err) {
			goto("/checkout/failure")
		}
	}
</script>

<button {...props} {onclick}>{@render children()}</button>

<style>
	button {
		background-color: black;
		color: white;
		padding: 20px 24px;
		font-weight: normal;
		font-size: 22px;
		text-transform: uppercase;
		transition: all 0.3s;
		border: 1px solid white;
	}

	button:hover {
		background-color: white;
		color: black;
	}
</style>
