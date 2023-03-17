<script>
    import { onMount } from "svelte";
    import { abi, address } from "../contract-info";
    import { ethers } from "ethers";
    // import detectEthereumProvider from "@metamask/detect-provider";

    // This function detects most providers injected at window.ethereum
    export let provider;

    let accounts = [];
    let ourContract;

    onMount(async () => {
        // window.web3

        if (typeof window.ethereum !== "undefined") {
            // This function detects most providers injected at window.ethereum

            console.log("MetaMask is installed!");

            accounts = await ethereum.request({
                method: "eth_requestAccounts",
            });

            ourContract = await new ethers.Contract(address, abi, provider);

            console.log(ourContract);
            // const name = await ourContract.functions.getName();

            console.log(ourContract.getFunction("getName"))

            const experiment = (await ourContract.getFunction("getName"))

            console.log(experiment);
        }
    });
</script>

hallo

{#if accounts.length > 0}
    {accounts[0]}

    <p><br /></p>

    The smart contract address is: {address}

    <p><br></p>
    The smart contract abi is: {JSON.stringify( abi)}
{/if}
