<template>
  <div  class="toolbar">
    <q-ajax-bar color="#80cbc4"></q-ajax-bar>
    <router-link :to="'/'" v-if="$router.currentRoute.meta.backButton">
      <button>
        <i>arrow_back</i>
      </button>
    </router-link>
    <button class="hide-on-drawer-visible" @click="$parent.$children[1].$refs.leftDrawer.open()" v-else >
      <i>menu</i>
    </button>
    <q-toolbar-title :padding="1">
      Quasar Admin App
    </q-toolbar-title>
    <button>
      <a href="https://github.com/odranoelBR/vue-quasar-admin-example" class="text-white">
        <i class="fa fa-2x fa-github"></i>
      </a>
      <span class="label bg-primary text-white">
        <i class="on-left">mail</i>
        10
      </span>
    </button>
  </div>
</template>
<script>
  export default {
  }
</script>
<style scoped></style>
