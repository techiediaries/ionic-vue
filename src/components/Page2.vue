<template>
  <ion-app>
    <ion-page class="show-page">
      <ion-header>
        <ion-toolbar>
          <ion-title>Ionic 4 + Vue Application </ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content class="content" padding>
        This is page 2
        
        <ion-button @click="goToHome" full>Go Home</ion-button>

      </ion-content>
    </ion-page>
  </ion-app>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
    }
  },  
  methods: {
      goToHome(){
          this.$router.push('/')
      }
  }  
}
</script>

<style>

</style>


