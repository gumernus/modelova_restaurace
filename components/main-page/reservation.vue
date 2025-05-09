<script setup>
import { ref } from 'vue';

const formData = ref({
  fullname: '',
  guests: '',
  date: '',
  time: '',
  email: '',
  phone: '',
  note: ''
});

const confirmationMessage = ref('');

const handleSubmit = () => {
  const reservationData = {
    fullname: formData.value.fullname.trim(),
    guests: parseInt(formData.value.guests, 10),
    date: formData.value.date,
    time: formData.value.time,
    email: formData.value.email.trim(),
    phone: formData.value.phone.trim(),
    note: formData.value.note.trim()
  };

  console.log('Reservation Data:', reservationData);

  // Show confirmation message
  confirmationMessage.value = 'Rezervace byla úspěšně odeslána.';

  // Clear form data
  formData.value = {
    fullname: '',
    guests: '',
    date: '',
    time: '',
    email: '',
    phone: '',
    note: ''
  };

  // Hide confirmation message after 5 seconds
  setTimeout(() => {
    confirmationMessage.value = '';
  }, 5000);
};
</script>

<template>
  <section class="reservation">
    <h1>Rezervace</h1>
    <div class="reservation-container">
      <div class="img"></div>
      <div class="content">
        <form @submit.prevent="handleSubmit">
          <div class="row" style="margin-bottom: 25px;">
            <div class="field">
              <label for="fullname">*celé jméno</label>
              <input type="text" id="fullname" name="fullname" v-model="formData.fullname" placeholder="Jan Novák">
            </div>
            <div class="field" style="width: 100px;">
              <label for="guests">*počet osob</label>
              <input type="number" id="guests" name="guests" v-model="formData.guests" placeholder="4" min="1">
            </div>
          </div>
          <div class="row" style="margin-bottom: 25px;">
            <div class="field">
              <label for="date">*datum</label>
              <input type="date" id="date" name="date" v-model="formData.date">
            </div>
            <div class="field">
              <label for="time">*čas</label>
              <input type="time" id="time" name="time" v-model="formData.time">
            </div>
          </div>
          <div class="row" style="margin-bottom: 25px;">
            <div class="field" style="width: 100%;">
              <label for="email">email</label>
              <input type="email" id="email" name="email" v-model="formData.email" placeholder="jan.novak@gmail.com">
            </div>
            <div class="field" style="width: 100%;">
              <label for="phone">telefonní číslo</label>
              <input type="tel" id="phone" name="phone" v-model="formData.phone" placeholder="+420 123 456 789">
            </div>
          </div>
          <div class="row" style="margin-bottom: 25px;">
            <div class="field poznamka" style="width: 100%;">
              <label for="note">poznámka</label>
              <textarea id="note" class="poznamka" name="note" v-model="formData.note" placeholder="Toto je text poznámky"></textarea>
            </div>
          </div>
          <div class="row" style="align-items: center;">
            <div class="field">
              <button type="submit" class="btn primary">Odeslat rezervaci</button>
            </div>
            <p v-if="confirmationMessage" style="margin-left: 15px;">{{ confirmationMessage }}</p>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<style setup scoped>
.reservation {
  margin-top: 50px;
}

.reservation-container {
  display: flex;
  flex-direction: row;
  align-items: stretch;
  flex-wrap: wrap;
  gap: 50px;
  margin-top: 50px;
  margin-bottom: 50px;
}

.content {
  display: flex;
  flex-direction: column;
  flex: 0.5;
  gap: 25px;
  max-width: 60%;
}

.row {
  display: flex;
  flex-direction: row;
  gap: 25px;
  flex-wrap: wrap; /* Allow wrapping for better responsiveness */
}

.field {
  display: flex;
  flex-direction: column;
  gap: 15px;
  min-width: 100px;
  flex: 1; /* Allow fields to grow and shrink */
}

.img {
  flex: 0.5;
  border-radius: 25px;
  background: url("/image-23.png") no-repeat center center;
  background-size: cover;
  min-height: 300px; /* Ensure a minimum height for better layout */
}

input {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 10px 20px;
  border-radius: 9999px;
  text-decoration: none;
  font-size: 15px;
  background-color: var(--title-color-light);;
  color: var(--text-color);
  border: 1px solid var(--primary-color);
}

.field.poznamka textarea {
  width: 100%;
  height: 150px;
  padding: 16px;
  border: 1px solid var(--primary-color);
  border-radius: 25px;
  font-size: 15px;
  line-height: 1.5;
  resize: none;
  background-color: var(--title-color-light);;
  color: var(--text-color);
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
  width: fit-content; /* Adjust width to fit content like other buttons */
  justify-content: center;
}

.btn.primary {
  background-color: var(--primary-color);
  color: #eff5e3;
}

.confirmation-message {
  margin-top: 20px;
  color: green;
  font-weight: bold;
  text-align: center;
}

@media (max-width: 800px) {
  .reservation-container {
    flex-direction: column;
    gap: 30px; /* Reduce gap for smaller screens */
  }
  
  .content {
    width: 100%;
    max-width: 100%; /* Ensure content takes full width */
  }

  .img {
    min-height: 200px; /* Adjust minimum height for smaller screens */
  }

  .row {
    flex-direction: column; /* Stack fields vertically */
    gap: 15px; /* Reduce gap between fields */
  }

  .field {
    width: 100%; /* Ensure fields take full width */
  }
}

@media (max-width: 500px) {
  .btn {
    font-size: 13px; /* Adjust button font size for very small screens */
    padding: 8px 16px; /* Adjust padding for buttons */
  }

  input, textarea {
    font-size: 13px; /* Adjust input and textarea font size */
    padding: 8px 16px; /* Adjust padding for inputs */
  }
}
</style>