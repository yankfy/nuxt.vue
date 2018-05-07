<template>
  <div>
    <h2>News Index page</h2>
    <p>NewsID:{{$route.params.newsId}}</p>
    <ul>
      <li>
        <a href="/">Home</a>
      </li>
      <li>
        <nuxt-link :to="{name: 'news-id',params:{id:123,title:'News-1'}}">News-1</nuxt-link>
        <!-- <br> -->
        <!-- <a href="/news/123">News-1</a> -->
      </li>
      <li>
        <nuxt-link :to="{name: 'news-id',params:{id:456,title:'News-2'}}">News-2</nuxt-link>
        <!-- <a href="/news/456">News-2</a> -->
      </li>
    </ul>
  </div>
</template>

<script>
  export default {

  }

</script>

<style>


</style>
