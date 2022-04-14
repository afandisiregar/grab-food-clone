<template>
    <section id="waiki" class="section-list_menu">
        <div class="list-menu_wrapper container mx-auto">
            <h2 class="title-list_menu">
                WAIKI Rice Box
            </h2>

            <div class="content-list_menu">
                <div class="list-menu_item" v-for="(menu,index) in menus" :key="index">
                    <div class="w-full h-full">
                        <div class="h-full">
                            <div class="list-menu_card disable-overlay">
                                <div class="menu-cover">
                                    <img :src="menu.img" alt="menu.alt" class="menu-image">
                                </div>
                                <div class="menu-info flex flex-col w-full">
                                    <div class="menu-description">
                                        <h3 class="menu-title_info">
                                            {{menu.title}}
                                        </h3>
                                    </div>
                                    <div class="menu-button">
                                        <div class="icon-plus">
                                            <i class="ri-add-line"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Waiki',
    data() {
        return {
            menus: [
                {
                    title: 'Chicken Pop Barbeque & Veggie - Rice Box',
                    img: require('./../../assets/images/afcd0975_3c568fd9625.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/it…20126140536016410/photo/afcd0975_3c568fd9625.jpeg'
                },
                {
                    title: 'Chicken Pop Teriyaki & Veggie - Rice Box',
                    img: require('./../../assets/images/afcd0975_3c568fd9625.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/it…20126140536016410/photo/afcd0975_3c568fd9625.jpeg'
                },
                {
                    title: 'Chicken Pop Salted & Veggie - Rice Box',
                    img: require('./../../assets/images/afcd0975_3c568fd9625.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/it…20126140536016410/photo/afcd0975_3c568fd9625.jpeg'
                },
                {
                    title: 'Chicken Pop Black Pepper & Veggie - Rice Box',
                    img: require('./../../assets/images/afcd0975_3c568fd9625.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/it…20126140536016410/photo/afcd0975_3c568fd9625.jpeg'
                }
            ]
        }
    }
}
</script>

<style scoped>

</style>