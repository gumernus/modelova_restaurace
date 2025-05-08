<template>
  <section class="reviews">
    <h1>Recenze</h1>
    <div class="scroll-row" ref="scrollRow">

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>Jane Smith</h4>
        </div>
        <p>Restaurace je opravdu nádherná – minimalistický interiér, decentní hudba, a obsluha, která se o vás stará jako o člena královské rodiny. Jídlo bylo neskutečné – degustace 5 chodů, každý promyšlený do posledního detailu. Jen víno k rybě mi přišlo trochu nevyvážené. Jinak naprosto fantastický večer.</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>Jane Smith</h4>
        </div>
        <p>Na restauraci jsem se moc těšila, dlouho jsem si šetřila na tento večer. Interiér krásný, ale místo u kuchyně trochu rušilo atmosféru. Předkrm mě nadchnul, hlavní chod už tolik ne – maso bylo přesušené. Dezert to naštěstí zachránil. Celkově hezké, ale za ty peníze jsem čekala víc.</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>John Doe</h4>
        </div>
        <p>Skvělá atmosféra a výborné jídlo. Obsluha byla velmi přátelská a profesionální. Určitě se sem vrátím!</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>Anna Novak</h4>
        </div>
        <p>Restaurace má krásný interiér, ale jídlo mě příliš nenadchlo. Obsluha byla milá, ale čekání na hlavní chod bylo dlouhé.</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>Peter Parker</h4>
        </div>
        <p>Jídlo bylo vynikající, ale ceny jsou trochu vyšší. Celkově ale skvělý zážitek, doporučuji!</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

      <div class="card">
        <div class="profile-row">
          <img src="/image-30.png" alt="PFP">
          <h4>Emily Davis</h4>
        </div>
        <p>Úžasné místo na romantickou večeři. Jídlo bylo perfektní a obsluha velmi pozorná. Doporučuji všem!</p>
        <div class="stars-row">
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
      </div>

    </div>
    <div class="controls">
      <button class="btn primary">Zobrazit všechny recenze</button>
      <div class="arrows">
        <button class="btn secondary" @click="scrollLeft">←</button>
        <button class="btn secondary" @click="scrollRight">→</button>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const scrollRow = ref(null);

const scrollLeft = () => {
  if (scrollRow.value) {
    scrollRow.value.scrollBy({ left: -300, behavior: 'smooth' });
  }
};

const scrollRight = () => {
  if (scrollRow.value) {
    scrollRow.value.scrollBy({ left: 300, behavior: 'smooth' });
  }
};
</script>

<style scoped>
.reviews {
  margin-top: 50px;
}

.scroll-row {
  display: flex;
  overflow-x: auto;
  gap: 25px;
  margin-top: 50px;
}

.controls {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 50px;
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
  cursor: pointer;
  border: none;
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

.arrows {
  display: flex;
  gap: 10px;
}

.card {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 25px;
  padding: 25px;
  border-radius: 25px;
  text-decoration: none;
  font-size: 15px;
  background-color: #fff;
  color: #4b4b4b;
  border: 1px solid #395832;
  flex: 0 0 auto;
  min-width: 200px;
  max-width: 400px;
  height: 100%;
}

.profile-row {
  display: flex;
  align-items: center;
  gap: 15px;
}

.profile-row img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
}

.stars-row {
  display: flex;
  gap: 2px;
  color: rgb(255, 160, 16);
}

.stars-row i {
  font-size: 16px;
}
</style>
