<script setup>
import CFantome from "../src/components/CFantome.vue";
import CGrille from "../src/components/CGrille.vue";
import CPacMan from "../src/components/CPacman.vue";
import Pacman from "../src/components/Pacman.vue";
export default {
  components: { CFantome, CGrille, CPacMan, Pacman },
};
</script>

<template>
  <section>
    <p id="score">Score :</p>
    <p id="sens">Sens Pacman :</p>
    <h1>Pacman</h1>
    <div id="grille"></div>
    <CFantome />
    <CGrille />
    <CPacMan />
    <Pacman />
  </section>
</template>

<style scoped>
h1 {
  display: flex;
  justify-content: center;
}
#grille {
  display: grid;
  margin-left: 150px;
  margin-top: 5%;
}
.mur {
  background-image: url(./images/murbrique.jpg);
}
.sol {
  background-color: black;
}
.bonbon {
  background-image: url(./images/bonbon.gif);
}
.pacman {
  background-image: url(./images/pacman4.gif);
}
.fantome {
  background-image: url(./images/fantome_bleu1.gif);
}
.fantome-bleu {
  background-image: url(../images/fantome_bleu1.gif);
}
.fantome-rouge {
  background-image: url(./images/fantome_rouge1.gif);
}
.fantome-orange {
  background-image: url(./images/fantome_orange1.gif);
}
.fantome-vert {
  background-image: url(./images/fantome_vert1.gif);
}
p {
  font-size: 1.6em;
}
</style>
