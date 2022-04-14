<template>
    <div class="merchant-photo_wrapper">
        <div class="merchant-cover">
            <img :src="require('./../../assets/images/03c7f74481b8467eaee275265311a7bb_1628499015316487688.png')" alt="https://d1sag4ddilekf6.azureedge.net/compressed/me…481b8467eaee275265311a7bb_1628499015316487688.png" class="merchant-image">
        </div>
    </div>
</template>

<style scoped>
    .merchant-photo_wrapper{
        display: none;
        flex: 0;
    }

    .merchant-cover{
        width: 100%;
    }

    .merchant-image{
        width: 100%;
        height: 100%;
    }

    @media (max-width:550px){
        .merchant-photo_wrapper{
            display: block;
        }
    }
</style>