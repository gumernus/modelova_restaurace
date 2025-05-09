<template>
  <section class="contacts">
    <h1>Kontakty</h1>
    <div class="contacts-container">
      <div class="image"></div>
      <div class="content">
        <div class=column>
          <div class="field">
            <label>adresa</label>
            <p>15, Polská 160, 602 00 Brno</p>
          </div>
          <div class="field">
            <label>e-mail</label>
            <p>info@vaseresturace.cz</p>
          </div>
          <div class="field">
            <label>telefon</label>
            <p>+420 123 456 789</p>
          </div>
        </div>
        <div class=column>
          <div class="field">
            <label>otevírací doba pondělí - pátek</label>
            <p>Obědy 11:30 – 14:30</p>
            <p>Večeře: 17:30 – 22:00</p>
          </div>
          <div class="field">
            <label>otevírací doba sobota</label>
            <p>Večeře: 17:30 – 23:00</p>
          </div>
          <div class="field">
            <label>otevírací doba neděle</label>
            <p>Brunch: 10:00 – 14:00</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style setup scoped>
.contacts {
  margin-top: 50px;
}

.contacts-container {
  display: flex;
  gap: 50px;
  justify-content: space-between;
  flex-wrap: wrap;
  margin-top: 50px;
  height: 400px;
  width: 100%;
  padding: 25px;
  border: 1px solid var(--primary-color);
  border-radius: 50px;
  background-color: var(--title-color-light);;
  color: var(--text-color);
}

.image {
  flex: 0.5;
  height: 100%;
  background-image: url('/mapa.png');
  background-size: cover;
  background-position: center;
  border-radius: 25px;
}

.content {
  padding-top: 50px;
  padding-bottom: 50px;
  flex: 0.5;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 25px;
}

.column {
  width: 100%;
  display: flex;

  @media (max-width: 800px) {
    .contacts-container {
      flex-wrap: wrap;
      height: auto;
      gap: 30px;
    }

    .image {
      flex: 0.5;
      height: auto;
    }

    .content {
      flex-direction: column;
      gap: 30px;
    }

    .column {
      width: 100%;
    }
  }

  flex-direction: column;
  gap: 25px;
}

.field {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

@media (max-width: 900px) {
  .contacts-container {
    flex-wrap: wrap;
    height: auto;
    flex-direction: column;
    gap: 30px;
    align-items: center;
    /* Center items horizontally */
  }

  .image {
    flex: 0.5;
    height: auto;
  }

  .content {
    align-items: center;
    flex-direction: row;
    gap: 50px;
  }

  .column {
    width: 100%;
  }
}

@media (max-width: 600px) {
  .content {
    flex-direction: row;
    gap: 50px;
  }
}

@media (max-width: 450px) {
  .content {
    flex-direction: column;
    gap: 50px;
  }
}
</style>