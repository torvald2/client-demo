<template lang="pug">
    b-modal(id="npool-modal" ref="npool-modal"  size="lg" title="Создать ноду nPool")
      b-form-group( label="Имя пользователя ")
        b-form-input(type="text")
      b-form-group( label="Пароль")
        b-form-input(type="text")
      b-form-group( label="Время ожидания ")
        b-form-input(type="number")
      b-form-group(description="Только Ipv4 адреса, каждый с новой строки" label="Свободных генераций: 10" :invalid-feedback="invalidFeedback" :state="state")
        b-form-textarea(v-model="ips" rows="10")
      template(#modal-footer="{ ok, cancel, hide }")
        b-button(squared variant="warning").ml-2
          b-icon(icon="globe")
          span.mr-1 
          | Coздать ноду nPool
  </template>
        
  <script>
        
  export default {
  name: 'AddNode',
  components: {
  }
  }
  </script>
        
  <style>
        
  </style>