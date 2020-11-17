<template>
  <div id="welcome">
    <div id="cat-shelter-welcome">
      <h1>Welcome to our shelter page!</h1>
      <p id="welcome-p">All of our cats are up to date on their shots and ready to be adopted. Take
        a look through our catalog today, and maybe you'll find a furry friend you
        fall in love with and take home!</p>
    </div>
        <p id="mock-data-banner">This mock data comes from the Utah Humane Society website. Many of these
        cats have already been adopted out, but if you're lucky, you can still find
        some of them <a href="https://www.utahhumane.org/adopt?f%5B0%5D=field_species%3A2">here</a>.
        </p>
  </div>
</template>

<style scoped>
#welcome {
  text-align: center;
  width: 60%;
}

p {
  margin-top: 5rem;
  text-align: left;
}

#mock-data-banner {
}

#welcome-p {
  font-size: 1.5rem;
}

#cat-shelter-welcome {
  border: 3px solid black;
  background-color: #efefef;
  border-radius: 5px;
  padding: 2rem 2rem 2rem 2rem;
  margin: 1rem 1rem 1rem 1rem;
}
</style>
