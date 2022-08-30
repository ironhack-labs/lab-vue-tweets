<template>
    <span className="timestamp"> {{ timestamp}} </span>
</template>

<script>
export default {
    name : "Timestamp",
    props: {//recibe del padre app.vue la variable timestamp
        timestamp: String,
    },
};
</script>

<style>

</style>