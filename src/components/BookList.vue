<template>
<div>
    <h1>{{title}}</h1>
</div>
</template>

<script>
module.exports = {
    name: 'BookList',
    data: function () {
        return {
            title: 'All Books'
        }
    }
}
</script>

<style scoped>
h1,h2 {
    font-weight: normal
}
</style>