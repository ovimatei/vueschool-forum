<template>
  <div class="col-full">
    <h1>Welcome to the forum</h1>
    <ForumList :forums="Object.values(forums)"/>
  </div>
</template>

<script>
import sourceData from '@/data'
import ThreadList from '@/components/ThreadList'
import ForumList from '../components/ForumList'

console.log(sourceData)
export default {
  name: 'Home',
  components: {ForumList, ThreadList},
  data () {
    return {
      threads: sourceData.threads,
      posts: sourceData.posts,
      users: sourceData.users,
      forums: sourceData.forums
    }
  }
}
</script>
