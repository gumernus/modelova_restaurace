<template>
    <div>
        <Main-PageNavbar />
        <section id="all-reviews" class="all-reviews">
            <h1>Všechny Recenze</h1>
            <div class="reviews-grid">
                <div class="card" v-for="(review, index) in reviews" :key="index">
                    <div class="profile-row">
                        <img :src="review.image" alt="PFP" />
                        <h4>{{ review.name }}</h4>
                    </div>
                    <p>{{ review.text }}</p>
                    <div class="stars-row">
                        <i v-for="n in review.stars" :key="n" class="fa-solid fa-star"></i>
                    </div>
                </div>
            </div>
        </section>
        <Main-PageFooter />
    </div>
</template>

<script setup>
const reviews = [
    {
        name: "Jane Smith",
        image: "/image-30.png",
        text: "Restaurace je opravdu nádherná – minimalistický interiér, decentní hudba, a obsluha, která se o vás stará jako o člena královské rodiny.",
        stars: 5,
    },
    {
        name: "John Doe",
        image: "/image-30.png",
        text: "Skvělá atmosféra a výborné jídlo. Obsluha byla velmi přátelská a profesionální. Určitě se sem vrátím!",
        stars: 5,
    },
    {
        name: "Anna Novak",
        image: "/image-30.png",
        text: "Restaurace má krásný interiér, ale jídlo mě příliš nenadchlo. Obsluha byla milá, ale čekání na hlavní chod bylo dlouhé.",
        stars: 4,
    },
    {
        name: "Peter Parker",
        image: "/image-30.png",
        text: "Jídlo bylo vynikající, ale ceny jsou trochu vyšší. Celkově ale skvělý zážitek, doporučuji!",
        stars: 4,
    },
    {
        name: "Emily Davis",
        image: "/image-30.png",
        text: "Úžasné místo na romantickou večeři. Jídlo bylo perfektní a obsluha velmi pozorná. Doporučuji všem!",
        stars: 5,
    },
];
</script>

<style scoped>
.all-reviews {
    margin-top: 50px;
}

.reviews-grid {
    margin-top: 50px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
}

.card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    gap: 25px;
    padding: 25px;
    border-radius: 25px;
    background-color: #fff;
    color: #4b4b4b;
    border: 1px solid #395832;
    flex: 0 0 auto;
    min-width: 200px;
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

.card h4 {
    margin: 0;
    font-size: 18px;
    color: #333;
}

.card p {
    margin: 0;
    font-size: 14px;
    color: #555;
}

.stars-row {
    display: flex;
    gap: 2px;
    color: rgb(255, 160, 16);
}

.stars-row i {
    font-size: 16px;
}

@media (max-width: 800px) {
    .reviews-grid {
        grid-template-columns: repeat(2, 1fr);
        /* 2 reviews per row for medium devices */
    }
}

@media (max-width: 650px) {
    .reviews-grid {
        grid-template-columns: 1fr;
        /* 1 review per row for small devices */
    }
}
</style>
