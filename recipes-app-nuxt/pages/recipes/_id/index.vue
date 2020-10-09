<template>
  <section class="single-recipe">
    <h1>{{ recipe.title }}</h1>
    <div>
      <img class="recipe-image" :src="recipe.thumbnail" :alt="recipe.title" />
    </div>
    <p>{{ recipe.previewText }}</p>
  </section>
</template>

<script>
export default {
  asyncData(Context) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipe: [
            {
              id: '2',
              title: 'Pizza',
              previewText: 'Best Pizza ever',
              thumbnail:
                'https://res.cloudinary.com/hv9ssmzrz/image/fetch/c_fill,f_auto,h_600,q_auto,w_800/https://s3-eu-west-1.amazonaws.com/images-ca-1-0-1-eu/tag_photos/original/889/pizza_flickr_4932057475_2a9ce50750_b.jpg',
            },
            {
              id: '1',
              title: 'Cheesecake',
              previewText: 'Best Cheesecake ever',
              thumbnail:
                'https://andyshelter.com/wp-content/uploads/2015/07/1-cheesecake-1183.jpg',
            },
          ].find((el) => el.id === Context.params.id),
        })
      }, 1500)
    })
  },
}
</script>

<style scoped>
.single-recipe {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 30px;
}

.recipe-image {
  width: 80%;
  height: auto;
}
</style>
