<script lang="ts">
	import '@capacitor/core';
	export let name: string;
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
        height: 100%;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

    section {
        background-color: aqua;
		height: 100%;
    }
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
<main>
	<header>
        <h1>Hello {name}!</h1>
        <h1>V2</h1>
    </header>
    <section>
        <slot></slot>
    </section>
	
</main>
