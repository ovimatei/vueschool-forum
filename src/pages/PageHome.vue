<template>
  <div class="col-full">
    <h1>Welcome to the forum</h1>
    <CategoryList :categories="categories"/>
  </div>
</template>

<script>
import sourceData from '@/data'
import CategoryList from '@/components/CategoryList'

console.log(sourceData)
export default {
  name: 'Home',
  components: {CategoryList},
  data () {
    return {
      categories: sourceData.categories
    }
  }
}
</script>
