<template>
    <section id="seerameonikan" class="section-list_menu">
        <div class="list-menu_wrapper container mx-auto">
            <h2 class="title-list_menu">
                Seeramon Ikan
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
                                        <div class="menu-description_info">
                                            {{menu.description}}
                                        </div>
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
    name: 'SeeramonIkan',
    data() {
        return {
            menus: [
                {
                    title: 'Ikan Kerapu Siram Saos',
                    description: 'Ikan Kerapu Siram Saos Asam Manis / telur asin',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090016033177/photo/1a00fe16_7296f872d67.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090016033177/photo/1a00fe16_7296f872d67.jpeg'
                },
                {
                    title: 'Ikan Kakap Siram Saos',
                    description: 'Ikan Kakap Siram Saos Asam Manis / telur asin',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090018013134/photo/992a34b0_488920e58ab.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090001023678/photo/5242e957_ff2cdac04a8.jpeg'
                },
            ]
        }
    }
}
</script>

<style scoped>
    
</style>