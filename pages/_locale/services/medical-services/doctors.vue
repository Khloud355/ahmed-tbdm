<template>
    <section class="doctors-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Medical Services</nuxt-link></li>
                    <li class="breadcrumb-item active" aria-current="page">Doctors</li>
                </ol>
            </nav>

            <app-main-categories></app-main-categories>

            <nuxt-child></nuxt-child>

        </div>
    </section>
</template>

<script>
import MainCategories from '~/components/Categories/DoctorsMainCategories'
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