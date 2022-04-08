<template>
  <div>
    <label for="menu-toggle"><h3 style="font-weight: 400">Furniture:</h3></label>
    <input type="checkbox" id="menu-toggle" />
    <ul id="menu">
      <li id="li">
        <label for="submenu-toggle" style="font-weight: 300">Living room</label>
        <input type="checkbox" id="submenu-toggle" />
        <ul id="submenu" style="margin-top: 1rem; font-weight: 200">
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
