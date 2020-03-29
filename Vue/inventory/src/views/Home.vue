<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar>
        <ion-title size="large" text-center>Inventory Check-in</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <inventoryEntry v-on:get-codes="getInventory" />
    </ion-content>
  </div>
</template>

<script>
  import inventoryEntry from "../components/inventoryEntry";
  export default {
    name: "Home",
    components: { inventoryEntry },
    methods: {
      getInventory(inv) {
        console.log(inv);
      }
    }
  };
</script>
