<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" @click="showMessage()"> {{message}}
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Provide } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  }
})
export default class Home extends Vue {
  // data
  private message: string = 'message'

  // methods
  private showMessage(): void {
    alert(this.message)
  }
}
</script>
