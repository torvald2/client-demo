<template lang="pug">
  b-modal(id="ad-node-modal" ref="ad-node-modal"  size="lg" title="Добавить существующую ноду")
    b-form-group(description="Только Ipv4 адреса, каждый с новой строки" label="Введите список IP адресов для добавления" :invalid-feedback="invalidFeedback" :state="state")
       b-form-textarea(v-model="ips" rows="10")
    template(#modal-footer="{ ok, cancel, hide }")
      b-button(squared variant="primary")
          b-icon(icon="tools")
          span.mr-1 
          | Добавить ноды
</template>
      
<script>
      
export default {
name: 'AddNode',
data() {
    return {
        ips: ""
    }
},
computed: {
    state() {
        return this.ips.length >= 4
      },
      invalidFeedback() {
        
        return 'Нужно ввести хотя бы один IP адрес'
      }
}
}
</script>
      
<style>
      
</style>