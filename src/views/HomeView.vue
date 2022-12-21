<template>
  <div class="home">
    <ItemsListComponent :items="items" />
  </div>
</template>

<script lang="ts">
import {defineComponent} from "vue";
import ItemsListComponent from "@/components/items/ItemsList.component.vue"
export default defineComponent({
  name:'Home',

  components:{
    ItemsListComponent
  },
  setup(){
    const items:any[] = [
      {id:1, name:"Jerusalema"},
      {id:2, name:"Ikayayami"},
      {id:3, name:"londonoze"},
      {id:4, name:"Nanishielana"},
    ]

    return {
        items
    }
  }
})
</script>
