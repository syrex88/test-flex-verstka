<template>
  <section class="container">
    <div class="list-items">
      <div class="item">
        <div>Item 1</div>
      </div>
      <div class="item">
        <div>Item 2</div>
      </div>
      <div class="item">
        <div>Item 3</div>
      </div>
      <div class="item">
        <div>Item 3</div>
      </div>
    </div>
    <div class="item gray">
      <div>Item</div>
    </div>
  </section>
</template>

<style>

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: black;
}

.container > * {
  max-width: 50%;
}

.list-items {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.item {
  height: 25vh;
  width: 25vh;
  padding: 5px;
  max-width: 100%;
}

.item div {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.item.gray div {
  background-color: gray;
}

.list-items .item div {
  background-color: red;
}

@media (min-width: 525px) {
  .item {
    height: 50vh;
    width: 50vh;
    max-width: 100%;
  }

  .list-items {
    flex-direction: row;
    flex-wrap: wrap;
    max-width: 50%;
    width: 100vh;
  }
}

</style>
