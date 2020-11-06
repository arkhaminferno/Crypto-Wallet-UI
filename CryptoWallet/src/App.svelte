<script>
import Navbar from "./components/navbar.svelte"
import BalanceDetail from "./components/balanceDetail.svelte"
import IncomeExpense from "./components/incomeExpense.svelte"
import SendButton from "./components/sendButton.svelte"
import ReceiveButton from "./components/receiveButton.svelte"
import Circle from "./components/circular.svelte"
import CryptoOwned from "./components/cryptoOwned.svelte"
</script>

<div class="parent_div">
	
	<section class="child1">
		<div class="child1_container">
			<div class="navbar"><Navbar/></div>
						<div class="details_parent">
				<div class="detail_child1">
					<div><BalanceDetail/></div>
					<div><IncomeExpense/></div>
					<div class="buttons">
						<div><SendButton/></div>
						<div><ReceiveButton/></div>
					</div>
				</div>
				<div class="detail_child2">
					<Circle/>
				</div>
				<div class="detail_child3"><CryptoOwned/></div>
			</div>
		</div>
	</section>
	<section class="child2">
		<div class="child2_container">
<div class="wallet_detail">1</div>
<div class="transactions_detail">2</div>
		</div>
		
	</section>
</div>

<style>
	:global(*){
		box-sizing: border-box;
	}
	.parent_div{
		display: flex;
		flex-direction: column;
		margin-left: 5%;
		margin-right: 5%;
		border:1px solid black;
		height: 100vh;
	}
	.child1{
		height: 40%;
		display: flex;
		flex-direction: column;
		border: 1px solid green;
	}
	.child2{
		height: 60%;
	}

	.details_parent{
		display: flex;
		justify-content: space-between;
		flex: 1;
	}
	.navbar{
		height: 10%;
	}
	.details_parent{
		height: 90%;
	}
	
.child1_container{
	display: flex;
	flex-direction: column;
	height: 100%;
}
.detail_child1{
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}
.details_parent > div{
	width: 33.3%;
	height: 100%;
}
.detail_child1 > div{
	height:33.3%;
}
.child2_container{
	display: flex;
	flex-direction: column;
}
.child2{
	display: flex;
}
.buttons{
	display: flex;
	justify-content: space-evenly;
}
</style>