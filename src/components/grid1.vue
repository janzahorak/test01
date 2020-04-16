<template>
  <div class="grid1">
      <div class="grid1__item grid1__item--center">
          <div class="grid1__wrapper">
            <h3>Společná cesta</h3>
            <p>Společná cesta začíná v roce 2017, kdy při návštěvě New Yorku v létě téhož roku zabloudí do nejlepší mexické taqueríi ve městě. Jednoduchost, rychlost, čerstvost a především pravé mexické chutě jim dávají brouka do hlavy. O rok později při druhé návštěvě New Yorku je tato mexická taquería nevyhnutelnou zastávkou a z brouka se stává plán otevřít v Praze vlastní mexické bistro. Možná tak chtěl osud či hvězdy, ale po návratu z USA zjistili, že v Lidické ulici se opravuje dům, který by byl ideálním místem pro jejich nové bistro. Po roční práci bylo bistro v prosinci 2019 dokončeno a s nedočkavostí se těší na otevření v lednu 2020.</p>
          </div>
      </div>
      <div class="grid1__item grid1__item--images">
          <img class="grid1__image" src="../assets/img1.png" />
          <img class="grid1__image" src="../assets/img1.png" />
      </div>
  </div>
</template>

<script>
export default {
  name: 'Grid1'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.grid1 {
    display: flex;
}

.grid1__item {
    flex: 0 0 50%;
    max-width: 50%;
    text-align: left;
}

.grid1__item--center {
    display: flex;
    align-items: center;
    position: relative;
}

.grid1__item--center:before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 10px;
    bottom: 0;
    background-color: #f3f3f3;
    z-index: -1;
}

.grid1__item--images {
    display: flex;
}

.grid1__wrapper {
    padding: 40px;
}

.grid1__image {
    flex: 0 0 50%;
    max-width: 50%;
}

h3 {
    font-size: 32px;
}

</style>
