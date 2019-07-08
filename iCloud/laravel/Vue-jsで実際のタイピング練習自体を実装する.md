# Vue.jsで実際のタイピング練習自体を実装する


LaravelではすぐにVueが使えるようにpackage.jsonにすでに記述されている


npm I で必要なライブラリをいんすと





},
"devDependencies": {
"axios": "^0.19",
"bootstrap": "^4.1.0",
"cross-env": "^5.1",
"jquery": "^3.2",
"laravel-mix": "^4.0.7",
"lodash": "^4.17.5",
"popper.js": "^1.12",
"resolve-url-loader": "^2.3.1",
"sass": "^1.15.2",
"sass-loader": "^7.1.0",
"vue": "^2.6.10"
}


laravelでは全てのjsはresources/js/app.js で管理している


このapp.jsの親のビューはlayouts/app.blade.phpになっている



仕組みとしてはresources/js/app.js

Publicのapp.jsを作っているのがここ。

resources/js/app.jsを元に、コンパイルをして

結合している



resources/js/app.js

requre()

Window.Vue = rewuire(‘vue’)とか


Const app = new Vue({




Resources/js/app.jsに
Vue.component('example-component', require('./components/ExampleComponent.vue').default);



として読み込むことが必要である