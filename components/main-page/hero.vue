<template>
  <section class="hero">
    <div class="hero-content">
      <div class="hero-text">
        <h1>Poznejte nový kulinářský zážitek</h1>
        <p>
          Objevte místo, kde se precizní řemeslo snoubí s výjimečnými surovinami. Dopřejte si večer,
          který potěší všechny smysly v prostředí, kde každý detail hovoří o eleganci.
        </p>
        <div class="buttons">
          <a href="#rezervace" class="btn primary">Rezervovat</a>
          <a href="#kontakt" class="btn secondary">Kontaktovat</a>
        </div>
      </div>
      <div class="hero-image"></div> <!-- Zmizelo <img>, máme jen div -->
    </div>
    <div class="opening-hours">
      <div class="card">
        <h2>Pondělí až pátek</h2>
        <p>Obědy 11:30 – 14:30</p>
        <p>Večeře: 17:30 – 22:00</p>
      </div>
      <div class="card">
        <h2>Sobota</h2>
        <p>Večeře: 17:30 – 22:00</p>
      </div>
      <div class="card">
        <h2>Neděle</h2>
        <p>Brunch: 10:00 – 14:00</p>
      </div>
    </div>
  </section>
</template>

<style setup scoped>
.hero {
  display: flex;
  flex-direction: column;
  gap: 50px;
  padding-top: 200px;
}

.hero-content {
  display: flex;
  gap: 50px;
  justify-content: space-between;
  padding-bottom: 200px;
  flex-wrap: wrap;
}

.hero-text {
  display: flex;
  flex-direction: column;
  gap: 25px;
  padding: 50px 0;
  flex: 0.4;
}

.hero-image {
  flex: 0.6; 
  border-radius: 25px;
  background: url('/image-23.png') no-repeat center center;
  background-size: cover;
  min-height: 400px;
}

.buttons {
  display: flex;
  gap: 25px;
}

.btn {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 10px 20px;
  border-radius: 9999px;
  text-decoration: none;
  font-size: 15px;
  font-weight: 600;
}

.btn.primary {
  background-color: #395832;
  color: #eff5e3;
}

.btn.secondary {
  background-color: #eff5e3;
  color: #395832;
  border: 1px solid #395832;
}

.opening-hours {
  display: flex;
  flex-wrap: wrap;
  gap: 50px;
}

.card {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 25px;
  padding: 50px;
  border-radius: 25px;
  background-color: white;
  border: 1px solid #395832;
  min-width: 260px;
}

@media (max-width: 800px) {
  .hero-content {
    flex-direction: column;
  }

  .hero-image {
    min-height: 300px;
  }
}
</style>
