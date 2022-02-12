<template>
  <article></article>
</template>

<script>
export default {
  name: "ShowAllApps",
  props:['Vis']
}
</script>



<style v-if="Vis == true">
* {
  filter: brightness(80%);
}
</style>