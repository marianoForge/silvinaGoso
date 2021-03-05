<template>
  <v-btn color="primary" rounded v-bind="$attrs" v-on="$listeners">
    <slot />
  </v-btn>
</template>

<script>
export default {
  name: "BaseBtn",
};
</script>
