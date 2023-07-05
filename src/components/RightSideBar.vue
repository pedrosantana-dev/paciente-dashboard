<template>
	<q-drawer show-if-above side="right" bordered :width="300">
		<q-toolbar class="q-mt-lg">
			<q-space></q-space>
			<q-btn round icon="notifications">
				<q-badge floating rounded color="green" />
			</q-btn>
		</q-toolbar>
		<div class="flex flex-center column">
			<q-avatar size="100px">
				<img src="https://cdn.quasar.dev/img/avatar6.jpg" />
			</q-avatar>
			<q-item-label caption class="q-my-md"> Suas Atividades Hoje </q-item-label>
			<div class="text-h5"><strong>86%</strong></div>
		</div>
		<q-card flat class="q-mx-md" bordered>
			<q-toolbar class="">
				<div class="text-overline">Todas as atividades</div>
				<q-space></q-space>
				<q-btn round icon="fas fa-chevron-right" size="10px" color="green"></q-btn>
			</q-toolbar>
		</q-card>
		<q-card class="q-mx-md q-mt-lg" bordered>
			<q-toolbar>
				<div class="text-overline text-weight-bold">Chat Suporte</div>
				<q-space></q-space>
				<q-avatar size="25px">
					<img src="https://cdn.quasar.dev/img/avatar1.jpg" />
				</q-avatar>
				<div class="text-overline q-ml-sm">Joana</div>
			</q-toolbar>
			<q-separator />
			<div class="q-pa-md row justify-center">
				<div style="width: 100%; max-width: 400px">
					<q-chat-message
						name="eu"
						avatar="https://cdn.quasar.dev/img/avatar4.jpg"
						:text="['Olá, como você está?']"
						sent
						stamp="7 minutos atrás"
					/>
					<q-chat-message
						name="Jane"
						avatar="https://cdn.quasar.dev/img/avatar2.jpg"
						:text="['Bem, e você como está?']"
						stamp="4 minutos atrás"
					/>
				</div>
			</div>
			<q-input bottom-slots v-model="text" label="Sua mensagem..." class="q-mx-sm">
				<template v-slot:after>
					<q-btn round dense flat icon="fas fa-paper-plane" color="green" size="10px" class="q-mt-md" />
				</template>
			</q-input>
		</q-card>
	</q-drawer>
</template>

<script>
	export default {};
</script>

<style></style>
