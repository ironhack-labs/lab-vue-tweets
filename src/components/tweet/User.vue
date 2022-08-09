<template>
    <span className="user">
        <span className="name">{{ username }}</span>
        <span className="handle">@{{ handle }}</span>
    </span>
</template>

<script>
export default {
    props:['username', 'handle']
}
</script>

<style>

</style>