<script>
  import OurMapArea from "@/components/OurMapArea.svelte";
  import MetamaskIntegration from "@/components/MetamaskIntegration.svelte";

  export let name;

  let ourList = ["apple", "banana", "orange"]

  let flag = true

</script>

<h1>Hello {name}!</h1>
<p>
  Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how
  to build Svelte apps.
</p>

{#if flag}
  

{#each ourList as fruit }

<br>  
super leckere frucht: {fruit}
{/each}

{/if}

<OurMapArea />
<MetamaskIntegration />

<link
  href="https://fonts.googleapis.com/css?family=Overpass:100,400"
  rel="stylesheet"
/>

<style>
  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }
</style>
