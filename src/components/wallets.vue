<template lang="pug">
    b-card-group
      b-card( header="Статистика кошельков" bg-variant="success")
        b-card-text
          b-list-group
            b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
             | Всего
             b-badge(variant="primary" pill) 20.003 NKN 
            b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
             | Primary (NKNPthYDzwJuPuxNGhdnNjDZN7X6uLt1qRUS)
             b-badge(variant="warning" pill) 10.001 NKN
            b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
             | Secondary (NKNPthYDzwJuPuxNGhdnNjDZN7X6uLt1qRUS)
             b-badge(variant="success" pill) 10.002 NKN
            
     
    
    </template>
          
    <script>
    
    
    export default {
    name: 'navBar',
    components: {
       
    },
    methods:{
       
    }
    }
    </script>
          
    <style>
          
    </style>
          