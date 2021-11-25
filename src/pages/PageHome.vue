<template>
  <div class="col-full">
    <h1>Welcome to the forum</h1>
    <ThreadList :threads="Object.values(threads)"/>
  </div>
</template>

<script>
import sourceData from '@/data'
import ThreadList from '@/components/ThreadList'

console.log(sourceData)
export default {
  name: 'Home',
  components: {ThreadList},
  data () {
    return {
      threads: sourceData.threads,
      posts: sourceData.posts,
      users: sourceData.users
    }
  }
}
</script>
