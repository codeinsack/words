<template>
  <VContainer>
    <VRow>
      <VCol cols="12">
        {{ data }}
      </VCol>
    </VRow>
  </VContainer>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { useHelloWorld } from "./HelloWorld";

export default defineComponent({
  setup() {
    const { data } = useHelloWorld();

    return { data };
  }
});
</script>

<style scoped lang="scss"></style>
