<script setup>

const props = defineProps ({
    darkMode: {
        default: false,
        type: Boolean
    }
})
</script>

<template>
    <header :class="['header', {'header--darkmode' : props.darkMode}]">
        <p class="header__title">Barbod <span class="header__title--accent-color">Garshasbi</span></p>
        <div class="header__nav">
            <p class="header__nav__itm">About</p>
            <p onclick="window.location='#projects'" class="header__nav__itm">Projects</p>
            <p class="header__nav__itm">Contacts</p>
        </div>
    </header>
</template>

<style lang="scss">

.header {
    background-color: #191919;
    
    display: flex;
    justify-content: space-between;
    align-items: center;

    width: 100vw;
    
    padding: 2rem 4rem;

    .header__title {
        cursor: pointer;
        color: #EEEEEE;
 
        text-transform: uppercase;
 
        font-size: 2rem;
        font-weight: 500;
        letter-spacing: .6rem;
    }
    .header__title--accent-color {
        color: #c99f7c;
    }
    .header__nav {
        display: flex;
        .header__nav__itm {
            cursor: pointer;
            color: #EEEEEE;

            text-transform: uppercase;

            font-size: 1.2rem;
            font-weight: 200;
            margin-left:  6rem;

            transition-duration: 300ms;
        }
        .header__nav__itm:hover {
            transform: translateY(-.2rem );
        }
    }
}
.header--darkmode {
    background-color: #1E4652;
    .header__title {
        color: #FFF9EC;
    }
}

</style>
