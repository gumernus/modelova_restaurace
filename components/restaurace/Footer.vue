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
                    <NuxtLink to="/menu" class="link">Menu</NuxtLink>
                    <NuxtLink to="/events" class="link">Akce</NuxtLink>
                    <NuxtLink to="/contacts" class="link">Kontakt</NuxtLink>
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
                <svg><!-- Icon 1 --></svg>
                <svg><!-- Icon 2 --></svg>
                <svg><!-- Icon 3 --></svg>
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
    background-color: #395832;
    margin-left: -50px;
    margin-right: -50px;
    margin-top: 50px;
}

h1,
h2,
h3 {
    color: white
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
</style>
