<template>
  <!-- <div class="flex justify-start">
    <div class="flex flex-col">
      {{ message.user.name }}:
      <img
        :src="message.user.profile_photo_url"
        :alt="message.user.name"
        class="rounded-full h-8 w-8 object-cover"
      />
    </div>
    <div class="p-3 rounded-2xl bg-blue-400 text-white font-bold rounded-bl-none">{{ message.message }}</div>
  </div> -->
  <div class="flex gap-2 items-end mb-1 transition-opacity flex-row">
    <span class="flex flex-col"
      ><small class="text-center">{{message.user.name}}</small
      ><img
        class="h-8 w-8 rounded-full object-cover"
        :src="message.user.profile_photo_url"
        :alt="message.user.name" /></span
    ><span
      class="p-2 rounded-2xl bg-blue-400 text-white font-bold rounded-bl-none"
      >{{message.message}}</span
    >
  </div>
</template>

<script>
export default {
  props: ["message"],
};
</script>