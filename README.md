# vve-vue-axios

[![Build Status](https://travis-ci.org/vue-viewer-editor/vve-vue-axios.svg?branch=master)](https://travis-ci.org/vue-viewer-editor/vve-vue-axios)

A small wrapper for integrating axios to Vuejs

## How to install:
### CommonJS:
```bash
npm install --save axios vve-vue-axios
```

And in your entry file:
```js
import Vue from 'vue'
import axios from 'axios'
import VueAxios from 'vve-vue-axios'

Vue.use(VueAxios, axios)
```

### Script:
Just add 3 scripts in order: `vue`, `axios` and `vve-vue-axios` to your `document`.

## Usage:
This wrapper bind `axios` to `Vue` or `this` if you're using single file component.

You can use `axios` like this:
```js
Vue.axios.get(api).then((response) => {
  console.log(response.data)
})

Vue.$axios.get(api).then((response) => {
  console.log(response.data)
})

this.axios.get(api).then((response) => {
  console.log(response.data)
})

this.$axios.get(api).then((response) => {
  console.log(response.data)
})

this.$http.get(api).then((response) => {
  console.log(response.data)
})
```

Please kindly check full documention of [axios](https://github.com/axios/axios) too 

### Thanks
[vue-axios](https://github.com/imcvampire/vue-axios)
