<template>
  <div class="head">
    <ul class="menu-list">
      <li>Product</li>
      <li>About</li>
      <li>Blog</li>
      <li>Contact us</li>
    </ul>
    <div class="cart">
      <div class="quantity">2</div>
      <i style="color: white; font-size: 1.1rem" class="fa-solid fa-suitcase-rolling"></i>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.head {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 100%;
  border-top-right-radius: 25px;
  margin: 2rem;
  
}
.menu-list > li {
  display: inline;
  margin: 1rem;
  font-size: 1.1rem;
  
}

.menu-list > li:hover {
  cursor: pointer;
  background-color: rgb(202, 202, 202);
  padding: 0.5rem;
  border-radius: 0.5rem;
}

.cart{
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 25%;;
  height: 2.6rem;
  width: 2.6rem;
  background-color: #FF5F38;
font-size: 2rem; cursor: pointer; color: #FF5F38
}
.quantity{
  display: flex;
  align-items: center;
  justify-content: center;
 position: absolute;
 height: 1.5rem;
 width: 1.5rem;
 border-radius: 50%;
 z-index: 2;
 color: black;
 background-color: white;
 margin-left: 2.5rem;
 margin-bottom: 2.5rem;
 font-size: 0.8rem;
}
</style>
