<template>
	<div class="relative h-10 m-1">
		<div class="grid grid-cols-9"
			style="border-top: 1px solid #e6e6e6;">
			<input type="text"
				v-model="message"
				@keyup.enter="sendMessage()"
				placeholder="Yeni mesaj"
				class="col-span-8 outline-none p-1 rounded" />
			<button @click="sendMessage()"
				class="col-span-1 bg-gray-500 hover:bg-blue-700 p-2 rounded text-white">
				Yolla
			</button>
		</div>
	</div>
</template>

<script>
	export default{
		props:['room'],
		data:function(){
			return {
				message:''
			}
		},
		methods:{
			sendMessage(){
				if(this.message == ' '){
					return;
				}

				axios.post('/chat/room/'+this.room.id+'/message',{
					message:this.message
				})
				.then(response=>{
					if(response.status == 201){
						this.message = '';
						this.$emit('messageSent');
					}
				})
				.catch(error=>{
					console.log(error);
				})
			}
		}
	}
</script>
