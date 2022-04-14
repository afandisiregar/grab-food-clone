<template>
    <section id="aigo" class="section-list_menu">
        <div class="list-menu_wrapper container mx-auto">
            <h2 class="title-list_menu">
                Aigo
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
    name: 'Aigo',
    data() {
        return {
            menus: [
                {
                    title: 'Seo Goo Lalapan Ikan Laut Bakar/Goreng (Banyak Pilihan Ikan)',
                    description: 'Ikan Laut+Nasi dibakar dengan bumbu Bikin Doyan',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090000020527/photo/4a4aac07_5e40df724ba.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090000020527/photo/4a4aac07_5e40df724ba.jpeg'
                },
                {
                    title: 'Nasi Goreng Do Yan Seafood',
                    description: 'Nasi Putih + Udang goreng saos telur asin',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090001023678/photo/5242e957_ff2cdac04a8.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090001023678/photo/5242e957_ff2cdac04a8.jpeg'
                },
                {
                    title: 'Seo Goo Udang Saos Telur asin',
                    description: 'Nasi Putih + Udang goreng saos telur asin',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090004019767/photo/b031427f_bb8709e4e00.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090004019767/photo/b031427f_bb8709e4e00.jpeg'
                },
                {
                    title: 'Seo Goo Cumi Saus Telur Asin',
                    description: 'Nasi putih + Cumi goreng tepung saus telur asin',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090005024740/photo/ba094858_f4282e50a8b.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090005024740/photo/ba094858_f4282e50a8b.jpeg'
                },
                {
                    title: 'Seo Goo Udang (Banyak Pilihan Saos)',
                    description: 'Nasi Kotak Udang (Prawns Rice Box)',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090007031824/photo/e52484f4_c61a14249f7.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090007031824/photo/e52484f4_c61a14249f7.jpeg'
                }
            ]
        }
    }
}
</script>

<style scoped>
    
</style>