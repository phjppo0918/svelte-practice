<script>
	import { Router, Link, Route } from "svelte-routing";
	import Login from "./Login.svelte";
	import Board from "./Board.svelte";
	import Signup from "./Signup.svelte";

	export let url = "";
</script>

<main>
	<Router {url}>
		<nav>
			<Link to="/login">login</Link>
			<Link to="/board">board</Link>
			<Link to="/signup">signup</Link>
		</nav>
		<div>
			<Route path="/login" component={Login} />
			<Route path="/board" component={Board} />
			<Route path="/signup" component={Signup} />
		</div>
	</Router>
</main>

