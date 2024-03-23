<template>
  <div class="flex justify-center items-center h-screen">
    <form class='w-full max-w-lg p-5 mx-auto bg-white rounded-lg shadow-xl'>

      <h2 class="text-base font-semibold leading-7 text-gray-900">New Email</h2>

      <div class="relative mt-6">
        <input type="text" id="email" name="sender" class="w-full border border-gray-300 rounded-md py-2 ps-6 outline-none border-none border-b" placeholder=" ">
        <label for="email" class="absolute top-0 left-0 py-2 transition-all duration-300 origin-0 text-gray-500 text-sm">To: </label>
      </div>

      <div class="relative mt-3">
        <input type="text" id="email" name="receive" class="w-full border border-gray-300 rounded-md py-2 ps-14 outline-none border-none border-b" placeholder=" ">
        <label for="email" class="absolute top-0 left-0 py-2 transition-all duration-300 origin-0 text-gray-500 text-sm">Subject: </label>
      </div>
      
      <div class="mt-4">
          <TiptapEditor />
      </div>

      <button type="submit" class="mt-6 rounded-md text-white bg-sable px-3 py-2 w-full"> Send Email</button>
    </form>
  </div>
</template>

<style>
  .bg-sable {
    background-color: #F26634;
  }

  .border-b {
    border-bottom: 1px solid #e5e7eb;
    border-radius: 0;
  }
</style>

<script>
  import TiptapEditor from "~/components/TiptapEditor.vue";
  
  export default {
    name: 'App',
    components: {
      TiptapEditor
    }
  }
</script>