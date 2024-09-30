<template>


  <RouterView />
</template>

<script>

import i18n from "./i18n"
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'App',
  setup() {


    document.querySelector('html').setAttribute('lang', i18n.global.locale.value)

    return {}
  }
})
</script>

<style scoped></style>
