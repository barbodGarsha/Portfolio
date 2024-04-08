<script setup>

const props = defineProps({
    title: {
        default: '',
        type: String
    },
    image: {
        default: null,
        type: Image
    },
    href: {
        default: '',
        type: String
    }
})

function clicked() {
    window.location.href=props.href
}
</script>

<template>
    <div @click="clicked" class="card">
        <img :src="props.image" alt="background image" class="card__background">
        <p class="card__title">{{ props.title }}</p>
    </div>
</template>

<style lang="scss">
    .card {
        cursor: pointer;
        position: relative;
        overflow: hidden;
        width: 30%;
        height: 30vh;
        border-radius: 12px;

        transition-duration: 300ms;


        .card__background {
            width: 100%;
            border-radius: 12px;
            
        }

        .card__title {
            box-sizing: border-box;
            color: #EEEEEE;
            background: linear-gradient(0deg, rgba(25,25,25,1) 0%, rgba(25,25,25,0) 100%);
            position: absolute;
            bottom: 0;
            left: 0;

            display: flex;
            align-items: flex-end;
            padding: 1.5rem 1.2rem;            

            width: 100%;
            height: 100%;

            font-size: 1.5rem;
            font-weight: 500;
            transition-duration: 300ms;

            
        }
    }
    .card:hover {
        scale: 1.05;
    }
</style>
