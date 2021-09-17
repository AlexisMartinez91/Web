<template>
    <div class="entete">
        <div class="nomSite">
            <p class="titre">Nom du site</p>
        </div>
    </div>
        <div class="corps">
            <form method="POST" name="recherche" class="placeRecherche">
            </form>
            <div class="login">
                <div>
                    <p class="titreInscription">Connexion</p></br></br>
                </div>
                <form method="POST" name="Formulaire" class="formulaire">
                    <div>
                        <label for="mail">E-mail :</label>
                        <input class="champs" type="email" id="mail" name="user_mail"
                            placeholder="Francois.Dupont@gmail.com" required>
                    </div></br></br></br>
                    <div>
                        <label for="password">Mot de passe :</label>
                        <input class="champs" type="password" id="password" name="user_password"
                            placeholder="Mot de passe" required>
                    </div></br></br></br>
                    <div class="boutons">
                        <form action="AccueilConnecte.html">
                            <button class="caseBouton" type="submit">Se connecter</button>
                         </form>
                    </div></br>
                </form>
                <div class="retour">
                    <form action="AccueilConnecte.html">
                        <button class="caseBouton" type="submit">Retour au site</button>
                     </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
    body {
        background-image: url(https://www.wallpaperup.com/uploads/wallpapers/2014/03/19/302666/355c1d5fb827c8b94b37ca8e59f81a16.jpg);
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

    img {
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
        margin-top: -0px;
        margin-bottom: -0px;
        margin-left: 5px;
        margin-right: 5px;
    }

    .login {
        border-radius: 3px;
        box-shadow: black 0px 0px 5px;
        background-color: rgba(255, 255, 255, 0.8);
        width: 50%;
        margin-left: auto;
        margin-right: auto;
        margin-top: 70px;
        margin-bottom: 50px;
        padding-left: 0px;
        padding-right: 0px;
        padding-top: 15px;
        padding-bottom: 15px;

    }

    .titreInscription {
        font-size: xx-large;
        margin-left: auto;
        margin-right: auto;
        margin-top: 15px;
        margin-bottom: 30px;
        text-align: center;
        padding: 8px;
        width: 20%;
        font-weight: bolder;
    }

    .formulaire {
        padding-left: 20%;
        padding-right: 20%;
    }

    .champs {
        margin-top: 15px;
        margin-bottom: 15px;
        margin-left: auto;
        margin-right: auto;
        border: 0;
        border-bottom: 2px solid gray;
        padding: 10px;
        border-radius: 5px;
        width: 100%;
    }

    .caseBouton {
        text-transform: uppercase;
        border: 0;
        box-shadow: black 0px 0px 3px;
        padding: 5px;
        background-color: rgb(240, 240, 240);
    }
    .retour{
        margin-left: 150px;
    }
</style>