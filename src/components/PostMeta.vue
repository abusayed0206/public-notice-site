<template>
   <div class="post-meta">
      Posted on  {{ post.date }}.
      <template v-if="post.timeToRead">
        <strong>Read Time: {{ post.timeToRead }} min</strong>
      </template>
    </div>
</template>

<script>
export default {
  props: ['post']
}
</script>

<style lang="scss">
.post-meta {
  font-size: .8em;
  opacity: .8;
}
</style>