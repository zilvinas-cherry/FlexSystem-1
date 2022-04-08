<template>
  <div>
    <h3 style="font-weight: 400">Color</h3>
    <ul class="colors-list">
      <li class="colors" style="background-color: rgb(240, 229, 229)"></li>
      <li class="colors" style="background-color: rgb(38, 38, 99)"></li>
      <li class="colors" style="background-color: rgb(67, 23, 32)"></li>
      <li class="colors" style="background-color: rgb(106, 0, 0)"></li>
      <li class="colors" style="background-color: rgb(98, 255, 20)"></li>
      <li class="colors" style="background-color: rgb(16, 255, 227)"></li>
      <li class="colors" style="background-color: rgb(255, 0, 0)"></li>
      <li class="colors" style="background-color: rgb(255, 238, 0)"></li>
      <li class="colors" style="background-color: rgb(255, 145, 0)"></li>
      <li class="colors" style="background-color: rgb(76, 76, 255)"></li>
      <li class="colors" style="background-color: rgb(96, 69, 13)"></li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style>
.colors-list {
  margin-right: 1rem;
  width: 80%;
  font-weight: 500;
}
.colors {
  display: inline-block;
  width: 1.5rem;
  height: 1.5rem;
  border-radius: 50%;
  background-color: black;
  flex-basis: 12rem;
}
</style>
