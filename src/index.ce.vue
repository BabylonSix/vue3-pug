<template lang="pug">
div
	button(@click="this.dec") -
	span {{ count }}
	button(@click="this.inc") +
</template>

<script>
	export default {
		tag: 'my-counter',
		name: 'MyCounter',
		data() {
			return { count: 0 }
		},
		methods: {
			inc: function() {
				this.count++;
			},
			dec: function() {
				this.count--;
			}
		}
	};
</script>

<style scoped>
	span,
	button {
		font-size: 200%;
	}

	span {
		width: 4rem;
		display: inline-block;
		text-align: center;
	}

	button {
		width: 4rem;
		height: 4rem;
		border: none;
		border-radius: 10px;
		background-color: seagreen;
		color: white;
	}
</style>