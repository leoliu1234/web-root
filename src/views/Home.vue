<template>
  <div class="home">
    <div class="images">
      <div v-for="(item, index) in data" :key="`images-${index}`" class="img-item" >
        <img :src="item.path"/>
      </div>
    </div>

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

  private data: object[] = [{
    path: '/images/img (1).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (2).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (3).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (4).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (5).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (6).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (7).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (8).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (9).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (10).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (11).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (12).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (13).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (14).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (15).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (16).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (17).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (18).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (19).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (20).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (21).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (22).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (23).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (24).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (25).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (26).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (28).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (29).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (30).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (31).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (32).jpg',
    description: 'this is a image'
  }, {
    path: '/images/img (33).jpg',
    description: 'this is a image'
  }]

  // methods
  private showMessage(): void {
    alert(this.message)
  }
}
</script>

<style lang="stylus" scoped>
.home
  font-size 20px
  font-weight bold
  .images
    display flex
    flex-wrap wrap
    justify-content center
    width 50rem
    margin auto
    .img-item
      flex 0 0 6rem
      margin-bottom 1rem
      img
        width 5rem
        height 5rem
</style>

