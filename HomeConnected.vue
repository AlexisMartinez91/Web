<template>
    <div class="entete">
        <div class="nomSite">
            <p class="titre">Nom du site</p>
        </div>
        <div class="bouton">
            <form action="Accueil.html">
                <button class="caseBouton" type="submit">Déconnexion</button>
             </form>
             <form action="Tableaux.html">
                <button class="caseBouton" type="submit">Tableaux</button>
             </form>
        </div>
    </div>
    <div class="Page">
        <div class="listeInstruments">
            <p class="mesInstrumentsTexte">Instruments disponible</p>
            <ul>
                <li>Saxophones</li>
                <li>Guitares</li>
                <li>Basses</li>
                <li>Flûtes</li>
                <li>Pianos</li>
                <li>Trompettes</li>
                <li>Violons</li>
                <li>Contrebasses</li>
                <li>Percussions</li>
                <li>Amplis</li>
                <li>Sampleurs</li>
                <li>etc...</li>
            </ul>
        </div>
        <div class="corps">
            <form method="POST" name="recherche" class="placeRecherche">
                <div class="recherche">
                    <input class="recherche" type="search" id="instrument" name="recherche"
                        placeholder="Que recherchez-vous ? ..." required>
                </div>
                <div class="boutonRecherche">
                    <button class="boutonRecherche" id="trouve" onclick="rechercher()"><img class="imgRecherche"
                            src="https://image.flaticon.com/icons/png/512/116/116836.png"></button>
                </div>
            </form>
            <div class="présentation">
                <p>Avec notre site, créer les instruments qui vous ressemble afin 
                    d'avoir un style incroyable</br> Avec notre partenaire Woodbras, la référence en terme de musique,
                    soyez sûre d'avoir toujours le meilleur matériel et de toujours rester au top !!!</p>
            </div></br></br></br>
            <div class="articleune">
                <p>Articles à la une</p>
            </div>
            <div class="article">
                <div class="image">
                    <img class="imgArticle"
                        src="https://www.woodbrass.com/images/SQUARE400/woodbrass/CORT+E70OP.JPG">
                </div>
                <div class="texteArticle">
                    <div class="titreArticle">
                        <p>CORT EARTH70 NATURAL OPEN PORES</p>
                    </div>
                    <div>
                        <p>Table Massive en Epicéa de Sitka; Dos et Eclisses en Acajou; Frettes 20; Diapason 643mm (25.3"); Cordes D'Addario EXP16 Strings</p>
                    </div>
                </div>
                <div class="actions">
                    <div>
                        <p>198.00€</p>
                    </div>
                    <div>
                        <p><a href="https://www.woodbrass.com/guitares-acoustiques-folk-cort-earth70-natural-open-pores-p210296.html">Lien</a></p>
                    </div>
                </div>
            </div>
            <div class="article">
                <div class="image">
                    <img class="imgArticle"
                        src="https://www.woodbrass.com/images/SQUARE400/woodbrass/VOX+MVO+VT40X.JPG">
                </div>
                <div class="texteArticle">
                    <div class="titreArticle">
                        <p>VOX VT40X</p>
                    </div>
                    <div>
                        <p>11 modélisations d’ampli; 10 effets personalisables; Préampli: Valve Reactor avec lampe 12AX7; Puissance: 40 Watts RMS; Haut-parleur:1x10 5 ohms</p>
                    </div>
                </div>
                <div class="actions">
                    <div>
                        <p>215.00€</p>
                    </div>
                    <div>
                        <p><a href="https://www.woodbrass.com/combos-guitare-a-modelisation-vox-vt40x-p214755.html">Lien</a></p>
                    </div>
                </div>
            </div>
            <div class="article">
                <div class="image">
                    <img class="imgArticle"
                        src="https://www.woodbrass.com/images/SQUARE400/woodbrass/3YAMAHA+NP12+BK.JPG">
                </div>
                <div class="texteArticle">
                    <div class="titreArticle">
                        <p>YAMAHA NP-12 BK</p>
                    </div>
                    <div>
                        <p>Fonction Dual/Layer; Métronome; Accordement possible; Alimentation 12V ou piles; Autonomie sur piles de 6 heures; USB ; Inclus Pupitre</p>
                    </div>
                </div>
                <div class="actions">
                    <div>
                        <p>229.00€</p>
                    </div>
                    <div>
                        <p><a href="https://www.woodbrass.com/claviers-%20-pianos-arrangeurs-yamaha-np-12-bk-p217021.html">Lien</a></p>
                    </div>
                </div>
            </div>
            <div class="article">
                <div class="image">
                    <img class="imgArticle"
                        src="https://www.woodbrass.com/images/SQUARE400/woodbrass/1NI+MASCHINE+MK3.JPG">
                </div>
                <div class="texteArticle">
                    <div class="titreArticle">
                        <p>NATIVE INSTRUMENTS MASCHINE MK3</p>
                    </div>
                    <div>
                        <p>Bibliothèque KOMPLETE 13 SELECT de 25 Go; 16 pads ultra-sensibles; Alimention USB 2.0 ou bloc d'alimentation secteur; Compatible MAC et Windows</p>
                    </div>
                </div>
                <div class="actions">
                    <div>
                        <p>545.00€</p>
                    </div>
                    <div>
                        <p><a href="https://www.woodbrass.com/synthes-groovebox-%20-samplers-native-instruments-maschine-mk3-p254708.html">Lien</a></p>
                    </div>
                </div>
            </div>

        </div>
        <div class="listeTableau">
            <p class="mesTableauxTexte"> Mes tableaux</p>
        </div>
    </div>
</template>

<script>
    function rechercher() {
        var rechercher = document.getElementById("instrument").value;
        var tab = rechercher.split(" ");
        var instrument = ""
        for (com in tab) {
            if (com == tab.length - 1) {
                instrument += tab[com]
            }
            else {
                instrument += tab[com] + "+";
            }
        }
        window.open("https://woodbrass.com/" + instrument);

    };
</script>

<style scoped>
    body {
        background-image: url(https://image.winudf.com/v2/image1/Y29tLmFwcDNkd2FsbHBhcGVyaGQuZ3VpdGFyd2FsbHBhcGVyX3NjcmVlbl81XzE1NjcwMjUxODRfMDUw/screen-5.jpg?fakeurl=1&type=.jpg);
        background-attachment: fixed;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
    }

    .entete {
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgb(255, 255, 255, 0.8);
        display: flex;
        flex-wrap: wrap;
    }

    .entete>* {
        flex: 1 1 0;
    }

    .Page {
        display: flex;
        flex-wrap: wrap;
    }

    .listeInstruments {
        flex: 1 1 0;
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgb(255, 255, 255, 0.8);
        margin-top: 10px;
        padding: 5px;
    }

    .corps {
        flex: 4 1 0;
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgb(255, 255, 255, 0.5);
        margin: 10px;
        padding: 5px;
        padding-bottom: 300px;
    }

    .listeTableau {
        flex: 1 1 0;
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgb(255, 255, 255, 0.8);
        margin-top: 10px;
        padding: 5px;
    }

    .recherche {
        width: 100%;
        padding: 10px;
        font-size: 20px;
        background-color: rgb(228, 220, 255);
        border: 0;
        flex: 7 1 0;
    }

    .placeRecherche {
        width: 60%;
        margin-left: auto;
        margin-right: auto;
        margin-top: 50px;
        display: flex;
        flex-wrap: wrap;
        box-shadow: black 0px 0px 5px;
        border-radius: 3px;
    }

    .boutonRecherche {
        width: fit-content;
        border: 0;
        background: none;
        flex: 1 1 0;
        background-color: rgb(228, 220, 255);
        cursor: pointer;
    }

    .imgRecherche {
        width: 45px;
        height: 45px;
        margin-top: 10px;
    }

    .nomSite {
        max-width: max-content;
        box-shadow: black 0px 0px 5px;
        background-color: white;
        border-radius: 3px;
        margin: 10px;
    }

    .bouton>* {
        flex: 1 1 0;
    }

    .bouton {
        margin: 10px;
        margin-left: auto;
        padding: 5px;
        max-width: max-content;
        display: flex;
        flex-wrap: wrap;
    }

    button {
        margin-left: 5px;
        margin-right: 5px
    }

    .titre {
        font-size: 200%;
        margin-top: 5px;
        margin-bottom: -0px;
        margin-left: 5px;
        margin-right: 5px;
    }

    .mesInstrumentsTexte {
        font-size: 150%;
        margin-top: -0px;
        margin-bottom: -0px;
        margin-left: 5px;
        margin-right: 5px;
    }

    .mesTableauxTexte {
        font-size: 150%;
        margin-top: -0px;
        margin-bottom: -0px;
        margin-left: 5px;
        margin-right: 5px;
        text-align: center;
    }

    .présentation {
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgba(255, 255, 255, 0.8);
        width: 80%;
        margin-left: auto;
        margin-right: auto;
        margin-top: 50px;
        margin-bottom: 20px;
        padding: 20px;
        text-align: justify;
    }

    .article {
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: white;
        width: 90%;
        margin-left: auto;
        margin-right: auto;
        margin-top: 20px;
        margin-bottom: 20px;
        padding: 5px;
        display: flex;
        flex-wrap: wrap;
    }

    .imgArticle {
        width: 192px;
        height: 108px;
        border-radius: 3px;
        display: block;
        box-shadow: black 0px 0px 5px;
    }

    .image {
        flex: 1 1 0;
    }

    .texteArticle {
        flex: 3 1 0;
        padding-left: 10px;
    }

    .actions {
        flex: 1.5 1 0;
        display: flex;
        flex-wrap: wrap;
        padding: 10px;
    }

    .actions>* {
        flex: 1 1 0;
        margin: auto;
    }

    .ajouterA>* {
        margin: 5px;
        box-shadow: black 0px 0px 3px;
    }

    .titreArticle {
        font-size: large;
    }

    .caseBouton {
        text-transform: uppercase;
        border: 0;
        box-shadow: black 0px 0px 3px;
        padding: 5px;
        background-color: rgb(240, 240, 240);
        text-align: center;
    }
    .articleune {
        text-align: center;
        font-size: x-large;
        font-weight: bolder;
    }
</style>