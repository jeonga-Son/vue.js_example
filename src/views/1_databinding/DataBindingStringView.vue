<template>
  <div>
    <h1>Hello {{ userName }}</h1>
    <p>{{message}}</p>
  </div>
</template>

<script>
// eslint-disable-next-line
/* eslint-disable */
export default {
    // eslint-disable-next-line
    /* eslint-disable */
    data() {
        // eslint-disable-next-line
        /* eslint-disable */
        return {
            // eslint-disable-next-line
            /* eslint-disable */
            userName: 'Jone Doe',
            message: 'Welcome 개발자의 품격',
            arr: [],
            obj: {}
        }
    }
}
</script>

<style scoped>
.text-red {
    color: red;
}
</style>