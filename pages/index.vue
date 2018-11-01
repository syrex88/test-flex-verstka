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

.list-items {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.container > div {
  min-width: 50%;
}

.item {
  height: 25vh;
  width: 100%;
  padding: 5px;
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
    width: 100%;
  }

  .list-items {
    flex-direction: row;
    flex-wrap: wrap;
    max-width: 100vh;
  }
}

</style>
