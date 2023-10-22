<template>
  <v-app>

    <nav-component>
    </nav-component>


    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

import NavComponent from './components/navegacion/NavComponent.vue';

export default {
  name: 'App',
  components: {
    NavComponent
  },

  data: () => ({
    //
  }),
};
</script>
