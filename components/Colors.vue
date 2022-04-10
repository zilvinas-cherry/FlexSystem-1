<template>
  <div>
    <h3 style="font-weight: 400">Color</h3>
    <ul class="colors-list">
      <li class="colors" style="background-color: #365653"></li>
      <li class="colors" style="background-color: #C4C4C4"></li>
      <li class="colors" style="background-color: #000000"></li>
      <li class="colors" style="background-color: #6E4B15"></li>
      <li class="colors" style="background-color: #05426D"></li>
      <li class="colors" style="background-color: #109D2E"></li>
      <li class="colors" style="background-color: #FFF4CF"></li>
      <li class="colors" style="background-color: #C21A17"></li>
      <li class="colors" style="background-color: #FDE0F7"></li>
      <li class="colors" style="background-color: #7A3274"></li>
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
  width: 1.4rem;
  height: 1.4rem;
  border-radius: 50%;
  background-color: black;
  flex-basis: 12rem;
}
</style>
