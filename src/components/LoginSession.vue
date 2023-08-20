<template>
  <div>
    <v-toolbar id="toolbarColor">
      <v-spacer></v-spacer>
      <v-toolbar-title>
        <h3>{{ tituloLogin }}</h3>
      </v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
  </div>
</template>
<script>
export default {
  name: 'LoginSession',
  data() {
    return {
      titulo: -1,
    };
  },

  computed: {
    tituloLogin() {
      return this.titulo === -1 ? 'Sistema de Autenticación' : '';
    },
  },
};
</script>

<style>
#toolbarColor{
  font-family: Georgia, 'Times New Roman', Times, serif;
  background-color: #15395A;
  color: white;
  font-size: 20px;
}
</style>
