<script>
	// import Card from "./lib/components/card.svelte";
	import Card from "./lib/components/card-proxy.svelte";
	const cardInfos = [
		["#", "/assets/cards/back.png"],
		["/cs/pl/riscv/", "/assets/cards/riscv.png"],
		["/cs/pl/rust/basic/", "/assets/cards/rust.png"],
		["/cs/pl/haskell/", "/assets/cards/haskell.png"],
		["/cs/system/", "/assets/cards/system.png"],
		["/cs/pl/asm/", "/assets/cards/asm.png"],
		["/cs/algorithm/ds/", "/assets/cards/ds.png"],
		["/cs/regex/", "/assets/cards/regex.png"],
		["/cs/unicode/", "/assets/cards/unicode.png"],
		["/cs/tools/", "/assets/cards/tools.png"],
		["/sec/vulns/log4j/", "/assets/cards/log4j.png"],
		["/web/svg/", "/assets/cards/svg.png"],
		["/ctf/qrcode/", "/assets/cards/qrcode.png"],
		["/ctf/blockchain/eth/", "/assets/cards/eth.png"],
		["/ctf/escapes/pysandbox/", "/assets/cards/pyjail.png"],
		["/writeups/", "/assets/cards/writeups.png"],
		["#", "/assets/cards/donate.png"],
	]
	const len = cardInfos.length;
	const randomIdx = Math.floor(Math.random() * len);
	const pageURL = cardInfos[randomIdx][0];
	const imgURL = cardInfos[randomIdx][1];
</script>

<main>
	<div class="showcase">
		<Card
			id="swsh12pt5-160"
			name="Pikachu"
			types="Lightning"
			supertype="Pokémon"
			subtypes="Basic"
			rarity="Rare Secret"
			showcase={true}
			pageURL={pageURL}
			img={imgURL}
		/>
	</div>
</main>
