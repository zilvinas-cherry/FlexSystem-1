<template>
  <div>
    <h3 style="font-weight: 400">Style</h3>
    <ul class="style-category">
      <li class="style-item">
        <input type="checkbox" />
        <div style="margin-left: 0.5rem; display: inline">
          modern/contemporary
        </div>
      </li>
      <li class="style-item">
        <input type="checkbox" />
        <div style="margin-left: 0.5rem; display: inline">boho chic</div>
      </li>
      <li class="style-item">
        <input type="checkbox" />
        <div style="margin-left: 0.5rem; display: inline">rustic/farmhous</div>
      </li>
      <li class="style-item">
        <input type="checkbox" />
        <div style="margin-left: 0.5rem; display: inline">traditional</div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  
};
</script>

<style>
.style-category {
  display: flex;
  flex-direction: column;
  margin-right: 1rem;
  font-weight: 200;
}
.style-item {
  display: flex;
  align-items: center;
}
</style>
