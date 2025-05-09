<template>
  <section class="gallery">
    <h1>Galerie</h1>
    <div class="gallery-content">
      <div class="big-image" style="background-image: url('/image-90.jpeg');"></div>
      <div class="small-images">
        <div class="small-image" style="background-image: url('/image-37.png');"></div>
        <div class="small-image overlay" style="background-image: url('/image-36.png');">
          <nuxt-link to="/gallery" class="overlay-text">+19 dalších</nuxt-link>
        </div>
      </div>
    </div>
    <div class="controls">
      <nuxt-link to="/gallery" class="btn primary">Zobrazit celou galerii</nuxt-link>
    </div>
  </section>
</template>

<style setup scoped>
.gallery {
  margin-top: 50px;
}

.gallery-content {
  display: flex;
  gap: 50px;
  justify-content: space-between;
  flex-wrap: wrap;
  margin-top: 50px;
  height: 500px;
}

.big-image {
  flex: 0.7;
  height: 100%;
  background-color: #ccc;
  background-size: cover;
  background-position: center;
  border-radius: 25px;
}

.small-images {
  flex: 0.3;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 50px;
}

.small-image {
  height: 50%;
  background-color: #f16060;
  background-size: cover;
  background-position: center;
  border-radius: 25px;
}

.small-image.overlay {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  background-size: cover;
  background-position: center;
  border-radius: 25px;
}

.small-image.overlay::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(57, 88, 50, 0.8);
  border-radius: 25px;
  z-index: 1;
}

.small-image.overlay .overlay-text {
  position: relative;
  color: white;
  font-weight: bold;
  text-decoration: none;
  font-size: 18px;
  z-index: 2;
}

.controls {
  display: flex;
  justify-content: flex-start;
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

@media (max-width: 800px) {
  .gallery-content {
    flex-direction: column;
    gap: 25px;
  }

  .big-image {
    width: 100%;
    height: 300px;
  }

  .small-images {
    flex-direction: row;
    gap: 25px;
  }

  .small-image {
    width: 50%;
    height: 150px;
  }
}

@media (max-width: 500px) {
  .small-images {
    flex-direction: column;
  }

  .small-image {
    width: 100%;
  }
}
</style>