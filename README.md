# vue-paginator
A Vue.js eazy to use paginator plugin. It works well for paginating a collection of data of any length.

# Installation

## Via NPM
On your command-line interface, run
`npm install --save eazy-vue-paginator`

## Via CDN
just add the s

#How to use it
Once you've installed it, you can go ahead to use it after you call it once using the following codes
1. `import EazyPaginator from "eazy-vue-paginator"`
2. `import Vue from "vue"`
3. `Vue.use(EazyPaginator)`
4. use it using any of the following options below as per your usage need
In the vue template or vue html app where you want the paginator to appear just use it like so
### Basic Usage
If the collection is a simple array like
`['first','second',...]`
Use it thus
`<v-bsdev-paginator :collection="collection_for_pagination" />`

### More usage
For more than what you have above just use this
`<v-bsdev-paginator :collection="collection_for_pagination" :viewable="viewable_keys" />`

### Multiple Instance Support
Yes, on the same component, view etc, you can call the
`<v-bsdev-paginator :collection="collection_for_pagination" :viewable="viewable_keys" />` and pass different `:collection` and `:viewable` to it.


## Description of params

### :collection param
The collection is the array or json that you want the paginator to paginate.
For instance if you have an array called `namesArray` then the collection should be `... :collection="namesArray" ...`. Same for json

### :viewable param
Most times your paginator collection would contain items that you don't want to display.
Say you have a collection that like `{"first": 283, "name": "Mark", "password" : "kai378vi83u2kud8iueauie336763"}` and you want to display just `first and name`, you have to use the viewable like so by passing an array of your viewable like `viewable=['first', 'name']`, to the `... :viewable="viewable" ...`.

### Note on using :viewable param
If you don't use it, the paginator will assume your collection is just a simple array.

That is all!

Hope you find it usefull. Let's know if you have issues
https://github.com/bsdev-tech/eazy-vue-paginator/issues