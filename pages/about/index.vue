<template>
  <div class="about container">
    <h1 class="title">about Page</h1>
    <p>詳細ページのテストです。</p>
  </div>
</template>

<style>
.title {
  text-align: center;
  margin: 2em;
}
</style>

<script>
export default {
  data() {
    return {
      meta: {
        title: 'about',
        description: '概要',
      },
    }
  },
  head() {
    return {
      title: this.meta.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: this.meta.description,
        },
      ],
    }
  },
}
</script>
