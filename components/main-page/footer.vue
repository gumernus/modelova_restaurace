<template>
    <footer class="footer">
        <div class="footer-top">
            <div class="footer-column">
                <h2 class="title">Vaše Restaurace</h2>
                <p class="text">
                    Zakládáme si na precizní kuchyni, špičkovém servisu a výjimečné atmosféře, která z každé
                    návštěvy činí jedinečný zážitek.
                </p>
            </div>
            <div class="footer-links">
                <div class="link-group">
                    <h3 class="title">Rychlé odkazy</h3>
                    <NuxtLink to="#menu" class="link">Menu</NuxtLink>
                    <NuxtLink to="#recenze" class="link">Recenze</NuxtLink>
                    <NuxtLink to="#kontakty" class="link">Kontakt</NuxtLink>
                </div>
                <div class="link-group">
                    <h3 class="title">Další</h3>
                    <NuxtLink to="/privacy-policy" class="link">Ochrana osobních údajů</NuxtLink>
                    <NuxtLink to="/terms" class="link">Obchodní podmínky</NuxtLink>
                </div>
            </div>
        </div>
        <div class="footer-divider"></div>
        <div class="footer-bottom">
            <p>Vaše Restaurace © 2025 - web vytvořilo Bialu Software</p>
            <div class="footer-icons">
                <a href="https://facebook.com" target="_blank" aria-label="Facebook" class="icon-link">
                    <i class="fab fa-facebook"></i>
                </a>
                <a href="https://instagram.com" target="_blank" aria-label="Instagram" class="icon-link">
                    <i class="fab fa-instagram"></i>
                </a>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 50px;
    padding: 50px;
    background-color: var(--primary-color);
    margin-left: -50px;
    margin-right: -50px;
    margin-top: 50px;
}

h1,
h2,
h3 {
    color: var(--title-color-light);
}

p {
    color: #eff5e3;
}

.footer-top {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    width: 100%;
}

.footer-column {
    display: flex;
    flex-direction: column;
    gap: 15px;
    width: 40%;
}

.footer-links {
    display: flex;
    gap: 50px;
}

.footer-links .link-group {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.footer-links .link-group .link {
    font-size: 15px;
    color: #eff5e3;
    text-decoration: none;
}

.footer-links .link-group .link:hover {
    text-decoration: underline;
}

.footer-divider {
    width: 100%;
    height: 2px;
    background-color: rgba(255, 255, 255, 0.2);
    border-radius: 1px;
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.footer-bottom p {
    font-size: 15px;
    color: #eff5e3;
}

.footer-icons {
    display: flex;
    gap: 10px;
}

.footer-icons svg {
    width: 30px;
    height: 30px;
    fill: #eff5e3;
}

.footer-icons .icon-link {
    color: #eff5e3;
    font-size: 20px;
    text-decoration: none;
    transition: color 0.3s;
}

.footer-icons .icon-link:hover {
    color: var(--title-color-light);;
}

@media (max-width: 800px) {
    .footer-top {
        flex-wrap: wrap;
        gap: 30px;
    }

    .footer-column {
        width: 100%;
    }

    .footer-links {
        flex-wrap: wrap;
        gap: 30px;
    }

    .footer-bottom {
        flex-wrap: wrap;
        gap: 20px;
        text-align: center;
    }

    .footer-icons {
        justify-content: center;
    }
}
</style>

<script setup>
// Ensure Font Awesome is included in your project
// You can add this in your Nuxt config or directly in your HTML head:
// <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">
</script>
