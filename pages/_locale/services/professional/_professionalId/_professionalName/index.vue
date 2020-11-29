<template>
    <section class="profession-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Medical Services</nuxt-link></li>
                    <li class="breadcrumb-item active" aria-current="page">Doctor Profile</li>
                </ol>
            </nav>

            <div class="row">
                <div class="col-8">
                    <div class="doctor-info">
                        <div class="info">
                            <div class="doctor-img">
                                <img src="/images/person.jpeg" alt="">
                            </div>
                            <div class="title">
                                <h4>Tom Hanks</h4>
                                <span>Dentist</span>
                            </div>
                            <div class="rate">
                                <div class="rate-box">
                                    <span>5.0</span>
                                    <img src="/images/icons/svg/vendor-star.svg" alt="">
                                </div>
                            </div>
                        </div>
                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the  industry’s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. Lorem Ipsum has been the  industry’s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
                    </div>
                    <div class="clinic" v-for="clinic in 2 " :key="clinic">
                        <h3>Clinic 1</h3>
                        <div class="clinic-contacts">
                            <div class="contacts">
                                <div class="row">
                                    <div class="col-md-6">
                                        <div class="contact">
                                            <img src="/images/icons/svg/phone.svg" alt="">
                                            <p>414-4645-5416</p>
                                        </div>
                                    </div>
                                    <div class="col-md-6">
                                        <div class="contact">
                                            <img class="mail" src="/images/icons/svg/mail.svg" alt="">
                                            <p>info@tbdm.net</p>
                                        </div>
                                    </div>
                                    <div class="col-md-6">
                                        <div class="contact">
                                            <img src="/images/icons/svg/location.svg" alt="">
                                            <p class="location">New Cairo, Egypt</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div class="appointments">
                            <div class="swiper arrow-secondary" v-swiper="swiperOption" :instance-name="'mySwiper' + clinic">
                                <div class="swiper-wrapper">
                                    <div class="swiper-slide" v-for="vendor in 7" :key="vendor">
                                        <div class="appointment">
                                            <div class="info">
                                                <p class="day">Monday</p>
                                                <p class="time">23:00 - 24:00</p>
                                                <p class="price">25.00 <span>EGP</span></p>
                                            </div>
                                            <div class="book">
                                                Book Now
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="swiper-button-prev" slot="button-prev">
                                    <img style="transform: rotate(180deg)" src="/images/icons/svg/offers-arrow.svg" alt="">
                                </div>
                                <div class="swiper-button-next" slot="button-next">
                                    <img src="/images/icons/svg/offers-arrow.svg" alt="">
                                </div>
                            </div>
                        </div>

                    </div>

                    <div class="reviews">
                        <div class="add-review">
                            <h4>Add your review</h4>
                            <div class="row no-gutters">
                                <div class="col-3">
                                    <h6>Your review</h6>
                                </div>
                                <div class="col-9">
                                    <textarea class="form-control" id="review" rows="4"></textarea>
                                </div>
                            </div>
                            <div class="row no-gutters">
                                <div class="col-3 d-flex align-items-center">
                                    <h6>Overall rating</h6>
                                </div>
                                <div class="col-9">
                                    <client-only>
                                        <star-rating 
                                            :rating="3.5" 
                                            :increment=".5"
                                            active-color="#FFD506" 
                                            :show-rating="false" 
                                            :star-size="20"
                                            :padding=".9">
                                        </star-rating>
                                    </client-only>
                                </div>
                            </div>
                            <div class="row no-gutters">
                                <div class="col-3"></div>
                                <div class="col-9">
                                    <button class="btn">Submit</button>
                                </div>
                            </div>
                        </div>
                        <hr>
                        <div class="prev-reviews">
                            <h4>Previous reviews</h4>
                            <div class="row no-gutters review">
                                <div class="col-3">
                                    <client-only>
                                        <star-rating 
                                            :rating="3.5" 
                                            :increment=".5"
                                            :read-only="true" 
                                            active-color="#FFD506" 
                                            :show-rating="false" 
                                            :star-size="20"
                                            :padding=".9">
                                        </star-rating>
                                    </client-only>
                                    <h6>Pablo Permins</h6>
                                    <span class="time">one hour ago</span>
                                </div>
                                <div class="col-9">
                                    <div class="comment">
                                        <p>Got this through the post the other day and right from opening the packet I knew this was quality, put it on and I was right!! Well done</p>
                                        <div class="icons">
                                            <div class="icon">
                                                <span class="image">
                                                    <img src="/images/icons/svg/comment-heart.svg" alt="">
                                                </span>
                                                <span class="count">113</span>
                                            </div>
                                            <div class="icon">
                                                <span class="image">
                                                    <img src="/images/icons/svg/icon-comment.svg" alt="">
                                                </span>
                                                <span class="count">6</span>
                                            </div>
                                            <!-- <div class="more">
                                                <p>See more reviews</p>
                                            </div> -->
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="row no-gutters review">
                                <div class="col-3">
                                    <client-only>
                                        <star-rating 
                                            :rating="3.5" 
                                            :increment=".5"
                                            :read-only="true" 
                                            active-color="#FFD506" 
                                            :show-rating="false" 
                                            :star-size="20"
                                            :padding=".9">
                                        </star-rating>
                                    </client-only>
                                    <h6>Pablo Permins</h6>
                                    <span class="time">one hour ago</span>
                                </div>
                                <div class="col-9">
                                    <div class="comment">
                                        <p>Got this through the post the other day and right from opening the packet I knew this was quality, put it on and I was right!! Well done</p>
                                        <div class="icons">
                                            <div class="icon">
                                                <span class="image">
                                                    <img src="/images/icons/svg/comment-heart.svg" alt="">
                                                </span>
                                                <span class="count">113</span>
                                            </div>
                                            <div class="icon">
                                                <span class="image">
                                                    <img src="/images/icons/svg/icon-comment.svg" alt="">
                                                </span>
                                                <span class="count">6</span>
                                            </div>
                                            <!-- <div class="more">
                                                <p>See more reviews</p>
                                            </div> -->
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="more">
                                <p>See more reviews</p>
                            </div>

                        </div>
                    </div>

                </div>
                <div class="col-4">
                    <div class="doctor-contacts">
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
export default {
    data() {
        return {
            swiperOption: {
                    slidesPerView: 4,
                    spaceBetween: 30,
                    // initialSlide: 1
                    // centeredSlides: true,
                    // loop: true,
                    // loopedSlides: 54,
                    navigation: {
                    nextEl: ".swiper-button-next",
                    prevEl: ".swiper-button-prev"
                    }
                    // pagination: {
                    //   el: ".swiper-pagination",
                    //   clickable: true
                    // }
            }
        }
    }
}
</script>

