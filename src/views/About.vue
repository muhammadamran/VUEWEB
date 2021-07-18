<template>
  <div class="about">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="About"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/Header.vue'

export default {
  name: 'About',
  components: {
    HelloWorld
  }
}
</script>
