<template>
	<q-layout view="lHh Lpr lFf">
		<SideBar />
		<RightSideBar />
		<q-page-container>
			<router-view />
		</q-page-container>
	</q-layout>
</template>

<script>
	import { ref } from "vue";
	import SideBar from "./components/SideBar.vue";
	import RightSideBar from "./components/RightSideBar.vue";

	export default {
		name: "LayoutDefault",

		components: {
			SideBar,
			RightSideBar,
		},

		setup() {
			return {
				leftDrawerOpen: ref(false),
			};
		},
	};
</script>
