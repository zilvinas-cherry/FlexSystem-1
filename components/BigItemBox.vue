<template>
  <div class="itemB-container">
    <div v-for="item in items" :key="item.id" class="itemB-box">
      <MoveNext />
      <div class="itemB">
        <div class="close-container">
          <div class="circlec"><i class="fa-solid fa-xmark"></i></div>
        </div>
        <div class="itemB-up">
          <div
            style="font-size: 1.5rem; font-weight: 400; margin-bottom: 0.3rem"
          >
            {{ item.name }}
          </div>
          <div style="font-size: 1rem; font-weight: 200; margin-bottom: 0.6rem">
            {{ item.description }}
          </div>
        </div>
        <div class="big-heart"><i class="fa-brands fa-gratipay"></i></div>

        <div class="itemB-bottom">
          <div style="font-size: 1.5rem; font-weight: 500; color: black">
            {{ item.price }}$
          </div>
          <div style="font-size: 1.5rem; font-weight: 500; color: black">
            <i style="color: rgb(254, 190, 0); margin-right: 0.5rem; font-size: 1.25rem;" class="fa-solid fa-star"></i
            >{{ item.rating }}
          </div>
        </div>
      </div>
      <img class="itemBimg" src="~/static/3.jpg" />
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
  margin-left: 1px;
  align-items: flex-end;
  align-content: start;
}

.itemB-box {
  position: relative;
  display: flex;
  justify-content: center;
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
  box-shadow: 0 16px 32px rgba(0, 0, 0, 0.07), 0 32px 64px rgba(0, 0, 0, 0.07);
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
.big-heart {
  display:flex;
  position: absolute;
  align-items: center;
  height: 2.3rem;
  width: 2.3rem;
  border-radius: 50%;
  color: #fd4a62;
  font-size: 2.5rem;
  margin-left: 27rem;
  margin-bottom: 25rem;
  z-index: 10;
}
.big-heart:hover {
  cursor: pointer;
  box-shadow: 0px 0px 12px rgba(253, 74, 98, 0.9),
  0px 0px 13px rgba(253, 74, 98, 0.9);
}
.close-container {
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 5;
  margin-bottom: 19rem;
  margin-left: 2rem;
  width: 1.75rem;
  height: 1.75rem;

  opacity: 0.7;
}
.circlec {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 1.75rem;
  width: 1.75rem;
  border-radius: 50%;
  background-color: #adb1b1;
  font-size: 0.75rem;
}
.close-container:hover {
  border-radius: 50%;
  border: 1px solid #363636;
}
</style>
