<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated='false' class="bg-transparent text-black">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          @click="leftDrawerOpen = !leftDrawerOpen"
          aria-label="Menu"
          icon="menu"
        />

        <q-toolbar-title>
          POLARS ROOM
        </q-toolbar-title>

        <div>POLARS v2.0</div>
      </q-toolbar>
    </q-header>

    

    <q-page-container>
      <router-view></router-view>
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  name: 'LayoutDefault',

  components: {
  },

  setup () {
    return {
      leftDrawerOpen: ref(false)
    }
  }
}
</script>
