<template>
  <ion-content>
    <ion-button @click="showModal()">Open modal</ion-button>
  </ion-content>
</template>

<script>
import Modal from "@/components/Modal.vue";
export default {
  name: "home",
  methods: {
    showModal: async function() {
      const modal = await this.$ionic.modalController.create({
        component: Modal,
        componentProps: {
          propsData: {
            userData: Math.round(Math.random() * 100)
          }
        }
      });
      await modal.present();
    }
  }
};
</script>