<!-- eslint-disable -->
<template>
  <section class="recipes">
    <Recipe
      v-for="recipe in recipes"
      :key="recipe.id"
      :thumbnail="recipe.thumbnail"
      :title="recipe.title"
      :previewText="recipe.previewText"
    />
  </section>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
  components: {
    Recipe,
  },
  asyncData() {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipes: [
            {
              id: '2',
              title: 'Pizza',
              previewText: 'Best Pizza ever',
              thumbnail:
                'https://andyshelter.com/wp-content/uploads/2015/07/1-cheesecake-1183.jpg',
            },
            {
              id: '1',
              title: 'Cheesecake',
              previewText: 'Best Cheesecake ever',
              thumbnail:
                'https://res.cloudinary.com/hv9ssmzrz/image/fetch/c_fill,f_auto,h_600,q_auto,w_800/https://s3-eu-west-1.amazonaws.com/images-ca-1-0-1-eu/tag_photos/original/889/pizza_flickr_4932057475_2a9ce50750_b.jpg',
            },
          ],
        })
      }, 1500)
    })
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
