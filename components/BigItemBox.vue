<template>
  <div class="itemB-container">
    <div v-for="item in items" :key="item.id" class="itemB-box">
      <div class="itemB">
        <div class="itemB-up">
          <div style="font-size: 2rem; font-weight: 400; margin-bottom: 0.3rem">
            {{ item.name }}
          </div>
          <div
            style="font-size: 1rem; font-weight: 100; margin-bottom: 0.6rem"
          >
            {{ item.description }}
          </div>
        </div>
        <div class="itemB-bottom">
          <div style="font-size: 2rem; font-weight: 400">{{ item.price }}$</div>
        <div style="font-size: 2rem; font-weight: 400">
            <i style="color: rgb(254,190,0); margin-right: 0.5rem; font-size: 0.8rem" class="fa-solid fa-star"></i
            >{{ item.rating }}
          </div>
        </div>
      </div>
      <img class="itemBimg" src="~/static/2.jpg" />
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
          name: 'SOFA "MARTA"',
          description: "Lane Furniture",
          price: 650,
          rating: 4.8,
        },
      ],
    };
  },
};
</script>

<style>
.itemB-container {
  display: flex;
   flex-wrap: wrap;
  align-items: flex-end;
  align-content: start;
}

.itemB-box {
  position: relative;
  display: flex;
  justify-content: center;
}

.itemB-box:after {
  position: absolute;
  content: "";
  top: 10px;
}
.itemB-box:hover {
  cursor: pointer;
  transform: translateY(-3%);
}
.itemB:hover {
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(64, 255, 0, 0.3) 0px 30px 60px -30px,
    rgba(70, 130, 80, 0.35) 0px -2px 6px 0px inset;
}
.itemB {
  position: relative;
  display: flex;
  justify-content: flex-end;
  flex-direction: column;
  width: 32rem;
  height: 22rem;
  background-color: rgb(255, 255, 255);
  border-radius: 1rem;
  box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
}
.itemB-up {
  margin-left: 1rem;
}
.itemB-bottom {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  margin-left: 1rem;
  margin-right: 1rem;
  margin-bottom: 0.5rem;
}
.itemBimg {
  width: 30rem;
  height: 20rem;
  position: absolute;
  border-radius: 1rem;
  bottom: 9rem;
}
</style>
