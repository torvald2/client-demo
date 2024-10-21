<template lang="pug">
    b-modal(id="wallets-modal" ref="wallets-modal"  size="lg" title="Добавить/удалить кошельки")
      b-form(inline)
        b-form-input(placeholder="Имя")
        b-form-input(placeholder="Адрес")
        b-button(pill variant="primary").ml-2
          b-icon(icon="plus")
      br
      b-form(inline v-for="wallet in wallets").mt-2
        b-form-input(v-model="wallet.name")
        b-form-input(v-model="wallet.address")
        b-button( variant="success").ml-2
          b-icon(icon="check")
        b-button( variant="danger")
          b-icon(icon="trash")
      template(#modal-footer="{ ok, cancel, hide }")
        b-button(squared variant="outline-primary")
            b-icon(icon="x-circle")
            span.mr-1 
            | Закрыть
  </template>
        
  <script>
        
  export default {
  name: 'AddNode',
  components: {
  },
  data() {
    return {
        wallets :[
            {
            name: "primary",
            address:"NKNPthYDzwJuPuxNGhdnNjDZN7X6uLt1qRUS"
            },
            {
            name: "secondary",
            address:"NKNPthYDzwJuPuxNGhdnNjDZN7X6uLt1qRUS"
            },
    
    ]
    }
  }
  }
  </script>
        
  <style>
        
  </style>