<template>
  <div class="container bg-gray-800 h-screen">
    <!-- 2 divs with w-1/2 and on large screens it will be w-1/5 and w-4/5  -->
    <div class="flex">
      <div class="w-1/2 lg:w-1/5 p-2">
        <div class="bg-gray-600 rounded h-32 w-full"></div>
      </div>
      <div class="w-1/2 lg:w-4/5 p-2">
       <div class="bg-gray-600 rounded h-32 w-full"></div>
      </div>
    </div>
     
  </div>
</template>

<script>
export default {
}
</script>

<style>

</style>