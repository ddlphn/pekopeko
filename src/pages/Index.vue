<template>
    <Layout>
      <div class="articles-list">
          <g-link :to="post.node.path" rel="bookmark" class="article-item" v-for="post in $page.posts.edges" :key="post.id">
            <div class="article-item__text">
              <p class="article-item__date">
                <span :key="tag.id" v-for="tag in post.node.tags" class="article-item__category" :id="'color' + tag.title">{{ tag.title }}</span>
                <!-- <time :datetime="post.node.date">{{ post.node.date }}</time> -->
              </p>
              <h1 class="article-item__title">{{ post.node.title }}</h1>
              <p class="article-item__excerpt">{{ post.node.summary }}</p>
              <p class="article-item__button"><font-awesome :icon="['fa', 'eye']"/></p>
            </div>
          </g-link>
      </div>
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

export default {
  components: {
    Pager
  },
  metaInfo: {
    title: 'Articles'
  },
}
</script>

<style lang="scss">
.articles-list {
  display: flex;
  flex-wrap: wrap;
}

.article-item {
  margin-top: 1rem;
  margin-bottom: 1rem;
  border-radius: 10px;
  background: #F4F5F5;
  transition: all 0.3s;
  padding: 2rem;
  width: 26%;
  margin: 0.5rem;
  position: relative;

  @media screen and (max-width: 1130px) {
    width: 100%;
  }

  &:hover {
    background: #191F2B;
    color: white;

    .article-item__text {
      color: white;
    }

    .article-item__category {
      background: white;
      color: #191F2B;
    }
  }

  a {
    width: 100%;
    height: 100%;
  }

  &__date {
    margin: 0;
    font-size: 14px;
    font-style: italic;
  }

  &__text {
    color: #191F2B;
    transition: all 0.3s;
  }

  &__category {
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
    font-style: initial;
    transition: all 0.3s;
  }

  &__title {
    font-size: 40px;
    font-weight: 800;
    margin: 0;
    padding-top: 0.5rem;
  }

  &__excerpt {
    margin: 0;
    padding-bottom: 1rem;
  }

  &__button {
    color: white;
    background: #191F2B;
    display: inline-block;
    border-bottom-right-radius: 10px;
    border-top-left-radius: 10px;
    padding-left: 1rem;
    padding-right: 1rem;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
    margin: 0;
    position: absolute;
    bottom: 0;
    right: 0;
    transition: all 0.3s;
  }
}

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

#colorVocabulaire {
  background: #FFDE03;
  color: black;
}

#colorGrammaire {
  background: #03A9F4;
  color: white;
}

#colorConjugaison {
  background: #8BC34A;
  color: white;
}
</style>