
<script>
    import Ownedcrypto from "../dummydata/cryptoOwned.js";
</script>

{#each Ownedcrypto as crypto (crypto.id)}
<table>
    <tr>
        <td>{crypto.logo}</td>
        <td>
            <div class="crypto_name">
<div>{crypto.alias}</div>
<div>{crypto.name}</div>
            </div>
        </td>
        <td>
            <div class="crypto_profit">
<div>{crypto.percentage}</div>
<div>{crypto.profit}</div>
            </div>
        </td>
    </tr>
</table>
{/each}


<style>
    .crypto_name{
        display: flex;
        flex-direction: column;
    }
    .crypto_profit{
        display: flex;
        flex-direction: column;
    }
</style>