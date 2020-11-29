<template>
    <div class="slider-thumbnails">
        <div class="product-slider">

            <div class="swiper" v-swiper:mainSwiper="swiperOption">
                <div class="swiper-wrapper">
                    <div class="swiper-slide" v-for="img in 10" :key="img">
                        <div class="product-img">
                            <img src="/images/image22.png" alt="">
                        </div>
                    </div>
                </div>
            </div>

        </div>

        <div class="thumbnails">
            <div class="product-thumbnails">
                <div class="slider">
                    <div class="swiper arrow-secondary" v-swiper:thumbnailSwiper="swiperThumbnailOption">
                        <div class="swiper-wrapper">
                            <div class="swiper-slide" v-for="img in 10" :key="img">
                                <div class="thumbnail">
                                    <img src="/images/image22.png" alt="">
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

        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            swiperOption: {
                    slidesPerView: 1,
                    loopedSlides: 10,
                    loop: true,
                    // spaceBetween: 14,
                    // initialSlide: 1
                    // centeredSlides: true,
                    // loop: true,
                    // loopedSlides: 54,

                    // pagination: {
                    //   el: ".swiper-pagination",
                    //   clickable: true
                    // }
            },
            swiperThumbnailOption: {
                slidesPerView: 7,
                spaceBetween: 15,
                slideToClickedSlide: true,
                loop: true,
                loopedSlides: 10,
                // touchRatio: 0.8,
                // centeredSlides: true,
                navigation: {
                    nextEl: ".swiper-button-next",
                    prevEl: ".swiper-button-prev"
                }
            }
        }
    },
    mounted() {
        this.mainSwiper.controller.control = this.thumbnailSwiper;
        this.thumbnailSwiper.controller.control = this.mainSwiper;
        // this.mainSwiper.loopedSlides = 5
        console.log('swiper main >>> ', this.mainSwiper.loopedSlides);
        console.log('swiper thumbnail >>> ', this.thumbnailSwiper.loopedSlides);
    }
}
</script>