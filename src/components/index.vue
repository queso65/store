<template>
  <head>
    <meta charset="utf-8" />
    <title>Store</title>
    <link rel="stylesheet" type="text/css" href="css/font-awesome.min.css" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Philosopher:ital@1&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" type="text/css" href="css/style.css" />
    <meta name="viewport" content="width=device-width" />
  </head>

  <body>
    <header class="header">
      <div class="container align-items_center">
        <a href="index.html" class="logo" title="logo">
          <img src="img/logo.png" class="img_logo" alt="Logo" />
        </a>
        <div class="header-right">
          <form class="search-form">
            <input
              type="text"
              name="id"
              value=""
              placeholder="Поиск"
              class="search search-input"
            />
            <button><i class="fa fa-search search-i"></i></button>
          </form>

          <div class="block">
            <div class="subblock">
              <div class="cart-informer">
                <button
                  class="cart-informer__button"
                  onclick="window.location.href = 'cart.html';"
                >
                  <span class="cart-informer__count" id="cart_count">5</span>
                  <span class="cart-informer__icon"
                    ><i class="fa fa-shopping-cart cart-informer__icon-i"></i
                  ></span>
                  <span class="cart-informer__value" id="cart_cost">500 ₽</span>
                </button>
              </div>

              <div class="login">
                <button
                  class="button-login"
                  onclick="window.location.href = 'login.html';"
                >
                  Вход
                </button>
              </div>
              <!--
                    <div class="dropdown">
                      <button class="dropbtn" onclick="myFunction()"> личный кабинет
                        <i class="fa fa-caret-down"></i>
                      </button>
                      <div class="dropdown-content" id="myDropdown">
                        <a href="">Перейти</a>
                        <a href="">Выход</a>
                      </div>
                    </div> 	
                    -->
            </div>
          </div>
        </div>
      </div>
    </header>

    <div class="menu">
      <div class="container">
        <div class="catalog">
          <div class="catalog__wrapper" id="catalog">
            <div class="catalog__header">
              <span>Категории</span
              ><i class="fa fa-bars catalog__header-icon"></i>
            </div>
            <ul class="catalog__list">
              <li class="catalog__item">
                <a href="" class="catalog__link">футболки</a>
              </li>
              <li class="catalog__item">
                <a href="" class="catalog__link">брелки</a>
              </li>
              <li class="catalog__item">
                <a href="" class="catalog__link">канцелярия</a>
                <div class="catalog__subcatalog">
                  <a href="" class="catalog__subcatalog-link">ручки</a>
                  <a href="" class="catalog__subcatalog-link">блокноты</a>
                </div>
              </li>
              <li class="catalog__item">
                <a href="" class="catalog__link">сумки</a>
              </li>
              <li class="catalog__item">
                <a href="" class="catalog__link">постеры</a>
              </li>
              <li class="catalog__item">
                <a href="" class="catalog__link">домашняя одежда</a>
              </li>
            </ul>
          </div>
        </div>
        <nav class="menu__nav">
          <a href="/" class="menu__nav-link">Главная</a>
          <a href="/" class="menu__nav-link">Блог</a>
        </nav>
        <a class="menu__border"></a>
      </div>
    </div>

    <h1 class="сategory">Все товары</h1>

    <!--  На одной странице по 9 товаров-->
    <div class="product-gr">
      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>

      <div class="product-item">
        <img src="img/T-shirt.jpg" />
        <div class="product-list">
          <h3 class="item_title">футболка</h3>
          <span class="price"><span class="item_price">200</span> ₽</span>
          <button data-id="" class="button add_item">В корзину</button>
        </div>
      </div>
    </div>

    <div class="pages">
      <div class="page__left"></div>
      <a data-id="" class="page page-text" href="page.html">1</a>
      <a data-id="" class="page page-text" href="page.html">2</a>
      <a data-id="" class="page page-text" href="page.html">3</a>
      <a data-id="" class="page page-text" href="last_page.html">4</a>
      <div class="page__right"></div>
    </div>

    <div class="grey__background">
      <div id="footer">
        <p>Ponyshop&trade;2023</p>
      </div>
    </div>
  </body>
</template>

<script>
</script>

<style></style>

<template>
  <div class="app">
    <h1>Страница с постами</h1>
    <input type="text" v-model="modificatorValue" />
    <my-button @click="showDialog" style="margin: 15px 0">
      Создать пост
    </my-button>
    <my-dialog v-model:show="dialogVisible">
      <post-form @create="createPost" />
    </my-dialog>
    <post-list :posts="posts" @remove="removePost" />
  </div>
</template>
    
    <script>
import PostForm from "./components/PostForm.vue";
import PostList from "./components/PostList.vue";
export default {
  components: {
    PostList,
    PostForm,
  },
  data() {
    return {
      posts: [
        { id: 1, title: "JavaScript", body: "Описание поста" },
        { id: 2, title: "JavaScript 2", body: "Описание поста 2" },
        { id: 3, title: "JavaScript 3", body: "Описание поста 3" },
        { id: 4, title: "JavaScript 4", body: "Описание поста 4" },
      ],
      dialogVisible: false,
    };
  },
  methods: {
    createPost(post) {
      this.posts.push(post);
      this.dialogVisible = false;
    },
    removePost(post) {
      this.posts = this.posts.filter((p) => p.id !== post.id);
    },
    showDialog() {
      this.dialogVisible = true;
    },
  },
};
</script>
    
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.app {
  padding: 20px;
}
</style>
    