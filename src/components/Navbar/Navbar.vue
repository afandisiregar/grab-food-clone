<template>
    <div class="nav-main-container">
        <div class="container mx-auto flex items-center navbar-container">
            <a href="#">
                <h1 class="nav-brand">
                    <img src="https://food.grab.com/static/images/logo-grabfood2.svg" alt="https://food.grab.com/static/images/logo-grabfood-white2.svg" class="navbar-logo">
                </h1>
            </a>
            <div class="search-navbar">
                <div class="search-navbar_wrapper">
                    <div class="input-search" id="search-an-active" @click.prevent="handleClickSearch" v-click-outside="handleClickOutside">
                        <span class="icon-map_pin">
                            <i class="ri-map-pin-line"></i>
                        </span>
                        <span class="title-search">
                            Type your location
                        </span>
                    </div>
                    <div class="search-input_active search-hide" id="search-active">
                        <div class="input-active">
                            <span class="icon-map_input">
                                <i class="ri-map-pin-line"></i>
                            </span>
                            <input type="text" placeholder="Type your location" class="input-search_navbar" id="input-search">
                        </div>
                    </div>
                </div>
            </div>
            <ul class="nav-link_wrapper">
                <li class="">
                    <div class="nav-link_item">
                        <button type="button" class="button-bag">
                            <i class="ri-shopping-bag-2-line"></i>
                        </button>
                    </div>
                </li>
                <li class="auth-wrapper ml-2">
                    <div class="login-wrapper">
                        <a href="" class="login-link">
                            Login/Sign Up
                        </a>
                    </div>
                </li>
            </ul>    
        </div>
        <div class="cotainer mx-auto">
            
        </div>
    </div>
</template>

<script>
import  ClickOutside from 'vue-click-outside'

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Navbar',
    directives: {
        ClickOutside
    },
    methods:{ 
        handleClickSearch() {
            const searchAnActive = document.getElementById('search-an-active')
            const searchActive = document.getElementById('search-active')
            
            
            if (!searchAnActive.classList.contains('search-hide')) {
                searchAnActive.classList.toggle('search-hide')
            }

            if (searchActive.classList.contains('search-hide')) {
                searchActive.classList.remove('search-hide')
                searchActive.classList.toggle('search-show')
                document.getElementById('input-search').focus()
            }


        },
        handleClickOutside() {
            const searchAnActive = document.getElementById('search-an-active')
            const searchActive = document.getElementById('search-active')

            if (searchAnActive.classList.contains('search-hide')) {
                searchAnActive.classList.remove('search-hide')
            }

            if (!searchActive.classList.contains('search-hide')) {
                searchActive.classList.toggle('search-hide')
                searchActive.classList.remove('search-show')
            }
        }
    }
}
</script>

<style scoped>
    .nav-brand {
        font-size: 20px;
        font-weight: var(--bold);
    }

    .navbar-logo{
        width: auto;
        height: 50px;
    }

    .nav-main-container{
        height: 88px;
        background-color: #FFF;
        /* border-bottom: 1px solid #e8e8e8;
        transition: .3s; */
        width: 100%;
        position: sticky;
        top: 0;
        left: 0;
        right: 0;
        z-index: 100;
    }

    .navbar-container{
        height: 88px;
        display: flex; 
        align-items: center; 
        justify-content: space-between;
    }

    .search-navbar{
        flex: 1 1 0%;
        width: 1px;
    }

    .search-navbar_wrapper{
        display: flex;
        justify-content: flex-start;
        flex-flow: row wrap;
    }

    .input-search{
        flex: 1 1 0%;
        width: 1px;
        max-width: 360px;
        height: 40px;
        margin: 0 50px;
        border: 1px solid #c5c5c5;
        border-radius: 6px;
        font-size:14px;
        font-weight: var(--light);
        color: #1c1c1c;
        cursor: pointer;
        padding: 0 24px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .icon-map_pin{
        margin-left: 4px;
        margin-right: 4px;
        font-size: 16px;
    }

    .title-search{
        color: #c5c5c5;
    }

    .nav-link_item{
        height: 40px;
        margin-left: 6px;
        margin-right: 6px;
    }

    .nav-link_wrapper{
        display: flex;
    }

    .button-bag{
        max-width: 40px;
        border: 1px solid #f0efef;
        background-color: #fff;
        padding: 5px 20px;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 6px;
    }

    .auth-wrapper{
        height: 40px;
    }

    .login-wrapper{
        height: 40px;
        font-size: 12px;
        font-weight: var(--bold);
        text-align: center;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .login-link{
        height: 100%;
        border-radius: 4px;
        border: 1px solid #f0efef;
        color: #676767;
        background-color: #FFF;
        padding: 0 12px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .search-input_active{
        height: 40px;
        margin: 0 50px;
    }

    .input-active{
        position: relative;
        width: 360px;
    }

    .icon-map_input{
        position: absolute;
        left: 15px;
        top: 20%;
        font-size: 16px;
    }

    .input-search_navbar{
        width: 100%;
        height: 40px;
        background: transparent;
        padding-left: 40px;
        padding-right: 40px;
        border-width: 1px;
        line-height: 1.42857143;
        border-color: #c5c5c5;
        border-radius: 6px;
        font-size: 14px;
        font-weight: var(--light);
        transition: all .3s;
    }

    .input-search_navbar:focus{
        outline: none !important;
        border: .5px solid var(--primary-color) !important;
        box-shadow: 0 0 5px var(--primary-color);
    }

    .search-show{
        display: block;
    }

    .search-hide{
        display: none;
    }

    @media (max-width:992px){
        .search-navbar{
            display: none !important;
        }

        .navbar-container{
            height: 60px;
            border-bottom: 1px solid #f0efef;
        }
    }
</style>