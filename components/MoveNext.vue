<template>
  <div class="mn-container">
    <div class="back"><i class="fa-solid fa-arrow-left"></i></div>
    <div class="small-ball"></div>
    <div class="small-ball"></div>
    <div class="middle-ball-container">
      <div class="mb-background"></div>
      <div class="mb"></div>
    </div>
    <div class="small-ball"></div>
    <div class="small-ball"></div>

    <div class="next"><i class="fa-solid fa-arrow-right"></i></div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.mn-container {
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1;
  gap: 0.5rem;
  margin-top: 12.5rem;
  display: flex;
  height: 2rem;
  width: 20rem;
}
.back {
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 2;
  height: 2.5rem;
  width: 2.5rem;
  border-radius: 50%;
  background: linear-gradient(
    276deg,
    rgba(255, 201, 86, 1) 32%,
    rgba(254, 215, 132, 1) 100%
  );
  font-size: 0.75rem;
  color: white;
  margin: 0.25rem;
}
.back:hover {
  cursor: pointer;
  box-shadow: 0px 0px 12px rgba(255, 197, 76, 0.9),
    0px 0px 13px rgba(255, 197, 76, 0.9);
}
.next {
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 2;
  height: 2.5rem;
  width: 2.5rem;
  border-radius: 50%;

  background: linear-gradient(
    276deg,
    rgba(254, 129, 109, 1) 0%,
    rgba(250, 79, 59, 1) 65%
  );
  font-size: 0.75rem;
  color: white;
  margin: 0.25rem;
}
.next:hover {
  cursor: pointer;
  box-shadow: 0px 0px 12px rgba(249, 75, 55, 0.9);
}

.small-ball {
  height: 0.25rem;
  width: 0.25rem;
  border-radius: 50%;
  background-color: #ffc54c;
}

.middle-ball-container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 0.5rem;
  width: 0.5rem;
  background-color: #fb604d;
  border-radius: 50%;
}

.mb-background {
  height: 0.4rem;
  width: 0.4rem;
  border-radius: 50%;
  background-color: #ffffff;
}
.mb {
  position: absolute;
  height: 0.3rem;
  width: 0.3rem;
  border-radius: 50%;
  background-color: #fb604d;
}
</style>
