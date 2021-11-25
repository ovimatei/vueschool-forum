<template>
  <div class="col-full">
    <h1>Not Found</h1>
    <p>Oops, we could't find the page you are looking for, why don't you
      <router-link :to="{name: 'Home'}">go home instead?</router-link>
    </p>
  </div>

</template>

<script>
export default {
  name: 'NotFound'
}
</script>

<style scoped>
h1 {
  font-size: 100px;
}

p {
  font-size: 50px;
  font-weight: 100;
}

div {
  text-align: center;
}
</style>
