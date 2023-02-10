<script>
    import { onMount } from "svelte";

    let account;
    onMount(async () => {
        if (typeof window.ethereum === "undefined") {
            alert(
                "this is a decentralized app --> please install metamask or use brave.com to interact with the blockchain"
            );
        } else {
            alert("Your browserwallet is ready!");
        }

        const accounts = await ethereum.request({
            method: "eth_requestAccounts",
        });
        account = accounts[0];
    });

    function signData() {
        alert("signing transaction");
    }
</script>

{#if account !== undefined}
    you are connected with wallet:
    <h4>{account}</h4>
{/if}

<button on:click={signData} />
