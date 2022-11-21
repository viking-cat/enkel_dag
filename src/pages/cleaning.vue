<template>
  <q-page>
    <div class="q-ma-sm">
      Detta är städsidan
    </div>
    <div class="q-ma-sm">
      <q-table :rows="rows" :columns="columns" row-key="name" />
      Gurgel
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'CleaningPage',
  data () {
    return {
      rows: [
        {
          id: 1,
          name: 'Panda',
          email: 'panda@chihuahua.com',
          age: 6
        },
        {
          id: 2,
          name: 'Lily',
          email: 'lily@chihuahua.com',
          age: 5
        }
      ],
      columns: [
        { label: 'name', field: 'name', name: 'name', align: 'left' },
        { label: 'email', field: 'email', name: 'email', align: 'left' },
        { label: 'age', field: 'age', name: 'age', align: 'center' }
      ]
    }
  }
})
</script>
