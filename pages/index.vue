<template>
  <div>
    <div class="grid-container">
      <div class="grid-category">
        <div class="category-items">
          <div style="font-weight: 400; font-size: 1.5rem">Category</div>
          <MenuToggle />
          <h3 style="font-weight: 400">Filter by:</h3>
          <h3 style="font-weight: 400">Price</h3>
          <Colors />
          <Style />
        </div>
      </div>
      <div class="grid-header"><Header /></div>
      <div class="grid-contentas">
        <div class="item1"><ItemBox1 /></div>
        <div class="big-modal">
          <div><BigItemBox /></div>
          <div><BigModal /></div>
        </div>
        <div class="item22"><ItemBox2 /></div>
      </div>
    </div>
  </div>
</template>

<script>
import ItemBox1 from "~/components/ItemBox1";
import MenuToggle from "~/components/MenuToggle";
import PriceSlider from "~/components/PriceSlider";
import Colors from "~/components/Colors";
import BigModal from "~/components/BigModal";
export default {
  name: "IndexPage",
  components: { ItemBox1, MenuToggle, PriceSlider, Colors, BigModal },
 
};
</script>
<style>
html,
body {
  font-family: 'Lexend Deca', sans-serif;
  min-height: 100vh;
  background-color: rgb(173, 177, 177);
}
.grid-container {
  display: grid;
  margin-right: 300px;
  margin-left: 300px;
  margin-top: 150px;
  margin-bottom: 150px;
  grid-template-columns: 300px 1fr ;
  grid-template-areas:
    "category header"
    "category contentas";
}

.grid-category {
  position: relative;
  display: flex;
  grid-area: category;
  border-right: 1px solid rgb(123, 123, 123);
  width: 100%;
  min-height: 100%;
  background-color: rgb(255, 255, 255);
  border-bottom-left-radius: 25px;
  border-top-left-radius: 25px;
}

.category-items {
  margin-top: 2rem;
  margin-left: 3rem;
}

.grid-header {
  position: relative;
  display: flex;
  grid-area: header;
  margin-left: 0px;
  background-color: rgb(255, 255, 255);
  width: 100% -1px;
  margin-left: 1px;
font-weight: 300;
  border-top-right-radius: 25px;
}
.grid-contentas {
  display: grid;
  grid-area: contentas;
  width: 100%;
  background-color: rgb(255, 255, 255);
  border-bottom-right-radius: 25px;
  grid-template-areas:
    "item1 modal"
    "item2 item2";
}

@media (max-width: 1700px) {
  .grid-contentas {
    display: grid;
    grid-area: contentas;
    width: 100%;
    background-color: rgb(255, 255, 255);
    border-bottom-right-radius: 25px;
    grid-template-areas:
      "modal"
      "item1"
      "item2"
      ;
  }
}
.item1 {
  grid-area: item1;
  width: 100%;
}

.big-modal {
  grid-area: modal;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 30rem;
  width: 100%;
  background-color: rgb(230, 230, 230);
  border-radius: 25px;
}
.item22 {
  grid-area: item2;
  width: 100%;
}
</style>
