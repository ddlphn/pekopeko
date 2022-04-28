<template>
    <Layout>
      <PostBlog />
      <Pager :info="$page.posts.pageInfo" class="pagination"/>
  </Layout>
</template>

<page-query>
query Posts ($page: Int) {
  posts: allPost (sortBy: "date", order: DESC, perPage: 8, page: $page) @paginate {
    totalCount
    pageInfo {
      totalPages
      currentPage
    }
    edges {
      node {
        id
        title
        date (format: "MMMM Y")
        summary
        path
        tags {
          title
          path,
        }
      }
    }
  }
}
</page-query>

<script>
import { Pager } from 'gridsome'
import PostBlog from '~/components/PostBlog.vue'

export default {
  components: {
    Pager,
    PostBlog,
  },
  metaInfo: {
    title: 'Accueil'
  },
}
</script>

<style lang="scss">
.pagination {
  text-align: center;
  padding-top: 2rem;
  padding-bottom: 2rem;

  a {
    margin-left: 0.5rem;
    margin-right: 0.5rem;
    display: inline-block;
    width: 25px;
    height: 25px;
    border-radius: 50%;

    &.active {
      background-color: white;
      color: #0d2538;
    }
  }
}
</style>