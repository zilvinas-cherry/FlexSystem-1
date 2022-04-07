<template>
  <div>
    <label for="menu-toggle"><h4>Furniture:</h4></label>
    <input type="checkbox" id="menu-toggle" />
    <ul id="menu">
      <li id="li">
        <label for="submenu-toggle">Living room</label>
        <input type="checkbox" id="submenu-toggle" />
        <ul id="submenu" style="margin-top: 1rem">
          <li id="li">Sofas</li>
          <li id="li">Coffe & Tables</li>
          <li id="li">Accent Chairs</li>
          <li id="li">Ottomans & Benches</li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style>
label {
  cursor: pointer;
}

#menu-toggle {
  display: none; /* hide the checkbox */
}
#submenu-toggle {
  display: none; /* hide the checkbox */
}

#menu {
  display: none;
  margin-left: 1rem;
}

#submenu {
  display: none;
  margin-left: 1rem;
}

#menu-toggle:checked + #menu {
  display: block;
}
#submenu-toggle:checked + #submenu {
  display: block;
}

#li {
  list-style: none;
  margin-bottom: 1rem;
}
ul {
  padding: 0;
}
</style>
