<template>
	<div id="info" class="flex-row bordered">
		<div>
			Wall: <a :href="'https://wavesexplorer.com/address/' + $parent.wall">{{ $parent.wall }}</a>
		</div>
		<div>
			Fee: {{ fee }} WAVES
		</div>
		<div>
			<a href="https://github.com/bodrych/waves-wall">GitHub</a>
		</div>
		<div>
			Waves Keeper:
			<a href="https://addons.mozilla.org/ru/firefox/addon/waves-keeper">Firefox,</a>
			<a href="https://chrome.google.com/webstore/detail/waves-keeper/lpilbniiabackdjcionkobglmddfbcjo">Google Chrome</a>
		</div>
		<div>
			<a href="https://forum.wavesplatform.com/t/the-waves-wall/3670">Forum thread</a>
		</div>
	</div>
</template>

<script>
	export default {
		data: () => {
			return {
				fee: '0.001'
			}
		}
	}
</script>

<style scoped>
	#info {
		margin-top: 5px;
		padding: 5px;
		justify-content: space-between;
		flex-wrap: wrap;
	}
</style>