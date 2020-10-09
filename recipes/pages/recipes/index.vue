<!-- eslint-disable -->
<template>
  <section class="recipes">
    <Recipe
      thumbnail="https://andyshelter.com/wp-content/uploads/2015/07/1-cheesecake-1183.jpg"
      title="Cheesecake"
      previewText="Best Cheesecake ever"
    />
    <Recipe
      thumbnail="https://res.cloudinary.com/hv9ssmzrz/image/fetch/c_fill,f_auto,h_600,q_auto,w_800/https://s3-eu-west-1.amazonaws.com/images-ca-1-0-1-eu/tag_photos/original/889/pizza_flickr_4932057475_2a9ce50750_b.jpg"
      title="Pizza"
      previewText="Best Pizza ever"
    />
  </section>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
  components: {
    Recipe,
  },
}
</script>

<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
</style>
