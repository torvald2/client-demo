<template lang="pug">
    b-navbar(toggleable="lg" type="dark" variant="info")
      b-navbar-brand(href="#") NKN Master
      b-navbar-nav.ml-auto
        b-button(squared variant="primary" @click="showAdNodeModal")
          b-icon(icon="tools")
          span.mr-1 
          | Добавить ноду
        b-button(squared variant="success" @click="showSoloNodeModal").ml-2
          b-icon(icon="file-earmark-lock")
          span.mr-1 
          | Создать ноду Solo
        b-button(squared variant="warning" @click="showNpoolNodeModal").ml-2
          b-icon(icon="globe")
          span.mr-1 
          | Coздать ноду nPool
        b-button(squared variant="light" @click="showWalletModal").ml-2
          b-icon(icon="wallet")
          span.mr-1 
          | Wallets
          
        AdNodeModal
        CreateSoloNodeModal
        CreateNpoolNodeModal
        WalletsModal
      
</template>
      
<script>
import AdNodeModal from '@/components/add-node-modal.vue'
import CreateSoloNodeModal from '@/components/create-node-modal.vue'
import CreateNpoolNodeModal from '@/components/create-npool-modal.vue'
import WalletsModal from '@/components/wallets-modal.vue'


export default {
name: 'navBar',
components: {
    AdNodeModal,
    CreateSoloNodeModal,
    CreateNpoolNodeModal,
    WalletsModal
},
methods:{
    showAdNodeModal(){
        this.$bvModal.show("ad-node-modal")
    },
    showSoloNodeModal(){
        this.$bvModal.show("create-solo-node-modal")
    },
    showNpoolNodeModal(){
        this.$bvModal.show("npool-modal")
    },
    showWalletModal(){
        this.$bvModal.show("wallets-modal")
    }
}
}
</script>
      
<style>
      
</style>
      