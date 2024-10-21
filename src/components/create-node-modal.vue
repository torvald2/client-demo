<template lang="pug">
    b-modal(id="create-solo-node-modal" ref="create-solo-node-modal"  size="lg" title="Создать ноду Solo")
      b-form-group( label="Имя пользователя ")
        b-form-input(type="text")
      b-form-group( label="Пароль")
        b-form-input(type="text")
      b-form-group( label="Время ожидания ")
        b-form-input(type="number")
      b-form-group(description="Только Ipv4 адреса, каждый с новой строки" label="Свободных генераций: 10" :invalid-feedback="invalidFeedback" :state="state")
        b-form-textarea(v-model="ips" rows="10")
      template(#modal-footer="{ ok, cancel, hide }")
        b-button(squared variant="success").ml-2
          b-icon(icon="file-earmark-lock")
          span.mr-1 
          | Создать ноду Solo
  </template>
        
  <script>
        
  export default {
  name: 'AddNode',
  data() {
    return {
        ips: ""
    }
  },
  components: {
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