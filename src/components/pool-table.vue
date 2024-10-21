<template lang="pug">
b-card(header="Ноды:" bg-variant="light")
  b-table(:items="items" :fields="fields" )
    template(#cell(actions)="row")
      b-button(size="sm" variant="danger")
        b-icon(icon="trash")
  b-pagination(total-rows="1000"  per_page="50")
</template>
          
    <script>
    
    
    export default {
    name: 'navBar',
    data() {
        return {
            items:[
                {
                    "num":1,
                    "ip":"172.16.29.12",
                    "status":"ONLINE",
                    "proposed":10,
                    "work_time":"10h30m",
                    "r_h":10,
                    "r_h_1":600,
                    "ver":"1.0.1"
                },
                {
                    "num":2,
                    "ip":"172.16.29.13",
                    "status":"ERROR",
                    "proposed":0,
                    "work_time":"10h30m",
                    "r_h":0,
                    "r_h_1":0,
                    "ver":"1.0.1"
                },
                {
                    "num":3,
                    "ip":"172.16.30.1",
                    "status":"WAITING",
                    "proposed":0,
                    "work_time":"0",
                    "r_h":0,
                    "r_h_1":0,
                    "ver":"0"
                }
            ],
            fields:[
                {key:"num", label:"#", sortable: true},
                {key:"ip", label:"IP Address", sortable: false},
                {key:"status", label:"Status", sortable: false},
                {key:"proposed", label:"Proposed", sortable: true},
                {key:"work_time", label:"Время работы", sortable: true},
                {key:"r_h", label:"R/H", sortable: true},
                {key:"r_h_1", label:"R/H 1 Час ", sortable: true},
                {key:"ver", label:"Версия", sortable: false},
                {key:"actions", label:"", sortable: false},


                
            ],
        }

    },
    components: {
       
    },
    methods:{
       
    }
    }
    </script>
          
    <style>
          
    </style>
          