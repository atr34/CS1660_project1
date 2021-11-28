<template>
  <div class="home">
    <HelloWorld msg="Welcome to the Big Data Process Application" />  
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>
