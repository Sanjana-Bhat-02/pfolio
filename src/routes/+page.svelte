<script>
	import Main from "./+layout.svelte";
</script>

<Main />


<style>
	h1 {
		color: #ffffff;
		text-transform: uppercase;
		font-size: 300%;
		font-weight: 100;
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		z-index: 8;
	}

	@keyframes fadeIn {
		from {
			opacity: 0;
		}
		to {
			opacity: 1;
		}
	}
</style>
