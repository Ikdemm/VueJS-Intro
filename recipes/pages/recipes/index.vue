<!-- eslint-disable -->
<template>
  <section class="recipes">
    <article class="recipe">
      <div
        class="thumbnail"
        style="
          background-image: url('https://andyshelter.com/wp-content/uploads/2015/07/1-cheesecake-1183.jpg');
        "
      ></div>
      <h1>Cheesecake</h1>
      <p>Some nice preview text</p>
    </article>
    <article class="recipe">
      <div
        class="thumbnail"
        style="
          background-image: url('https://res.cloudinary.com/hv9ssmzrz/image/fetch/c_fill,f_auto,h_600,q_auto,w_800/https://s3-eu-west-1.amazonaws.com/images-ca-1-0-1-eu/tag_photos/original/889/pizza_flickr_4932057475_2a9ce50750_b.jpg');
        "
      ></div>
      <h1>Pizza</h1>
      <p>Some nice preview text</p>
    </article>
  </section>
</template>

<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}

.recipe {
  box-sizing: border-box;
  width: 280px;
  padding: 8px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #aaa;
}

.thumbnail {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 200px;
}
</style>
