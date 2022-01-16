<template>
    <div class="col">
        <div class="icon">
            <img :src="image" :alt="alt">
        </div>
        <p>{{ text }}</p>
    </div>
</template>

<script>
export default {
    name: 'MainLinks',
    props: ['image', 'alt', 'text']
}
</script>

<style lang="scss">
    .col {
        height: 100%;
        flex-basis: calc(100% / 6);
        margin-right: 2em;
        padding: 3em 0;
        display: flex;
        align-items: center;
        .icon {
            height: 60%;
            margin-right: 1em;
            img {
                height: 100%;
            }
        }
        p {
            font-size: 0.8em;
            text-transform: uppercase;
            font-weight: 400;
            color: white;
        }
    }
</style>