<template>
  <store-header></store-header>
  <store-catalog></store-catalog>

  <h1 class="сategory">Все товары</h1>

  <!--  На одной странице по 9 товаров-->
  <store-list :posts="posts[page]" @remove="removePost" />

  <store-numberpages
    :totalPages="numberPages()"
    @changePage="changePage"
  ></store-numberpages>

  <store-footer></store-footer>
</template>
  
  <script>
import StoreList from "@/components/StoreList.vue";
import StoreHeader from "@/components/StoreHeader.vue";
import StoreCatalog from "@/components/StoreCatalog.vue";
import StoreFooter from "@/components/StoreFooter.vue";
import StoreNumberpages from "@/components/StoreNumberpages.vue";
export default {
  components: {
    StoreList,
    StoreHeader,
    StoreCatalog,
    StoreFooter,
    StoreNumberpages,
  },
  data() {
    return {
      posts: [
        [
          {
            id: 1,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 2,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 3,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 4,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 5,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 6,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 7,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 8,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 9,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
        ],
        [
          {
            id: 10,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 11,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 12,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
          {
            id: 13,
            img: require("../assets/img/T-shirt.jpg"),
            title: "футболка",
            price: "200",
          },
        ],
      ],
      page: 0,
      limit: 9,
      totalPages: 0,
    };
  },
  methods: {
    removePost(post) {
      this.posts = this.posts.filter((p) => p.id !== post.id);
      this.numberPages();
    },
    numberPages() {
      this.totalPages = Math.ceil(this.posts.length / this.limit);
      return this.totalPages;
    },
    changePage(page) {
      this.page = page - 1;
    },
  },
};
</script>
  
  <style>
.сategory {
  font-family: "Philosopher", sans-serif;
  text-align: center;
  color: #a53bcc;
  font-size: 28px;
}
</style>