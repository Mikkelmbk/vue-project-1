<template>
  <nav class="h-20 bg-teal-500">

      <p>{{ status }}</p>

      <button class="button bg-yellow-500 rounded p-1 mx-2 text-red-500 font-bold border-2 border-black outline-none" v-on:click="changeStatus">Click me</button>

      <input type="text" v-model="username">
      <p> {{ username }}</p>
    
  </nav>
</template>

<script>
export default {
    data: function(){
        return {
            status: "This is a test",
            username: "Mikkel"
        }
    },
    methods: {
        changeStatus(){
            this.status = "This is still a test buddy"
        }
    }
}
</script>