<script>
    import Main from './+layout.svelte';
	import Header from './components/Header.svelte'
	export let name;
    
    
</script>


    <main>
		<Header/>
	<Main>
        <h1>Hello There, I'm Sanjana</h1>
		
    </Main>
	</main>
     


<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 1200px;
		background-color: rgb(17, 32, 55);
		
	}

	h1 {
		color: #ffffff;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		z-index: 1;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	
</style>