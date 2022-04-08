<template>
  <div class="head">
    <ul class="menu-list">
      <li>Product</li>
      <li>About</li>
      <li>Blog</li>
      <li>Contact us</li>
    </ul>
    <div style="font-size: 2rem; cursor: pointer; color: rgb(252, 70, 42)">
      <i class="fa-solid fa-shop"></i>
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
  width: 90%;
  border-top-right-radius: 25px;
  margin: 2rem;
  
}
.menu-list > li {
  display: inline;
  margin: 1rem;
  font-size: 1rem;
  
}

.menu-list > li:hover {
  cursor: pointer;
  background-color: rgb(202, 202, 202);
  padding: 0.5rem;
  border-radius: 0.5rem;
}
</style>
