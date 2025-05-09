<template>
    <div>
        <Main-PageNavbar />
        <section class="menu">
            <h1>Menu</h1>
            <div id="burgers" class="menu-category">
                <h2>Burgery</h2>
                <div class="menu-rows">
                    <div class="menu-row">
                        <div class="menu-name">Cheeseburger</div>
                        <div class="menu-description">Šťavnaté maso, domácí pečivo, sýr a jemná omáčka.</div>
                        <div class="menu-price">250 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Bacon Burger</div>
                        <div class="menu-description">Burger s křupavou slaninou a BBQ omáčkou.</div>
                        <div class="menu-price">270 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Double Cheeseburger</div>
                        <div class="menu-description">Dvojitá porce masa a sýra.</div>
                        <div class="menu-price">300 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Veggie Burger</div>
                        <div class="menu-description">Burger s grilovanou zeleninou a avokádovým dipem.</div>
                        <div class="menu-price">240 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Chili Burger</div>
                        <div class="menu-description">Pikantní burger s jalapeños a pálivou omáčkou.</div>
                        <div class="menu-price">260 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">BBQ Burger</div>
                        <div class="menu-description">Burger s BBQ omáčkou a karamelizovanou cibulkou.</div>
                        <div class="menu-price">280 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Classic Burger</div>
                        <div class="menu-description">Klasický burger s kečupem a hořčicí.</div>
                        <div class="menu-price">230 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Blue Cheese Burger</div>
                        <div class="menu-description">Burger s modrým sýrem a rukolou.</div>
                        <div class="menu-price">290 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Mushroom Burger</div>
                        <div class="menu-description">Burger s restovanými houbami a sýrem.</div>
                        <div class="menu-price">270 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Truffle Burger</div>
                        <div class="menu-description">Burger s lanýžovou omáčkou a parmazánem.</div>
                        <div class="menu-price">320 Kč</div>
                    </div>
                </div>
            </div>
            <div id="salads" class="menu-category">
                <h2>Saláty</h2>
                <div class="menu-rows">
                    <div class="menu-row">
                        <div class="menu-name">Caesar Salát</div>
                        <div class="menu-description">Čerstvá zelenina, krutony a parmazán s lehkou zálivkou.</div>
                        <div class="menu-price">180 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Řecký Salát</div>
                        <div class="menu-description">Salát s olivami, fetou a čerstvou zeleninou.</div>
                        <div class="menu-price">190 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Těstovinový Salát</div>
                        <div class="menu-description">Salát s těstovinami, kuřecím masem a pestem.</div>
                        <div class="menu-price">200 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Quinoa Salát</div>
                        <div class="menu-description">Salát s quinoou, avokádem a granátovým jablkem.</div>
                        <div class="menu-price">210 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Šopský Salát</div>
                        <div class="menu-description">Tradiční salát s rajčaty, paprikou a sýrem.</div>
                        <div class="menu-price">170 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Caprese Salát</div>
                        <div class="menu-description">Salát s mozzarellou, rajčaty a bazalkou.</div>
                        <div class="menu-price">200 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Avokádový Salát</div>
                        <div class="menu-description">Salát s avokádem, rukolou a citronovým dresinkem.</div>
                        <div class="menu-price">220 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Kuřecí Salát</div>
                        <div class="menu-description">Salát s grilovaným kuřecím masem a sezamovým dresinkem.</div>
                        <div class="menu-price">230 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Ovocný Salát</div>
                        <div class="menu-description">Salát s čerstvým ovocem a medovým dresinkem.</div>
                        <div class="menu-price">190 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Cobb Salát</div>
                        <div class="menu-description">Salát s vejcem, slaninou a avokádem.</div>
                        <div class="menu-price">240 Kč</div>
                    </div>
                </div>
            </div>
            <div id="czech" class="menu-category">
                <h2>Česká kuchyně</h2>
                <div class="menu-rows">
                    <div class="menu-row">
                        <div class="menu-name">Svíčková</div>
                        <div class="menu-description">Tradiční český pokrm s houskovým knedlíkem a omáčkou.</div>
                        <div class="menu-price">220 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Vepřo knedlo zelo</div>
                        <div class="menu-description">Vepřové maso s knedlíkem a zelím.</div>
                        <div class="menu-price">200 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Guláš</div>
                        <div class="menu-description">Hovězí guláš s domácím chlebem.</div>
                        <div class="menu-price">190 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Kachna se zelím</div>
                        <div class="menu-description">Pečená kachna s červeným zelím a knedlíkem.</div>
                        <div class="menu-price">250 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Bramborák</div>
                        <div class="menu-description">Tradiční český bramborák s česnekem.</div>
                        <div class="menu-price">150 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Španělský ptáček</div>
                        <div class="menu-description">Plněné hovězí maso s rýží.</div>
                        <div class="menu-price">230 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Moravský vrabec</div>
                        <div class="menu-description">Vepřové maso s špenátem a knedlíkem.</div>
                        <div class="menu-price">210 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Hovězí na houbách</div>
                        <div class="menu-description">Hovězí maso s houbovou omáčkou.</div>
                        <div class="menu-price">240 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Králík na smetaně</div>
                        <div class="menu-description">Králík s jemnou smetanovou omáčkou.</div>
                        <div class="menu-price">260 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Pečené koleno</div>
                        <div class="menu-description">Pečené vepřové koleno s hořčicí a křenem.</div>
                        <div class="menu-price">280 Kč</div>
                    </div>
                </div>
            </div>
            <div id="vegetarian" class="menu-category">
                <h2>Bezmasá jídla</h2>
                <div class="menu-rows">
                    <div class="menu-row">
                        <div class="menu-name">Grilovaná zelenina</div>
                        <div class="menu-description">Čerstvá grilovaná zelenina s bylinkovým dipem.</div>
                        <div class="menu-price">200 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Rizoto s houbami</div>
                        <div class="menu-description">Krémové rizoto s lesními houbami.</div>
                        <div class="menu-price">220 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Špenátové lasagne</div>
                        <div class="menu-description">Lasagne s čerstvým špenátem a ricottou.</div>
                        <div class="menu-price">240 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Cizrnový kari</div>
                        <div class="menu-description">Pikantní kari s cizrnou a kokosovým mlékem.</div>
                        <div class="menu-price">230 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Zeleninový wrap</div>
                        <div class="menu-description">Wrap plněný čerstvou zeleninou a hummusem.</div>
                        <div class="menu-price">190 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Tofu stir-fry</div>
                        <div class="menu-description">Restované tofu se zeleninou a sojovou omáčkou.</div>
                        <div class="menu-price">210 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Vegetariánská pizza</div>
                        <div class="menu-description">Pizza s čerstvou zeleninou a mozzarellou.</div>
                        <div class="menu-price">250 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Pečené brambory</div>
                        <div class="menu-description">Pečené brambory s bylinkovým máslem.</div>
                        <div class="menu-price">180 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Zeleninová polévka</div>
                        <div class="menu-description">Čerstvá zeleninová polévka s krutony.</div>
                        <div class="menu-price">150 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Falafel</div>
                        <div class="menu-description">Falafel s tahini omáčkou a pita chlebem.</div>
                        <div class="menu-price">200 Kč</div>
                    </div>
                </div>
            </div>
            <div id="desserts" class="menu-category">
                <h2>Dezerty</h2>
                <div class="menu-rows">
                    <div class="menu-row">
                        <div class="menu-name">Čokoládový dort</div>
                        <div class="menu-description">Bohatý čokoládový dort s jemným krémem.</div>
                        <div class="menu-price">150 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Jablečný štrúdl</div>
                        <div class="menu-description">Tradiční štrúdl s jablky a skořicí.</div>
                        <div class="menu-price">120 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Panna cotta</div>
                        <div class="menu-description">Jemný italský dezert s ovocnou polevou.</div>
                        <div class="menu-price">140 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Tiramisu</div>
                        <div class="menu-description">Tradiční italský dezert s mascarpone.</div>
                        <div class="menu-price">160 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Cheesecake</div>
                        <div class="menu-description">Krémový cheesecake s ovocnou polevou.</div>
                        <div class="menu-price">150 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Makronky</div>
                        <div class="menu-description">Francouzské makronky s různými příchutěmi.</div>
                        <div class="menu-price">180 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Zmrzlinový pohár</div>
                        <div class="menu-description">Zmrzlina s ovocem a šlehačkou.</div>
                        <div class="menu-price">130 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Čokoládové suflé</div>
                        <div class="menu-description">Teplý čokoládový dezert s tekutým středem.</div>
                        <div class="menu-price">170 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Ovocný koláč</div>
                        <div class="menu-description">Koláč s čerstvým ovocem a drobenkou.</div>
                        <div class="menu-price">140 Kč</div>
                    </div>
                    <div class="menu-row">
                        <div class="menu-name">Medovník</div>
                        <div class="menu-description">Tradiční medový dort s ořechy.</div>
                        <div class="menu-price">150 Kč</div>
                    </div>
                </div>
            </div>
        </section>
        <Main-PageFooter />
    </div>
</template>

<style scoped>
.menu {
    margin-top: 50px;
}

.menu-category {
    margin-top: 50px;
}

.menu-rows {
    display: flex;
    flex-direction: column;
    gap: 25px;
    margin-top: 20px;
}

.menu-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 25px;
    border-radius: 25px;
    background-color: #f9f9f9;
}

.menu-name {
    flex: 1;
    font-weight: bold;
    color: #333;
}

.menu-description {
    flex: 2;
    text-align: center;
    color: #555;
}

.menu-price {
    flex: 1;
    text-align: right;
    font-weight: bold;
    color: var(--primary-color);
}

/* Responsive styles */
@media (max-width: 800px) {
    .menu-row {
        flex-direction: column;
        align-items: flex-start;
        gap: 15px;
        padding: 25px;
    }

    .menu-name, .menu-description, .menu-price {
        flex: none;
        text-align: left;
        width: 100%;
    }

    .menu-description {
        margin-top: 5px;
        margin-bottom: 5px;
    }

    .menu-price {
        text-align: left;
        font-size: 16px;
    }
}

@media (max-width: 500px) {
h1, h2{
    margin-left: -25px;
}
    .menu-row {
        margin-right: -50px;
        margin-left: -50px;
        border-radius: 0px;
    }

    .menu-name {
        font-size: 16px;
    }

    .menu-description {
        font-size: 14px;
    }

    .menu-price {
        font-size: 14px;
    }
}
</style>
