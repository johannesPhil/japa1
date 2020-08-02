<template>
  <div>
    <h2>
      {{ myName }}
    </h2>
  </div>
</template>

<script>
export default {
  name: "MyName",
  props: {
    myName: String
  }
};
</script>

<style lang="scss" scoped></style>
