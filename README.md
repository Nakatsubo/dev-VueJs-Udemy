# README
Let's study & enjoy Vue.js<br>
Referenced by<br>
<a href="https://www.udemy.com/" target="_blank" rel="nopener">https://www.udemy.com/</a>


- <a href="">Chapter1 Basic</a>

## Chapter1

### 環境構築
Vue.js の読み込み

#### テスト環境

```
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
```

#### 本番環境

```
<script src="https://cdn.jsdelivr.net/npm/vue"></script>
```

## Chapter2

### インスタンス

```
// 戻り値はルートのVueインスタンス
const app = new Vue({
  // options
})
```

### データバインディング
データと描画を同期させる仕組みのこと。

- 双方向バインディング(TwoWay)
- 単方向バインディング(OneWay)
- ワンタイムバインディング(OneTime)

```
<div id="app">
  <p><input type="text" v-model="message"></p>
  <p>{{ message }}</p>
</div>

const app = new Vue({
  el: '#app',
  data: {
    message: 'Hello, Vue.js'
  }
})
```

