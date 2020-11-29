<template>
    <div class="wishlist">
        <h3>Wishlist</h3>
        <div class="item" v-for="item in 8" :key="item">
            <div class="item-img">
                <img class="img-thumbnail" src="/images/T-shirt.png" alt="">
            </div>
            <div class="desc">
                <h5>Green T-shirt 2016</h5>
                <p>Men BK3569</p>
                <span class="remove">
                    <img src="/images/icons/svg/wishlist-remove.svg" alt="">
                    Remove
                </span>
            </div>
            <div class="price">
                $13
            </div>
            <div class="add-cart">
                <button class="btn">Move to Cart</button>
            </div>
        </div>
    </div>
</template>