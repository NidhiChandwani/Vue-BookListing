<template>
<div>
    <h1>{{title}}</h1>
    <ul>
        <li v-for="book in books" v-bind:key='book.title>{{book.title}}:{{book.author}}</li>
    </ul>
</div>
</template>

<script>
module.exports = {
    name: 'BookList',
    data: function () {
        return {
            title: 'All Books',
            books: [
                    {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
                    {title: 'American Gods', author: 'Neil Gaiman'},
                    {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
                ]
            }
         }
    }
</script>

<style scoped>
h1,h2 {
    font-weight: normal
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: block;
    margin: 0 10px;
}
</style>