<template>
  <section class="gallery">
    <h1>Galerie</h1>
    <div class="gallery-content">
      <div class="big-image" style="background-image: url('/image-23.png');"></div>
      <div class="small-images">
        <div class="small-image" style="background-image: url('/image-30.png');"></div>
        <div class="small-image" style="background-image: url('/image-31.png');"></div>
      </div>
    </div>
    <div class="controls">
      <button class="btn primary">Zobrazit celou galerii</button>
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
  gap: 25px;
}

.small-image {
  height: 50%;
  background-color: #f16060;
  background-size: cover;
  background-position: center;
  border-radius: 25px;
}

.controls {
  display: flex;
  justify-content: flex-start; /* Align to the left */
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
    gap: 30px;
  }

  .big-image {
    width: 100%;
    height: 300px;
  }

  .small-images {
    flex-direction: row;
    gap: 15px;
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