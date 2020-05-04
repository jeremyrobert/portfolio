<template>
  <Layout>
    <div class="container-inner mx-auto py-16">
      <h2 class="text-4xl font-bold">Mince ! Cette page n'existe pas ?!</h2>
      <g-link to="/" class="border-none">
        <p class="text-4xl mb-16">Retour</p>
      </g-link>
      <img src="../../static/404.svg" alt="404 page non trouvée" />
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Page Not Found"
  }
};
</script>
