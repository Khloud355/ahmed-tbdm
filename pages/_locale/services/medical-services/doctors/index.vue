<template>
    <section class="specialities-list">

            <div class="specialities">
                <div class="head">
                    <h3>Dentists</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctors">
                    <app-slider-doctor></app-slider-doctor>
                </div>

            </div>

            <div class="specialities">
                <div class="head">
                    <h3>Neurologists</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctors">
                    <app-slider-doctor></app-slider-doctor>
                </div>

            </div>

            <div class="specialities">
                <div class="head">
                    <h3>Cardiologist</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctors">
                    <app-slider-doctor></app-slider-doctor>
                </div>

            </div>

    </section>
</template>

<script>
import MainCategories from '~/components/Categories/MedicalMainCategories'
import SliderDoctor from '~/components/Vendor/SliderDoctor'

export default {
    components: {
        appMainCategories: MainCategories,
        appSliderDoctor: SliderDoctor
    },
    data() {
        return {

        }
    }
}
</script>