<template>
    <div class="user-reservations">
        <div class="head">
            <div class="row">
                <div class="col-3">
                    <span>Name</span>
                </div>
                <div class="col-2">
                    <span>Date</span>
                </div>
                <div class="col-2">
                    <span>Type</span>
                </div>
                <div class="col-3">
                    <span>Cost</span>
                </div>
                <div class="col-2">

                </div>
            </div>
        </div>
        <div class="reservation" v-for="reserve in 4" :key="reserve">
            <div class="row">
                <div class="col-3">
                    <div class="user">
                        <img src="/images/person.jpeg" alt="">
                        <span>Tom Hanks</span>
                    </div>
                </div>
                <div class="col-2">
                    <div class="date">
                        <p>Apr 4, 2020</p>
                        <span>23:00 PM</span>
                    </div>
                </div>
                <div class="col-2">
                    <div class="type">
                        <p>Doctor</p>
                        <span>Dentist</span>
                    </div>
                </div>
                <div class="col-3 align-self-center">
                    <div class="cost">
                        <span>54,00 EGP</span>
                    </div>
                </div>
                <div class="col-2 align-self-center">
                    <div class="remove">
                        <img src="/images/icons/svg/reservation-remove.svg" alt="">
                        <span>Cancel</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>