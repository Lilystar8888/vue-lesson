<template>
  <div :class="{ list: true, red: active }">
    Hello
    <button @click="active = !active">Toggle</button>

    <h3 :style="{ background: active ? 'green' : 'red' }">World</h3>

  </div>
</template>

<script>
export default {
  data: () => ({
    active: false,
    text: "",
  }),
};
</script>

<style>
.list {
  color: green;
}
.list.red {
  color: red;
}
</style>