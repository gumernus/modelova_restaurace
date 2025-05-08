<template>
  <nav class="navbar">
    <a href="#" class="brand">Vaše Restaurace</a>
    <div class="nav-links">
      <a href="#onas" class="link">O nás</a>
      <a href="#menu" class="link">Menu</a>
      <a href="#recenze" class="link">Recenze</a>
      <a href="#galerie" class="link">Galerie</a>
      <a href="#kontakty" class="link">Kontakty</a>
      <a href="#rezervace" class="reserve-btn">
        <span class="reserve-text">Rezervovat</span>
      </a>
    </div>
  </nav>
</template>


<script lang="ts" setup>

</script>

<style setup scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  overflow: hidden;
  border-radius: 9999px;
  background-color: #395832;
  padding-left: 28px;
  padding-right: 10px;
  padding-top: 10px;
  padding-bottom: 10px;
  height: 62.5px;
}

.brand {
  font-size: 17px;
  font-weight: 300;
  color: white;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 50px;
}

.link {
  font-size: 15px;
  color: white;
}

.reserve-btn {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 10px 20px;
  border-radius: 9999px;
  background-color: #eff5e3;
  border: none;
  cursor: pointer;
  width: fit-content;
}

.reserve-text {
  font-size: 15px;
  font-weight: 600;
  color: #395832;
}

@media screen and (max-width: 820px) {
.nav-links { display: none;}
}
</style>