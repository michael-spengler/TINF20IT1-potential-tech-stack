<script>
    import { onMount } from "svelte";
    // import { ethers } from "https://cdn.skypack.dev/ethers";
    // import { ethers } from "npm:ethers";
    // import { smartContractABI } from "../../abi.ts";

    // export let provider;

    let account;
    let smartContractRepresentation;

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

        // https://goerli.etherscan.io/address/0x86bb1f3b75b013a1bdd31efb20de79e20b137036
        // smartContractRepresentation = await new ethers.Contract(
        //         "0x86bb1f3b75b013a1bdd31efb20de79e20b137036",
        //         smartContractABI,
        //         provider
        //     );

        //     console.log("we are here")
        //     console.log(smartContractRepresentation);
            // const name = await smartContractRepresentation.getName();
            // nftUnderManagement.highestOffer =
            //     await erc721Contract.getHighestOffer();


    });

    function callSmartContractFunction() {
        alert("calling Smart ContractFunction");
    }
</script>

<p><br></p>
<h2>Blockchain Interaction Demo</h2>
{#if account !== undefined}
    you are connected with wallet:
    <h4>{account}</h4>
{/if}


<button on:click={callSmartContractFunction}>
	Call Smart Contract Function
</button>