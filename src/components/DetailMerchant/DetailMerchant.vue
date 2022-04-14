<template>
    <div>
        <div class="check-merchant mb-2">
            <span class="icon-check">
                <i class="ri-checkbox-circle-fill"></i>
            </span>
            <p class="title-check">Preferred Merchant</p>
        </div>

        <h1 class="title-merchant mb-1">Do Yan Seafood - Sumbersekar</h1>
        <h3 class="category-merchant">Seafood,Snack</h3>

        <div class="rate-mileage_wrapper my-1">
            <div class="rate-wrapper">
                <img src="	https://food.grab.com/static/images/icons/icon-star.svg" alt="	https://food.grab.com/static/images/icons/icon-star.svg" class="icon-rate">
                <p class="value-rate">4.6</p>
            </div>
            <div class="mileage-wrapper">
                <p class="value-mileage">664.1 km</p>
            </div>
        </div>

        <div class="open-hours_wrapper my-1">
            <label class="open-hours">Opening Hours</label>
            <div class="open-hours_text">
                Today &nbsp;&nbsp; Closed
            </div>
            <div class="closed-badge">
                Closed
            </div>
        </div>

        <div class="promo-wrapper mt-2">
            <div>
                <div class="promo-desc">
                    <img src="	https://food.grab.com/static/images/icons/icon-promo-tag.svg" alt="	https://food.grab.com/static/images/icons/icon-promo-tag.svg" class="icon-promo">
                    <div class="promo-text">DISKONKILATRAMADAN1 50% | HEMAT80G 80rb | HEMAT30G 30%</div>
                </div>
            </div>
            <div class="button-detail">
                See details
            </div>
        </div>

        <div class="order-fee_wrapper">
            <img src="https://food.grab.com/static/images/icons/icon-info.svg" alt="https://food.grab.com/static/images/icons/icon-info.svg" class="icon-fee">
            <div class="order-fee_text">
                Order fee of Rp3.000 applies for this restaurant.
            </div>
        </div>

        <div class="order-fee_mobile">
            <div>
                Order fee of Rp3.000 applies for this restaurant.
            </div>
            <div class="order-icon_mobile">
                <img src="https://food.grab.com/static/images/icons/icon-info.svg" alt="https://food.grab.com/static/images/icons/icon-info.svg" class="icon-fee">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'DetailMerchant',
}
</script>

<style scoped>
    .check-merchant {
        color: var(--primary-color);
        display: flex;
        align-items: center;
        margin-top: .75rem;
    }

    .icon-check{
        margin-right: .5rem;
    }

    .title-check{
        font-size: 14px;
        font-weight: var(--light);
    }

    .title-merchant{
        font-size: 2.57142857rem;
        line-height: 1.33333333;
        font-weight: var(--light);
        margin-bottom: 2px;
    }

    .category-merchant{
        font-size: 14px;
        font-weight: var(--light);
        line-height: 1.42857143;
        color: #676767;
    }

    .rate-mileage_wrapper{
        display: flex;
    }

    .rate-wrapper{
        display: flex;
        align-items: center;
        margin-right: 44px;
    }

    .icon-rate{
        margin-right: 10px;
    }

    .value-rate{
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
    }

    .mileage-wrapper{
        font-size: 14px;
        font-weight: var(--light);
    }

    .open-hours_wrapper{
        display: flex;
        align-items: center;
    }

    .open-hours{
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
        color: #676767;
        margin-right: 42px;
    }

    .open-hours_text{
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
    }

    .closed-badge{
        font-size: .85714286rem;
        line-height: 1.5;
        padding: 4px 8px;
        margin-left: 10px;
        color: #fff;
        background-color: #ee6352;
        font-weight: var(--light);
        border-radius: 4px;
    }

    .promo-wrapper{
        display: flex;
        align-items: center;
    }

    .promo-desc{
        display: flex;
        align-items: center;
    }

    .promo-text{
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
        -webkit-box-flex: 1;
        flex: 1;
        color: #1c1c1c;
        margin-left: 8px;
        margin-right: 16px;
    }

    .button-detail{
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
        padding-bottom: 2px;
        color: var(--secondary-color);
        cursor: pointer;
    }

    .order-fee_wrapper{
        display: flex;
        align-items: center;
    }

    .icon-fee{
        width: 24px;
        height: 24px;
        margin-right: 8px;
    }

    .order-fee_text{
        flex: 1;
        font-size: 14px;
        line-height: 1.42857143;
        font-weight: var(--light);
    }

    .order-fee_mobile{
        display: none;
        align-items: center;
        padding: 10px 15px;
        background-color: #f9fbfd;
        border-radius: 4px;
        font-size: 12px;
    }

    @media (max-width:580px) {
        .promo-wrapper{
            display: block;
        }

        .order-fee_mobile{
            display: flex;
        }

        .order-icon_mobile{
            padding-left: 10px;
        }

        .icon-fee{
            width: 16px;
            height: 16px;
        }

        .order-fee_wrapper{
            display: none;
        }
    }
</style>