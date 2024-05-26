<template>
<div class="container">
    <h2>Misolo Project</h2>
    <p>
      Misolo is a brand committed to <strong>social aid</strong>, that's why we want you to know and help us with our Misolo project. Some of our measures are to allocate <strong>5% of our profits</strong> to a humanitarian aid project in Angola. <strong>Each order is help.</strong> We provide our help through <strong>Misevi</strong>, which has communities in <strong>Bolivia and Angola</strong>. Although we collaborate with microprojects such as "Nutritional supplement for children" or "training and promotion of Angolan women" in Angola.
    </p>
    <p>
      Its presence in Angola is located in Lobito, among the Umbundu people. Its actions are especially linked to working women, early childhood and alcoholic patients. Two fundamental axes of its action are community intervention and the training of social agents. A great challenge in its reality is the young people, the immediate future of that welcoming and happy town.
    </p>
    <p>
      MISEVI is an ONGD oriented towards the human promotion of people, the fight against poverty and active commitment to the context of social exclusion that occurs in the countries where the Association is present. We are very proud of our small collaboration with them, and by purchasing our products, you can also participate in this Misolo Project.
    </p>
    <img src="../assets/project.png" alt="Productos de Misolo" class="image">
    <p>Thank You</p>
    <p>Inola Afdholiana-223510839</p>
</div>
</template>

<script>
  import { RouterLink } from 'vue-router';

  export default {
    name: 'Project',
    components: {
      RouterLink
    }
  };
</script>

<style scoped>
 .container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    font-family: Arial, sans-serif;
    color: #333;
    line-height: 1.6;
  }

h2 {
  color: #333;
}

h2 {
  font-size: 30px;
  margin-top: 60px;
  font-weight: bold;
  margin-bottom: 20px;
}

p {
  font-size: 18px;
  margin-bottom: 20px;
  text-align: justify;
}

strong {
  font-weight: bold;
}

.image {
  width: 100%;
  height: 400px;
  border-radius: 8px;
  margin-top: 20px;
}
</style>