<template>
    <section id="chingu" class="section-list_menu">
        <div class="list-menu_wrapper container mx-auto">
            <h2 class="title-list_menu">
                Chingu
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
    name: 'Chingu',
    data() {
        return {
            menus: [
                {
                    title: 'Oppa Cham Po Ryeo (Crispy Gurita, Cumi & Udang)',
                    description: 'Goreng Krispi Campur Gurita, Udang, & Cumi (Octopus, ..)',
                    img: require('./../../assets/images/5eefdacf_7dd55e6fe6d.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090000020527/photo/4a4aac07_5e40df724ba.jpeg'
                },
                {
                    title: 'Oppa Cumi ( Cumi Utuh Crispy)',
                    description: 'Per Tusuk - Cumi Utuh Goreng Krispi korea (Crispy Fried Squid)',
                    img: require('./../../assets/images/4f26b747_5b7568648ea.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090000020527/photo/4a4aac07_5e40df724ba.jpeg'
                },
                {
                    title: 'Unnie Cumi Crispy',
                    description: 'Cumi Goreng Krispi (Crispy Fried Calamari)',
                    img: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090011029814/photo/e7fb457e_5321446a93d.jpeg',
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090011029814/photo/e7fb457e_5321446a93d.jpeg'
                },
                {
                    title: 'Oppa Cumi Bae Sah ( Cumi dan kerang Masak Saos - 2 Porsi)',
                    description: 'Cumi Masak Saos (Cooked Calamari With Sauce)',
                    img: require('./../../assets/images/b4a46b46_af001f0b18b.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090005024740/photo/ba094858_f4282e50a8b.jpeg'
                },
                {
                    title: 'Aegi Kepiting (Crispy Baby Kepiting Rajungan)',
                    description: 'Kepiting Muda Goreng Krispi (Crispy Fried Baby Crab)',
                    img: require('./../../assets/images/45d199f4_67656741dcc.jpeg'),
                    alt: 'https://d1sag4ddilekf6.azureedge.net/compressed/items/IDITE20211207090007031824/photo/e52484f4_c61a14249f7.jpeg'
                }
            ]
        }
    }
}
</script>

<style scoped>
    
</style>