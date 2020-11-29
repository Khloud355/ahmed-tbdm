<template>
    <div class="professions-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item active" aria-current="page">Profession</li>
                </ol>
            </nav>

            <app-main-categories></app-main-categories>

            <nuxt-child></nuxt-child>

        </div>
    </div>
</template>

<script>
import MainCategories from '~/components/Categories/ProfessionsMainCategories';
import SliderProfession from '~/components/Vendor/SliderProfession';

export default {
    components: {
        appMainCategories: MainCategories,
        appSliderProfession: SliderProfession
    }
}
</script>