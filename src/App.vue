<template>
  <div id="app">
    <!-- <h1>Benvenuto</h1>
    <p>Daje</p> -->
    <AppHeader />
    <main>
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque
      laborum excepturi reprehenderit ut dolore ad. Quae, excepturi? Voluptatem
      porro saepe delectus provident fugit nemo sit voluptatum optio rem nisi
      deleniti accusantium, consequuntur, temporibus dicta consequatur.
      Exercitationem, quo itaque accusamus officia omnis reprehenderit inventore
      doloribus laborum natus tempore fuga nobis aliquid in dolor minus est
      quos. Quia dolor necessitatibus consectetur molestias modi ullam nulla
      quas quis impedit minus neque temporibus sequi pariatur, aperiam laborum
      fuga expedita est error magni repudiandae iste eius amet nobis possimus.
      Delectus atque laboriosam blanditiis, aperiam nobis voluptatibus dicta
      error nemo et inventore, voluptatum dolorem. Rem et at ex atque vel iusto
      distinctio ea, necessitatibus vitae ipsum, placeat, saepe totam voluptate
      odio quas laboriosam illo quasi dignissimos deleniti sit itaque rerum
      illum. Harum, ipsum quo maiores unde quam ratione similique velit aliquid
      aspernatur magni sunt atque tempore qui et ullam totam! Error nulla ad,
      sint voluptatum alias perspiciatis? In voluptatum natus a nesciunt. Itaque
      sequi autem quidem exercitationem nostrum! Et provident mollitia quae
      error recusandae quod nobis magni at iure, obcaecati repellat maxime
      dolore, aliquid, omnis numquam iusto? Nihil, incidunt veritatis. Iusto
      animi ipsum placeat laborum cum repudiandae, repellendus, quos neque,
      explicabo est eaque maiores esse atque debitis voluptates nemo cupiditate
      eius doloribus soluta. Sit pariatur ullam cupiditate mollitia, provident
      quidem repellendus temporibus rerum officia debitis laudantium
      reprehenderit itaque unde consequuntur, a sequi? Voluptatibus fugit
      laborum sequi! Veritatis dolor cupiditate in possimus! Non rem alias ipsam
      illo ipsa. Officiis, esse? Totam eum ab cupiditate iure eius mollitia
      harum est temporibus iusto dignissimos? Architecto temporibus, obcaecati
      harum aperiam debitis officia voluptate nulla corporis error voluptas quis
      fugiat sunt libero dolores, ex dolorem animi ratione quasi ducimus quidem
      amet molestiae explicabo. Tempora, error laudantium similique aliquid sunt
      maxime illum, aut, sed suscipit officia eligendi temporibus architecto.
      Veritatis fuga maxime ex accusamus illo dolor quae alias, beatae quam
      assumenda quos voluptates fugit, dignissimos aut eum velit minima esse
      aspernatur omnis vitae suscipit perspiciatis quis nihil. Ratione, porro
    </main>
    <AppUpperFooter />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppUpperFooter from "./components/AppUpperFooter.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppUpperFooter,
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general.scss";
main {
  margin-top: 100px;
  background-color: yellow;
  width: 100%;
}
</style>
