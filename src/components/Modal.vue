<template>
  <ion-content>
    <ion-grid>
        <ion-row>
            <ion-col>
                <p>Modal example</p>
            </ion-col>

            
        </ion-row>

        <ion-row>
            <ion-col>
                <ion-button @click="closeModal()">
                    Close
                </ion-button>
            </ion-col>
        </ion-row>
    </ion-grid>
    
  </ion-content>
</template>

<script>
    export default {
    name: "modal",
    methods: {
        closeModal: async function() {
            this.$ionic.modalController.dismiss();
        }
    }
    };
</script> 