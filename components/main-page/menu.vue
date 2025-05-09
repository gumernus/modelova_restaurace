<template>
    <section class="menu">
        <h1>Menu</h1>
        <div class="menu-items">
            <div class="item">
                <img src="/image-30.png" alt="Burger" class="item-image" />
                <div class="item-content">
                    <h2>Burgery</h2>
                    <p>Šťavnaté maso, domácí pečivo a jemné omáčky. Naše burgery jsou vyvážené, plné chuti a podávané s
                        precizností.</p>
                    <a href="#neco" class="btn primary">Přejít na nabídku</a>
                </div>
            </div>
            <div class="item">
                <img src="/image-31.png" alt="Burger" class="item-image" />
                <div class="item-content">
                    <h2>Saláty</h2>
                    <p>Čerstvá zelenina a sezónní suroviny kombinované s lehkými zálivkami. V každém soustu najdete
                        svěžest.</p>
                    <a href="#neco" class="btn primary">Přejít na nabídku</a>
                </div>
            </div>
            <div class="item">
                <img src="/image-32.png" alt="Burger" class="item-image" />
                <div class="item-content">
                    <h2>Česká kuchyně</h2>
                    <p>Tradiční české recepty v moderním pojetí. Vychutnejte si klasiku s lehkostí a důrazem na kvalitu.
                    </p>
                    <a href="#neco" class="btn primary">Přejít na nabídku</a>
                </div>
            </div>
            <div class="item">
                <img src="/image-35.png" alt="Burger" class="item-image" />
                <div class="item-content">
                    <h2>Bezmasá jídla</h2>
                    <p>Rostlinné ingredience v nápaditých kombinacích. Bez masa, ale s plnou, vyváženou chutí, která vás
                        překvapí.</p>
                    <a href="#neco" class="btn primary">Přejít na nabídku</a>
                </div>
            </div>
            <div class="item big-item">
                <img src="/image-34.png" alt="Burger" class="item-image" />
                <div class="item-content">
                    <h2>Dezerty</h2>
                    <p>Naše dezerty jsou skutečným zážitkem pro vaše smysly. Ručně vyráběné s láskou a pozorností k
                        detailu, kombinují tradiční cukrářské techniky s moderními trendy. Čokoláda, ovoce a ořechy v
                        harmonických kombinacích, které zanechají nezapomenutelný dojem. Každý zákusek je pečlivě
                        navržen, aby zůstal v paměti a dodal vaší návštěvě sladkou tečku.</p>
                    <a href="#neco" class="btn primary">Přejít na nabídku</a>
                </div>
            </div>
        </div>
    </section>
</template>


<script lang="ts" setup>

</script>

<style setup scoped>
h1,
h2,
p {
    color: white;
}

.menu {
    padding: 50px;
    margin-left: -50px;
    margin-right: -50px;
    margin-top: 50px;
    background-color: #395832;
}

.menu-items {
    padding-top: 50px;
    display: flex;
    flex-wrap: wrap;
    gap: 50px;
}

.item {
    display: flex;
    align-items: flex-start;
    height: fit-content;
    width: calc(50% - 25px);
    gap: 50px;
    align-items: center;
}

.item-image {
    width: auto;
    height: 200px;
    width: 300px;
    object-fit: cover;
    object-position: center;
    border-radius: 25px;
}

.item-content {
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    gap: 15px;
    flex: 1;
}

.big-item {
    align-items: flex-start;
    gap: 25px;
    border-radius: 50px;
    padding: 25px;
    background-color: #eff5e3;
    width: 100%;
}

.big-item h2 {
    color: black;
}

.big-item .item-image {
    width: 500px;
    height: 300px;
}

.big-item p {
    color: #4b4b4b;
}

.big-item .btn.primary {
    background-color: #395832;
    color: #eff5e3;
}

.btn {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    padding: 10px 20px;
    border-radius: 9999px;
    text-decoration: none;
    font-size: 15px;
    font-weight: 600;
    width: fit-content;
}

.btn.primary {
    background-color: #eff5e3;
    color: #395832;
}

@media screen and (max-width: 1250px) {
    .item {

        width: 100%;
    }
}

@media screen and (max-width: 1100px) {
    .big-item {
        align-items: flex-start;
        flex-direction: column;
        margin-top: 0px;
        gap: 25px;
        padding: 50px;
        border-radius: 50px;
        background-color: #eff5e3;
        width: 100%;
    }

    .big-item .item-image {
        width: 100%;
    }
}

@media screen and (max-width: 800px) {
    .item-image {
        width: 100%;
        height: 300px;
    }

    .item {
        flex-direction: column;
    }
}
</style>