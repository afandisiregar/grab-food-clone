<template>
    <div class="menu-merchant_wrapper">
        <div class="menu-merchant">
            <a href="#waiki" class="menu-merchant_link menu-active"  @click="handleClikMenu">
                WAIKI RICE Box
            </a>
        </div>
        <div class="menu-merchant">
            <a href="#aigo" class="menu-merchant_link" @click="handleClikMenu">
                Aigo
            </a>
        </div>
        <div class="menu-merchant">
            <a href="#chingu" class="menu-merchant_link" @click="handleClikMenu">
                Chingu
            </a>
        </div>
        <div class="menu-merchant">
            <a href="#seerameonikan" class="menu-merchant_link" @click="handleClikMenu">
                Seerameon Ikan
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MenuMerchant',
    methods: {
        handleClikMenu(e) {
            const menuLinks = document.querySelectorAll('.menu-merchant_link')
            menuLinks.forEach(value => {
                if(!value.classList.contains('menu-active')){
                    e.target.classList.toggle('menu-active')
                }else{
                    value.classList.remove('menu-active')
                }
            })
        }
    }
}
</script>

<style scoped>
    
    .menu-merchant_wrapper{
        display: flex;
        align-items: flex-end;
        height: 66px;
        width: 100%;
        position: sticky;
        top: 88px;
        background-color: #fff;
        box-shadow: 0 4px 6px 0 rgb(28 28 28 / 6%);
        padding: 0 15px;
        z-index: 999;
    }

    .menu-merchant{
        font-size: 1.14285714rem;
        line-height: 1.5;
        font-weight: var(--light);
        color: #676767;
        padding: 14px 24px;
    }

    .menu-merchant_link{
        padding: 18px 14px;
        transition: all .3s;
    }

    .menu-merchant_link:hover{
        color: var(--primary-color);
    }

    .menu-active{
        color: var(--primary-color);
        font-weight: var(--medium-bold);
        border-bottom: 2px solid var(--primary-color);
    }

    @media (max-width:767px) {
        .menu-merchant{
            font-size: 12px;
            padding: 14px 0px;
        }
    }
</style>