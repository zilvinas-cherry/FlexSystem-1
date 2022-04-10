<template>
  <div class="bmodal-container">
    <div class=mtop>
      <div class="review">1 review</div>
      <div class="stars">
        <i class="fa-solid fa-star"/>
        <i class="fa-solid fa-star"/>
        <i class="fa-solid fa-star"/>
        <i class="fa-solid fa-star"/>
        <i style="color: #939393" class="fa-solid fa-star"/>
      </div>
    </div>
    <div class="mtitle">
      <div class="mname">SOFA "MARTA"</div>
      <div class="mprice">750$</div>
    </div>
    <div class="desc-text">
      Marta is a small sofa with a big heart, that fits perfectly wherever space
      is limited. Smartly designed liteweight, a comfortable padded cover and
      uses less material - good for the planet.
    </div>
    <div class="soc-media">
      <div class="instagram"><i class="fa-brands fa-instagram"></i></div>
      <div class="facebook"><i class="fa-brands fa-facebook-square"></i></div>
      <div class="twitter"><i class="fa-brands fa-twitter"></i></div>
    </div>
    <div class="bm-bottom">
      <div class="add-to-cart">ADD TO CART</div>
      <div class="add-to-wishlist">Add to wish list</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.bmodal-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  height: 30rem;
  width: 20rem;
  margin-right: 1rem;
  
}
.mtop{
  display:flex;
  margin-left: 1rem;
  width: calc(100% - 2rem);
  align-items: center;
  justify-content: space-between;
  margin-bottom: 2rem;
  width: 90%;
 
}
.review{
  font-weight: 300;
  color: #939393;
}
.review:hover{
  cursor: pointer;
  
}
.stars{
  display: flex;
  gap: 0.5rem;
  font-size: 0.5rem;;
  color: rgb(254,190,0);
 
}

.mtitle{
  display: flex;
  margin-left: 1rem;
  margin-right: 1rem;
 justify-content: space-between;
  margin-bottom: 2rem;

}
.mname{
  font-size: 1.5rem;
}
.mprice{
  font-size: 1.5rem;
}
.desc-text {
  margin-left: 1rem;
  margin-bottom: 2rem;

  font-size: 0.8rem;
  line-height: 1.8;
}
.soc-media {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-left: 1rem;
  margin-bottom: 3rem;
  font-size: 1rem;
}
.instagram {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2rem;
  width: 2rem;
  border: 1px solid #433e5c;
  border-radius: 0.5rem;
}
.instagram:hover {
  cursor: pointer;
}
.facebook {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2rem;
  width: 2rem;
  border: 1px solid #433e5c;
  border-radius: 0.5rem;
}
.facebook:hover {
  cursor: pointer;
}
.twitter {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2rem;
  width: 2rem;
  font-weight: 100;
  border: 1px solid #433e5c;
  border-radius: 0.5rem;
}
.twitter:hover {
  cursor: pointer;
}
.bm-bottom {
  display: flex;
  align-items: center;
  justify-content: center;

  width: 100%;
  height: 20%;
}
.add-to-cart {
  background: rgb(47, 43, 68);
  background: linear-gradient(
    276deg,
    rgba(47, 43, 68, 1) 0%,
    rgba(90, 85, 118, 1) 100%
  );
  color: #fec856;
  font-size: 0.7rem;
  padding: 1rem;
  border-radius: 0.8rem;
}
.add-to-cart:hover{
  cursor: pointer;
}
.add-to-cart:after {
  position: absolute;
  content: "";
  top: 10px;
}
.add-to-cart:hover {
  cursor: pointer;
  transform: translateY(-3%);
}
.add-to-wishlist {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0.5rem 1rem 0.5rem 1rem;
  font-size: 0.7rem;
  margin: 2rem;
  border: 1px solid #433e5c;
  border-radius: 2rem;
}
.add-to-wishlist:hover{
  cursor: pointer;
}
.add-to-wishlist:after {
  position: absolute;
  content: "";
  top: 10px;
}
.add-to-wishlist:hover {
  cursor: pointer;
  transform: translateY(-3%);
}
</style>
