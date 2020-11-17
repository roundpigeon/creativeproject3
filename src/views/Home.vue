<template>
  <div class="home">
    <h1>Our Shelter Cats</h1>
    <div id="sortBy">
      Sort By:
      <select name="gender" id="gender">
        <option value="allGenders">All Genders</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
      </select>
      <select name="breed" id="breed">
        <option value="allBreeds">All Breeds</option>
        <option value="shorthair">Domestic Shorthair</option>
        <option value="mediumhair">Domestic Mediumhair</option>
        <option value="longhair">Domestic Longhair</option>
        <option value="russianBlue">Russian Blue</option>
      </select>
    </div>
    <div id="grid">
      <CatList :cats="cats" />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {

  }
}
</script>

<style>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

h1 {
  font-size: 3rem;
}

select {
  margin: 0px 4px 0px 4px;
  font-size: 1.25rem;
  padding: 2px 2px 2px 2px;
  border: 2px solid black;
  border-radius: 4px;
}

#sortBy {
  font-size: 1.25rem;
}
</style>

<script>
import CatList from "../components/CatList.vue"
export default {
  name: 'Home',
  components: {
    CatList
  },
  data() {
    return {
    }
  },
  computed: {
    cats() {
      return this.$root.$data.cats;
    }
  },
}
</script>
