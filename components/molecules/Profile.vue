<template>
	<div class="flex items-center space-x-6">
		<img src="https://github.com/tiagokriok.png" alt="Tiago Carioca (Gripen.Dev)" class="w-20 h-20 rounded-full">
		<div class="flex flex-col w-full">
			<strong class="text-title text-2xl">Tiago Carioca (Gripen.Dev)</strong>
			<p class="flex items-center space-x-2">
				<img src="icons/level.svg" alt="level">
				<span class="text-base">Level {{ level }}</span>
			</p>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import { mapState } from 'vuex';

export default Vue.extend({
	computed: mapState('Challenges', ['level']),
});
</script>
