<script >
    import '../lib/blockrain/blockrain.css'
     const blockrain = () => import('$lib/blockrain/blockrain.jquery.min.js')
 
    const click = async () => {
        await blockrain();
        window.$('.game').blockrain()
    }
</script>

<div class="game" style="width:250px; height:500px; border: 1px solid red;"></div>
<button on:click={click}>Play</button>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
