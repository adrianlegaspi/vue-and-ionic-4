<template>
  <ion-app>
      <ion-header>
        <ion-toolbar color="primary">
          <ion-title>Vue and Ionic 4 example</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-header>
          <ion-grid>
            <ion-row>
              <ion-col class="ion-text-center"><router-link to="/">Home</router-link></ion-col>
              <ion-col class="ion-text-center"><router-link to="/about">About</router-link> </ion-col>
            </ion-row>
          </ion-grid> 
      </ion-header>

      <ion-content>
        <ion-vue-router />
      </ion-content>
        
  </ion-app>
</template>

<style lang="scss">
</style>
