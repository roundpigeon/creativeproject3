<template>
  <div class="donate">
    <h1>Donations</h1>
    <p id="donate-p">We work hard to take care of all of our cats. We'd
      appreciate it greatly if you donated to us. Every dollar helps!</p>
    <h2>Choose a donation amount:</h2>
    <div id="donation-buttons">
      <button type="button">$1</button>
      <button type="button">$5</button>
      <button type="button">$10</button>
      <button type="button">$20</button>
      <button type="button">$100</button>
    </div>
  </div>
</template>

<style>
.donate {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

#donation-buttons {
  display: flex;
  flex-direction: row;
}

button {
  margin: 5px 5px 5px 5px;
  padding: 5px 10px 5px 10px;
  height: 3rem;
  border: 2px solid black;
  border-radius: 4px;
  font-size: 1.25rem;
}

button:hover {
  background-color: #b8b8b8;
}

button:active {
  background-color: #efefef;
}

h1 {
  font-size: 3.5rem;
  margin: 35px 0 35px 0;
}

#donate-p {
  font-size: 1.25rem;
}
</style>
