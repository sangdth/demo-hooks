<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Vue.js Finland"/>
    <HelloKitty msg="Meow meow" />
  </div>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator';

import HelloWorld from '@/components/HelloWorld.vue'; // @ is alias to /src
import HelloKitty from '@/components/HelloKitty.vue';

@Component({
  name: 'Home',
  components: {
    HelloWorld,
    HelloKitty,
  },
})

export default class Home extends Vue {
  created() {
    console.log('Home created');
  }

  mounted() {
    console.log('Home mounted');
  }
}
</script>
