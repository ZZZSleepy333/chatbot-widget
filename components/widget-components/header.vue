<template>
  <div
    id="chat-header "
    class="w-[400px] h-[96px] flex flex-row mt-4 shadow-SM relative"
  >
    <div class="ml-6 flex flex-row mt-6 items-start gap-2">
      <div id="avatar" class="relative col-span-1 h-fit w-fit flex-initial">
        <img
          src="assets/images/avatar.png"
          placeholder="avatar"
          class="w-12 h-12"
        />
        <div
          class="w-[12px] h-[12px] border-2 border-white rounded-full bg-[#00FF38] absolute bottom-0 right-0"
        ></div>
      </div>
      <div id="status" class="flex-initial w-fit h-fit">
        <h3 class="font-semibold text-[20px] w-fit h-fit">
          FPT Play AI Support
        </h3>
        <span class="text-sm text-gray-500 w-fit h-fit">Đang hoạt động</span>
      </div>
    </div>
    <div id="closeButton" class="cursor-pointer flex-auto">
      <button
        @click="modalStore.closeWidget"
        class="w-6 h-6 top-4 right-4 absolute"
      >
        <i class="fa-solid fa-x"></i>
      </button>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { useModalStore } from "~/stores/modal";

const modalStore = useModalStore();
</script>

<style></style>
