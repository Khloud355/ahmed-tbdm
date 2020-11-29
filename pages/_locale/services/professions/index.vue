<template>
    <div class="professions-content">
        <section class="professions">
            <div class="head">
                <h3>Carpenter</h3>
                <nuxt-link to="/">See more</nuxt-link>
            </div>

            <div class="profession-cards">
                <app-slider-profession></app-slider-profession>
            </div>

        </section>

        <section class="professions">
            <div class="head">
                <h3>Plumber</h3>
                <nuxt-link to="/">See more</nuxt-link>
            </div>

            <div class="profession-cards">
                <app-slider-profession></app-slider-profession>
            </div>

        </section>
    </div>
</template>

<script>
import SliderProfession from '~/components/Vendor/SliderProfession';

export default {
    components: {
        appSliderProfession: SliderProfession
    }
}
</script>