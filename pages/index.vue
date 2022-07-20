
<template>
  <section class="section">
    <div class="container">
      <h1 class="title">Dashboard</h1>

      <!-- <p>Hi {{ user.name }}</p> -->
    </div>
  </section>
</template>

<script>
export default {
  name : 'indexPage',
  data() {
    return {
      user: this.$auth.user,
    }
  }
}
</script>