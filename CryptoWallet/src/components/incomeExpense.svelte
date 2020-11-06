<div class="incomeExpense_parent">
<div class="incomeExpense_child1">
    <Income/>
</div>
<div class="incomeExpense_child2">
    <Expense/>
</div>
</div>

<style>
    .incomeExpense_parent{
        display: flex;
        justify-content: space-evenly;
    }
</style>

<script>
import Income from "./income.svelte"
import Expense from "./expense.svelte"
</script>