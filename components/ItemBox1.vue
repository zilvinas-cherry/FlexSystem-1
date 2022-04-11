<template>
  <div class="item-container">
    <div v-for="item in items" :key="item.id" class="item-box">
      <div class="item">
        <div class="item-up">
          <div style="font-size: 1rem; font-weight: 400; margin-bottom: 0.3rem">
            {{ item.name }}
          </div>
          <div
            style="font-size: 0.5rem; font-weight: 200; margin-bottom: 0.3rem"
          >
            {{ item.description }}
          </div>
        </div>
        <div class="heart"><i class="fa-brands fa-gratipay"></i></div>
        <div class="item-bottom">
          <div style="font-size: 1rem; font-weight: 600">{{ item.price }}$</div>
          <div style="font-size: 1rem; font-weight: 600; color: black">
            <i style="color: rgb(254, 190, 0); margin-right: 0.5rem; font-size: 0.8rem;" class="fa-solid fa-star"></i
            >{{ item.rating }}
          </div>
        </div>
      </div>
      <img class="item1img" :src="require(`~/static/${item.image}.jpg`)" />
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
          name: 'Sofa "Arson"',
          description: "Lane Furniture",
          price: 100,
          rating: 3.5,
          image: "1",
        },
        {
          id: "2",
          name: 'Sofa "Terry"',
          description: "Lane Furniture",
          price: 400,
          rating: 4.2,
          image: "2",
        },
      ],
    };
  },
};
</script>

<style>
@keyframes leftToRight {
        0% {
          Transform: Translatex(-50%);
          opacity: 0;
        }
        100% {
        Transform: Translatex(0%);
        opacity: 1;
        }
      }

@keyframes opacityRise {
        0% {
          opacity: 0.1;
        }
        100% {
          opacity: 1;
        }
      }

     
.item-container { 
  animation: 3s ease-out 0s 1 opacityRise;
  animation: 3s ease-out 0s 1 leftToRight;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  align-items: center;
  align-content: start;
  height: 100%;
}
@media (max-width: 1700px) {
  .item-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    height: 100%;
    margin-bottom: 3rem;
  }
}

.item-box {
  position: relative;
  display: flex;
  justify-content: center;
  padding: 3rem;
  height: 10rem;
}

@media (max-width: 1700px) {
  .item-box {
    position: relative;
    display: flex;
    margin-left: 2rem;
    margin-right: 2rem;
    justify-content: center;
    height: 10rem;
    margin-top: 3rem;
  }
}

.item-box:after {
  position: absolute;
  content: "";
 }
.item-box:hover {
  cursor: pointer;
  transform: translateY(-1%);
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
  width: 11rem;
  height: 11rem;
  background-color: rgb(255, 255, 255);
  border-radius: 1rem;
  box-shadow: 0 16px 32px rgba(0, 0, 0, 0.07), 0 32px 64px rgba(0, 0, 0, 0.07);
}
.item-up {
  margin-left: 1rem;
}
.item-bottom {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  margin-left: 1rem;
  margin-right: 1rem;
  margin-bottom: 0.5rem;
}
.item1img {
  width: 9rem;
  height: 8.5rem;
  position: absolute;
  border-radius: 1rem;
  bottom: 6.5rem;
}
.heart {
  display: flex;
  position: absolute;
  color: rgb(253, 74, 98);
  font-size: 1.5rem;
  height: 1.4rem;
  width: 1.4rem;
  border-radius: 50%;
  margin-left: 9rem;
  margin-bottom: 11rem;
  z-index: 10;
   box-shadow: 0px 8px 12px rgba(253, 74, 98, 0.487),
  0px 6px 13px rgba(253, 74, 98, 0.392);
}

.heart:hover {
  cursor: pointer;
  box-shadow: 0px 0px 12px rgba(253, 74, 98, 0.9),
  0px 0px 13px rgba(253, 74, 98, 0.9);
}
</style>
