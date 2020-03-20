<template>
  <div>
    <input type="text" :value="inputValue" @input="Emit($event.target.value)">
  </div>
</template>

<script>
export default {
  model: {
    prop: "inputValue",
    event: "emitValue"
  },
  props: {
    inputValue: String
  },
  methods: {
    Emit(value) {
      this.$emit("emitValue", value);
    }
  }
};
</script>
