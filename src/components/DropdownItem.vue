<template>
  <li class="dropdown-option" :class="{ 'is-diabled': disbaled }">
    <slot></slot>
  </li>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  props: {
    disbaled: {
      type: Boolean,
      default: false
    }
  }
})
</script>

<style scoped>
.dropdown-option.is-disabled * {
  color: #6c757d;
  pointer-events: none;
  background-color: transparent;
}
</style>
