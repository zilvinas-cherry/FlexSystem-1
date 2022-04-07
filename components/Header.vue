<template>
  <div class="head">
    <ul class="menu-list">
      <li>Product</li>
      <li>About</li>
      <li>Blog</li>
      <li>Contact us</li>
    </ul>
    <div style="font-size: 3rem; margin-bottom: 1rem; cursor: pointer">
      <i class="fa-solid fa-shop"></i>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.head{
    display: flex;
     justify-content: flex-end;
         width: 100%;
     border-top-right-radius: 25px;
     margin: 2rem;
}
.menu-list > li {
  display: inline;
  margin: 1rem;
}

.menu-list > li:hover {
  cursor: pointer;
  background-color: rgb(202, 202, 202);
  padding: 0.5rem;
  border-radius: 0.5rem;
}
</style>
