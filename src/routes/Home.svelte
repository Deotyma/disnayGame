<script>
    import Typewriter from 'svelte-typewriter';
    import { cascade,loop } from 'svelte-typewriter';
</script>

<!-- <Typewriter> -->
    <h1 use:loop={{ interval: 100 }}>Disney Hangman</h1>
<!-- </Typewriter> -->



<style>  
    h1{
        font-family: "Waltograph";
        font-size: 5rem;
    }
</style>