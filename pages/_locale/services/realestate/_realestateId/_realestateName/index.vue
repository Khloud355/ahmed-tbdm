<template>
    <section class="realestate-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Restaurants</nuxt-link></li>
                    <!-- this will be restaurant name -->
                    <li class="breadcrumb-item active" aria-current="page">RealestateProfile</li>
                </ol>
            </nav>

            <div class="row">
                <div class="col-8">
                    <app-slider-thumbnails></app-slider-thumbnails>

                    <div class="details">
                        <div class="head">
                            <h3>Twin House Ultra Modern</h3>
                            <span>$20.000</span>
                        </div>
                        <div class="desc">
                            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry’s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
                        </div>
                    </div>

                    <div class="features">
                        <h3>Features</h3>
                        <div class="row justify-content-between">
                            <div class="col-5">
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-type.svg" alt="">
                                        <span>Type</span>
                                    </div>
                                    <p>Lands</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-finishing.svg" alt="">
                                        <span>Finishing</span>
                                    </div>
                                    <p>Half</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-space.svg" alt="">
                                        <span>Floor Space</span>
                                    </div>
                                    <p>12 FT</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-payment.svg" alt="">
                                        <span>Payment Method</span>
                                    </div>
                                    <p>Installments</p>
                                </div>
                            </div>
                            <div class="col-5">
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-bedroom.svg" alt="">
                                        <span>Bedrooms</span>
                                    </div>
                                    <p>4</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-balacony.svg" alt="">
                                        <span>Balaconies</span>
                                    </div>
                                    <p>5</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-bathroom.svg" alt="">
                                        <span>Bathrooms</span>
                                    </div>
                                    <p>3</p>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-furnishing.svg" alt="">
                                        <span>Furnishing</span>
                                    </div>
                                    <p>Furnished</p>
                                </div>

                            </div>
                        </div>
                        <div class="row">
                            <div class="col-12">
                                <hr>
                            </div>
                        </div>
                        <div class="row justify-content-between">
                            <div class="col-5">
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-pool.svg" alt="">
                                        <span>Pool</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-garden.svg" alt="">
                                        <span>Garden</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-security.svg" alt="">
                                        <span>Security</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-pets.svg" alt="">
                                        <span>Pets allowed</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-kitchen.svg" alt="">
                                        <span>Kitchen appliance</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                            </div>
                            <div class="col-5">
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-view.svg" alt="">
                                        <span>View</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-area.svg" alt="">
                                        <span>BBQ Area</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-concierge.svg" alt="">
                                        <span>Concierge</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                                <div class="feature">
                                    <div class="icon">
                                        <img src="/images/icons/svg/realestate-maid.svg" alt="">
                                        <span>Maid Service</span>
                                    </div>
                                    <div class="check">
                                        <img src="/images/icons/svg/realestate-check.svg" alt="">
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="vendor-profile">
                        <!-- <h3>Vendor Profile</h3> -->
                        <div class="info">
                            <img src="/images/vendor.png" alt="">
                            <div class="name">
                                <h5>Tom Hanks</h5>
                                <span>2,465 Product</span>
                            </div>
                            <div class="rate">
                                <span>5.0</span>
                                <img src="/images/icons/svg/vendor-star.svg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="contacts">
                            <div class="row no-gutters">
                                <div class="col-1"><img src="/images/icons/svg/phone.svg" alt=""></div>
                                <div class="col-1"></div>
                                <div class="col-10"><p>414-4645-5416</p></div>
                            </div>
                            <div class="row no-gutters">
                                <div class="col-1"><img class="mail" src="/images/icons/svg/mail.svg" alt=""></div>
                                <div class="col-1"></div>
                                <div class="col-10"><p>info@tbdm.net</p></div>
                            </div>
                            <div class="row no-gutters">
                                <div class="col-1"><img src="/images/icons/svg/location.svg" alt=""></div>
                                <div class="col-1"></div>
                                <div class="col-10"><p>New Cairo, Egypt</p></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>
</template>

<script>
import SliderThumbnails from '~/components/SliderThumbnails';

export default {
    components: {
        appSliderThumbnails: SliderThumbnails
    },
}
</script>