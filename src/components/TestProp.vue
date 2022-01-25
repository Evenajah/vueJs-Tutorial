<template>
  {{ msg }}
</template>

<script>
export default {
  name: 'TestProp',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
