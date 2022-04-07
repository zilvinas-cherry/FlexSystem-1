<template>
  <div>
    <div class="grid-container">
      <div class="grid-category">
        <div class="category-items">
          <h3>Category</h3>
          <MenuToggle />
          <h4>Filter by:</h4>
          <h4>Price</h4>
          <Colors />
          <Style />
        </div>
      </div>
      <div class="grid-header"><Header /></div>
      <div class="grid-contentas">
        <div><ItemBox /></div>
        <div><BigItemBox /></div>
      </div>
    </div>
  </div>
</template>

<script>
import ItemBox from "~/components/ItemBox";
import MenuToggle from "~/components/MenuToggle";
import PriceSlider from "~/components/PriceSlider";
import Colors from "~/components/Colors";
export default {
  name: "IndexPage",
  components: { ItemBox, MenuToggle, PriceSlider, Colors },
};
</script>
<style>
html,
body {
  min-height: 100vh;
  background-color: rgb(177, 177, 177);
}
.grid-container {
  display: grid;
  margin: 50px;
  grid-template-columns: 250px 1fr 1fr 1fr;
  grid-template-areas:
    "category header header header"
    "category contentas contentas contentas";
}

.grid-category {
  position: relative;
  display: flex;
  grid-area: category;
  border-right: 1px solid rgb(123, 123, 123);
  width: 100%;
  min-height: 100%;
  background-color: rgb(237, 234, 242);
  border-bottom-left-radius: 25px;
  border-top-left-radius: 25px;
}

.category-items {
  margin-left: 2rem;
 
}

.grid-header {
  position: relative;
  display: flex;
  grid-area: header;
  width: 100%;
  background-color: rgb(237, 234, 242);
  border-top-right-radius: 25px;
}

.grid-contentas {
  display: flex;
  flex-wrap: wrap;
  grid-area: contentas;

  width: 100%;
  background-color: rgb(237, 234, 242);
  border-bottom-right-radius: 25px;
}
</style>
