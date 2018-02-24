<template>
  <ion-app>
    <ion-page class="show-page">
      <ion-header>
        <ion-toolbar>
          <ion-title>Ionic 4 + Vue Application </ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content class="content" padding>
          <ion-list>
            <ion-item v-for="item of items" v-bind:key="item.id">
              <ion-label full>{{item.name}}</ion-label>
            </ion-item>
          </ion-list>
           <ion-button @click="goToPage2" full>Go To Page II</ion-button>
      </ion-content>
    </ion-page>
  </ion-app>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      items: [{id: 0, name:'Ahmed'},{id:1, name: 'Naima'}]
    }
  },  
  methods: {
    goToPage2 () {
      this.$router.push('page2')
    }
  }  
}
</script>

<style>

</style>


