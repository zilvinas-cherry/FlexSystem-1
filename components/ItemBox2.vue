<template>
  <div class="item2-container">
    <div v-for="item in items" :key="item.id" class="item2-box">
      <div class="item2">
        <div class="item2-up">
          <div style="font-size: 1rem; font-weight: 400; margin-bottom: 0.3rem;">{{ item.name }}</div>
          <div style="font-size: 0.5rem; font-weight: 100; margin-bottom: 0.3rem;">{{ item.description }}</div>
        </div>
        <div class="item2-bottom">
          <div style="font-size: 1rem; font-weight: 400">
            {{ item.price }}$
          </div>
          <div style="font-size: 1rem; font-weight: 400">
            <i style="color: rgb(254,190,0); margin-right: 0.5rem; font-size: 0.8rem" class="fa-solid fa-star"></i
            >{{ item.rating }}
          </div>
        </div>
      </div>
      <img class="item2img" src="~/static/1.jpeg" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          id: "1",
          name: "Sofa \"Treza\"",
          description: "Lane Furniture",
          price: 100,
          rating: 3.5,
        },
        {
          id: "2",
          name: "Sofa \"Lolly\"",
          description: "Lane Furniture",
          price: 400,
          rating: 4.2,
        },
        {
          id: "2",
          name: "Sofa \"Molly\"",
          description: "Lane Furniture",
          price: 400,
          rating: 4.2,
        },
      ],
    };
  },
};
</script>

<style>
.item2-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
}

.item2-box {
    position: relative;
    display: flex;
    justify-content: center;
    padding: 3rem;
    height: 10rem;
    
  }

.item2-box:after {
  position: absolute;
  content: "";
  top: 10px;
}
.item2-box:hover {
  cursor: pointer;
  transform: translateY(-3%);
}
.item2:hover {
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(64, 255, 0, 0.3) 0px 30px 60px -30px,
    rgba(70, 130, 80, 0.35) 0px -2px 6px 0px inset;
}
.item2 {
  position: relative;
  display: flex;
  justify-content: flex-end;
  flex-direction: column;
  width: 11rem;
  height: 11rem;
  background-color: rgb(255, 255, 255);
  border-radius: 1rem;
 box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
}
.item2-up {
  margin-left: 1rem;
}
.item2-bottom {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  margin-left: 1rem;
  margin-right: 1rem;
  margin-bottom: 0.5rem;
}
.item2img {
  width: 9rem;
  height: 8.5rem;
  position: absolute;
  border-radius: 1rem;
  bottom: 6.5rem;

}
</style>
