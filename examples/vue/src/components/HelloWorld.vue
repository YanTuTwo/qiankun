<template>
  <div>
    <h1>{{ msg }}</h1>
    <p>
      <i class="el-icon-s-promotion" />
      vue version: {{ vueVersion }}, element-ui version: {{ elementVersion }}
    </p>
  </div>
</template>

<script>
	import ElementUI from 'element-ui';
	import Vue from 'vue';

	export default {
		name: 'HelloWorld',
		props: {
			msg: String,
		},
		data() {
			return {
				vueVersion: Vue.version,
				elementVersion: ElementUI.version,
			};
		},
	};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1 {
    color: #64b587;
	background-image: linear-gradient(#fff,#a3eaff);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    filter: drop-shadow(0 0 .375rem rgba(8,44,68,.5))
  }
</style>
