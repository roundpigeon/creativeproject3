<template>
<div class="wrapper">
  <div class="cats">
    <div class="cat" v-for="cat in cats" :key="cat.id">
      <div class="image">
        <img :src="'/images/'+cat.image" width="300px">
      </div>
      <div class="info">
        <h2>{{cat.name}}</h2>
        <p>{{cat.sex}}</p>
        <p>{{cat.breed}}</p>
        <p>{{cat.age}} old</p>
      </div>
    </div>
  </div>
</div>
</template>

<style>
.cats {
  display: flex;
  flex-direction: row;
}

.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
}

.cats {
  margin-top: 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.cat {
  margin: 10px;
  margin-top: 50px;
  width: 250px;
  border: 3px solid #333;
  border-radius: 5px;
}

.cat img {
  height: 250px;
  width: 250px;
  object-fit: cover;
}

.cat .image {
  display: flex;
  justify-content: center;
  margin-bottom: 5px;
}

.auto {
  margin-left: auto;
}
</style>

<script>
export default {
  name: 'CatList',
  props: {
    cats: Array
  }
}
</script>
