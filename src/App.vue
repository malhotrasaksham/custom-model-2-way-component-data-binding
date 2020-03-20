<template>
  <div id="app">
    <app-child v-model="data"></app-child>
    {{data}}
  </div>
</template>

<script>
import child from "@/components/child";

export default {
  components: {
    "app-child": child
  },
  data() {
    return {
      data: undefined
    };
  }
};
</script>

