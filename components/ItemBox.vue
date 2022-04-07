<template>
  <div class="item-container">
    <div v-for="item in items" :key="item.id" class="item-box">
      <div class="item">
        <div class="item-up">
          <div style="font-size: 1rem">{{ item.name }}</div>
          <div style="font-size: 0.5rem">{{item.description}}</div>
        </div>
        <div class="item-bottom">
          <div style="font-size: 1rem; font-weight: bold">{{item.price}}$</div>
          <div style="font-size: 1rem; font-weight: bold">
            <i style="color: yellow" class="fa-solid fa-star"></i>{{item.rating}}
          </div>
        </div>
      </div>
      <img style="position: absolute" src="~/static/1.jpeg" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { id: "1", name: "Cool", description: "Lana Furniture", price: 100, rating: 3.5 },
        { id: "2", name: "Elephant", description: "Lana Furniture", price: 400, rating: 4.2 },
        { id: "3", name: "Minimal", description: "Lana Furniture", price: 1000, rating: 5.0 },
        { id: "4", name: "Maxima", description: "Lana Furniture", price: 2000, rating: 4.2 },
        { id: "5", name: "Best", description: "Lana Furniture", price: 3000, rating: 2.5 },
      ],
    };
  },
};
</script>

<style>
.item-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;

}
.item-box {
  display: flex;
  justify-content: center;
  padding: 2rem;
  height: 14rem;
  margin-bottom: 3rem;
}
.item-box:after {
  position: absolute;
  content: "";
  top: 10px;
}
.item-box:hover {
  cursor: pointer;
  transform: translateY(-3%);
}
.item:hover {
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(64, 255, 0, 0.3) 0px 30px 60px -30px,
    rgba(70, 130, 80, 0.35) 0px -2px 6px 0px inset;
}
.item {
  position: relative;
  display: flex;
  justify-content: flex-end;
  flex-direction: column;
  top: 2rem;
  width: 10rem;
  height: 12rem;
  background-color: rgb(255, 255, 255);
  border-radius: 1rem;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(0, 0, 0, 0.3) 0px 30px 60px -30px,
    rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
}
.item-up {
  margin-left: 1rem;
}
.item-bottom {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-left: 1rem;
  margin-right: 1rem;
  margin-bottom: 0.5rem;
}
img {
  width: 9rem;
  position: absolute;
  border-radius: 1rem;
}
</style>
