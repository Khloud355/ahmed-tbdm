<template>
    <section class="medical-services-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item active" aria-current="page">Medical Services</li>
                </ol>
            </nav>

            <app-main-categories></app-main-categories>

            <section class="medical-service">
                <div class="head">
                    <h3>Doctors</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctor-cards">
                    <app-slider-medical></app-slider-medical>
                </div>

            </section>

            <section class="medical-service">
                <div class="head">
                    <h3>Clinics</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctor-cards">
                    <app-slider-medical></app-slider-medical>
                </div>

            </section>

            <section class="medical-service">
                <div class="head">
                    <h3>SPA</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctor-cards">
                    <app-slider-medical></app-slider-medical>
                </div>

            </section>

            <section class="medical-service">
                <div class="head">
                    <h3>Hospitals</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctor-cards">
                    <app-slider-medical></app-slider-medical>
                </div>

            </section>

            <section class="medical-service">
                <div class="head">
                    <h3>Pharmacies</h3>
                    <nuxt-link to="/">See more</nuxt-link>
                </div>

                <div class="doctor-cards">
                    <app-slider-medical></app-slider-medical>
                </div>

            </section>

        </div>
    </section>
</template>

<script>
import MainCategories from '~/components/Categories/MedicalMainCategories'
import SliderMedical from '~/components/Vendor/SliderMedical'

export default {
    components: {
        appMainCategories: MainCategories,
        appSliderMedical: SliderMedical
    },
    data() {
        return {

        }
    }
}
</script>