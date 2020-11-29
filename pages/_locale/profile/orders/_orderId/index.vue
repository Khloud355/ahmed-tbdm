<template>
    <div class="order-details">
        <div class="head">
            <h3>Order Details</h3>
            <div class="cancel">
                <img src="/images/icons/svg/reservation-remove.svg" alt="">
                <span>Cancel</span>
            </div>
        </div>
        <div class="details">
            <div class="order">
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
                    <!-- <button class="btn">Order Details</button> -->
                </div>
            </div>
        </div>
        <hr>
        <div class="shipment-details">
            <h3>Shipment Details</h3>
        </div>
        <hr>
        <div class="product-details">
            <h3>Products Details</h3>
        </div>
    </div>
</template>