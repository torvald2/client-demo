<template lang="pug">
b-card-group
  b-card( header="Статистика Solo" bg-variant="success")
    b-card-text
      b-list-group
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
         | Всего
         b-badge(variant="primary" pill) 30
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
         | В ожидании
         b-badge(variant="warning" pill) 10
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
         | Online
         b-badge(variant="success" pill) 19
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="success")
         | Ошибка
         b-badge(variant="danger" pill) 1
  b-card( header="Количество блоков" bg-variant="warning").ml-2
    b-card-text
      b-list-group
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="warning")
         | Текущие сутки
         b-badge(variant="primary" pill) 335
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="warning")
         | Прошедшие сутки
         b-badge(variant="warning" pill) 466
  b-card( header="Статистика NPool" bg-variant="info").ml-2
    b-card-text
      b-list-group
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="info")
         | Всего
         b-badge(variant="primary" pill) 30
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="info")
         | В ожидании
         b-badge(variant="warning" pill) 10
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="info")
         | Online
         b-badge(variant="success" pill) 19
        b-list-group-item(class="d-flex justify-content-between align-items-center" variant="info")
         | Ошибка
         b-badge(variant="danger" pill) 1

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
      