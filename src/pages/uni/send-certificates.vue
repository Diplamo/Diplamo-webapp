<script setup lang="ts">
/**
 * This is a Vue Component that will be
 * automatically mapped to a entry on vue-router.
 * Read more about routing:
 * @see /vite.config.ts
 * @see /src/router.ts
 */

import { useHead } from '@vueuse/head'
import { pageTitle } from '/@src/state/navbarLayoutState'

pageTitle.value = 'Send Certificates'
useHead({
  title: 'Send Certificates',
})
</script>

<template>
  <CustomNavbarSearchLayoutUni theme="center">
    <!-- Content Wrapper -->
    <div class="page-content-inner">
      <CustomFormLayoutStepper class="is-navbar" />
    </div>
  </CustomNavbarSearchLayoutUni>
</template>
