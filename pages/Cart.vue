<template>
    <div class="container">
      <h1 class="list-title">카트 페이지입니다!!</h1>
      <CartList></CartList>
      <div class="extra-panel">
        <button>구매하기!!!</button>
      </div>
      <div class="cart-wrapper">
        <button class="btn" @click="buyThing">구매하기</button>
        <button class="btn" @click="clearThing">장바구니 비우기</button>
      </div>
    </div>
  </template>
  
  <script>
  // import { FETCH_CART_ITEMS} from '@/store'
  import CartList from '~/components/CartList.vue'
  
  export default {
    components: { CartList },
    // async asyncData({ store }) {
    //   await store.dispatch(FETCH_CART_ITEMS)
    // },
    methods: {
      buyThing(){
        console.log("buy")
      },
      clearThing(){
        console.log("clear")
      }
    }
  }
  
  </script>
  
  <style scoped>
  .container {
    margin: 2rem 10rem;
  }
  .list-title {
    font-weight: 700;
    font-size: 1.4rem;
  }
  .list-wrapper {
    margin: 0.4rem 0;
  }
  .list-item {
    display: flex;
  }
  .thumbnail {
    width: 100px;
    height: 100px;
  }
  .description {
    padding: 2rem 1rem;
  }
  .extra-panel {
    text-align: right;
    padding: 0.2rem 0;
  }
  .cart-wrapper {
    position: sticky;
    float: right;
    bottom: 50px;
    right: 50px;
  }
  .cart-wrapper .btn {
    display: inline-block;
    height: 40px;
    font-size: 1rem;
    font-weight: 500;
  }
  </style>