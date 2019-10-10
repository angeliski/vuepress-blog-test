<template>
  <div>
  <div v-for="page in pages">
      <NavLink :link="page.path">Override {{ page.title }}</NavLink>
  </div> 
</div>
</template>
<script>
  export default {
    computed: {
      pages() {
        return this.$pagination.pages
      },
    },
  }
</script>