<template>
    <Layout>
    <div class="single-article">
      <h1 class="single-article__title">{{ $page.post.title }}</h1>
      <!-- <p class="single-article__date">{{ $page.post.date }}</p> -->

        <div class="single-article__tags">
        <g-link
            :id="'color' + tag.title"
            v-for="tag in $page.post.tags"
            :to="tag.path"
            :key="tag.id">
          {{ tag.title }}
        </g-link>
        </div>

      <div class="markdown-body mb-8" id="article-area" v-html="$page.post.content" />

      <div class="single-article__back">
        <g-link to="/">Retour à l'accueil</g-link>
      </div>
    </div>
    </Layout>
</template>


<page-query>
query Post ($path: String!) {
  post: post (path: $path) {
    title
    date (format: "MMMM D, Y")
    content
    tags {
      title
      path
    }
  }
}
</page-query>

<script>
  export default {
  metaInfo() {
    return {
      title: this.$page.post.title
    }
  }
}
</script>

<style lang="scss">
.single-article {
  padding-bottom: 5rem;

  &__title {
    font-size: 42px;
    margin: 0;
  }

  &__tags {
    a {
      background: #F7D0E2;
      color: #99386E;
      text-transform: uppercase;
      padding-top: 0.2rem;
      padding-bottom: 0.2rem;
      padding-left: 0.8rem;
      padding-right: 0.8rem;
      font-weight: 600;
      font-size: 14px;
      border-radius: 8px;
      margin-right: 1rem;
    }
  }

  &__back {
    margin-top: 5rem;
    text-align: right;

    a {
      background: #191F2B;
      color: white;
      text-transform: uppercase;
      padding-top: 0.5rem;
      padding-bottom: 0.5rem;
      padding-left: 1rem;
      padding-right: 1rem;
      font-weight: 600;
      font-size: 15px;
      border-radius: 8px;
      margin-right: 1rem;
    }
  }
}
</style>