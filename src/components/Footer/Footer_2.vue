<template>
    <div class="footer-dark">
        <div class="section-container">
            <div class="container mx-auto">
                <div class="row-footer_flex">
                    <div class="footer-col">
                        <div class="countries-text flex-direction">
                            Countries with GrabFood
                        </div>
                        <div class="countries-list flex-direction">
                            <a href="#" class="countries-item">Indonesia</a>
                            <a href="#" class="countries-item">Philippines</a>
                            <a href="#" class="countries-item">Thailand</a>
                            <a href="#" class="countries-item">Vietnam</a>
                            <a href="#" class="countries-item">Singapore</a>
                            <a href="#" class="countries-item">Malaysia</a>
                            <a href="#" class="countries-item">Myanmar</a>
                        </div>
                    </div>
                    <div class="footer-col social-new">
                        <ul>
                            <li>
                                <a href="">
                                    <span class="icon-facebook" style="font-size:32px;">
                                        <i class="ri-facebook-box-fill"></i>
                                    </span>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <span class="icon-instagram" style="font-size:32px;">
                                        <i class="ri-instagram-line"></i>
                                    </span>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <span class="icon-twitter" style="font-size:32px;">
                                        <i class="ri-twitter-line"></i>
                                    </span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="row-footer_flex">
                    <div class="footer-col mt-6">
                        <div class="footer-copyright_item">
                            © Grab 2022
                        </div>
                        <div class="footer-left_item">
                            <a href="" class="item-left">Terms of Service</a>
                            <span class="dots-item_left">•</span>
                            <a href="" class="item-left">Privacy Policy</a>
                        </div>
                    </div>
                    <div class="footer-col mt-6 download-footer">
                        <a href="" width="auto" height="38px">
                            <img src="https://food.grab.com/static/images/logo-appstore.svg" alt="https://food.grab.com/static/images/logo-appstore.svg" style="width:auto; height:38px;">
                        </a>
                        <a href="" class="ml-6" width="auto" height="38px">
                            <img src="https://food.grab.com/static/images/logo-playstore.svg" alt="https://food.grab.com/static/images/logo-playstore.svg" style="width:auto; height:38px;">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .footer-dark{
        background: #363a45;
        color: #fff;
        padding-top: 32px;
        padding-bottom: 48px;
        display: flex;
        flex-direction: column;
        flex: auto;
    }

    .row-footer_flex{
        flex-flow: row wrap;
    }

    .footer-col{
        float: left;
        flex: 0 0 auto;
        display: block;
        width: 50%;
    }

    .countries-text{
        font-size: 16px;
        font-weight: var(--light);
        line-height: 1.5;
        letter-spacing: normal;
        color: #FFF;
        margin-bottom: 8px;
    }

    .flex-direction{
        display: flex;
        justify-content: left;
    }

    .countries-item{
        font-size: 14px;
        color: #FFF;
        text-decoration: none;
    }

    .countries-item::after{
        content: "|";
        color: #6b7896;
        margin-right: 8px;
        margin-left: 8px;
    }

    .countries-item:last-child::after{
        content: "";
    }

    .social-new{
        text-align: right;
    }

    .social-new ul{
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
    }

    .social-new ul li{
        padding-left: 20px;
        display: inline;
    }

    .footer-copyright_item{
        display: flex;
        align-items: center;
        color: #afb0b4;
        font-size: 16px;
        margin-bottom: 8px;
    }

    .footer-left_item{
        display: flex;
        justify-content: left;
    }

    .footer-left_item .item-left{
        font-size: 14px;
    }

    .footer-left_item .dots-item_left{
        margin: 0 8px;
    }

    .download-footer{
        display: flex;
        justify-content: flex-end;
    }

    @media (max-width:992px) {
        .footer-col{
            width: 100%;
        }

        .countries-text{
            justify-content: center;
        }

        .countries-list{
            justify-content: center;
            flex-flow: row wrap;
            margin-bottom: 32px;
        }

        .social-new ul{
            justify-content: center;
        }

        .footer-col{
            width: 100%;
            text-align: center;
        }

        .footer-copyright_item{
            justify-content: center;
        }

        .footer-left_item{
            justify-content: center;
        }

        .footer-col{
            justify-content: center;
        }
    }
</style>