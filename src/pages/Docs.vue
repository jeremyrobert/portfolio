<template>
  <Layout>
    <div class="container-inner mx-auto py-16">
      <h2 class="text-4xl font-bold mb-16">En construction</h2>
      <img src="../../static/work_in_progress.svg" alt="En construction" />
      <!-- <div v-for="doc in $page.docs.edges" :key="doc.id" class="post border-gray-400 border-b mb-12">
        <h2 class="text-3xl font-bold"><g-link :to="doc.node.path" class="text-copy-primary">{{ doc.node.title }}</g-link></h2>

        <div class="text-lg mb-4">
          {{ doc.node.excerpt }}
        </div>

        <div class="mb-8">
          <g-link :to="doc.node.path" class="font-bold uppercase">Read More</g-link>
        </div>
      </div>-->
    </div>
  </Layout>
</template>

<page-query>
query Documentation {
  docs: allDocumentation (sortBy: "date", order: DESC) {
    edges {
      node {
        id
        path
        title
        excerpt
      }
    }
  }
}
</page-query>

<script>
export default {
  metaInfo: {
    title: "Docs"
  }
};
</script>
