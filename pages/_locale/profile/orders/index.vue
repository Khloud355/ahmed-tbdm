<template>
    <div class="orders">
        <h3>Orders</h3>

        <div class="order" v-for="order in 6" :key="order">
            <div class="info">
                <div class="row">
                    <div class="col-4 title">
                        <p>Order placed on: </p>
                        <p>Order ID: </p>
                        <p>Recipient: </p>
                        <p>Payment method: </p>
                    </div>
                    <div class="col-8 answer">
                        <p>Apr. 4, 2020</p>
                        <p>4984651984</p>
                        <p>Tom Hanks</p>
                        <p>Card end with **** 6987</p>
                    </div>
                </div>
            </div>
            <div class="total">
                <h6>Total</h6>
                <p class="price">20,000 EGP</p>
                <button class="btn">Order Details</button>
            </div>
        </div>
    </div>
</template>