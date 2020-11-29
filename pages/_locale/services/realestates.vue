<template>
    <section class="realestates-page">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
                    <li class="breadcrumb-item"><nuxt-link to="/">Services</nuxt-link></li>
                    <li class="breadcrumb-item active" aria-current="page">Realestates</li>
                </ol>
            </nav>

            <div class="realestates-filter">
                <div class="form-row">
                    <div class="form-group col-md-3">
                        <label for="specialization">Type</label>
                        <select id="specialization" class="form-control form-control-lg">
                            <option>Egypt</option>
                            <option>syria</option>
                        </select>
                    </div>
                    <div class="form-group col-md-3">
                        <label for="specialization">Finishing</label>
                        <select id="specialization" class="form-control form-control-lg">
                            <option>Egypt</option>
                            <option>syria</option>
                        </select>
                    </div>
                    <div class="form-group col-md-3">
                        <label for="specialization">Furnishing</label>
                        <select id="specialization" class="form-control form-control-lg">
                            <option>Egypt</option>
                            <option>syria</option>
                        </select>
                    </div>
                    <div class="form-group col-md-3">
                        <label for="specialization">Category</label>
                        <select id="specialization" class="form-control form-control-lg">
                            <option>Egypt</option>
                            <option>syria</option>
                        </select>
                    </div>

                    <div class="form-group col-md-3">
                        <div class="chiller_cb">
                            <input id="garden" type="checkbox">
                            <label for="garden">Garden</label>
                            <span></span>
                        </div>
                    </div>
                    <div class="form-group col-md-3">
                        <div class="chiller_cb">
                            <input id="maid" type="checkbox">
                            <label for="maid">Maid Service</label>
                            <span></span>
                        </div>
                    </div>
                    <div class="form-group col-md-3">
                        <div class="chiller_cb">
                            <input id="security" type="checkbox">
                            <label for="security">Security</label>
                            <span></span>
                        </div>
                    </div>
                    <div class="form-group col-md-3">
                        <div class="chiller_cb">
                            <input id="parking" type="checkbox">
                            <label for="parking">Parking</label>
                            <span></span>
                        </div>
                    </div>

                </div>

                <div class="filter-btn">
                    <button class="btn">Filter</button>
                </div>

            </div>

            <app-main-categories></app-main-categories>

            <nuxt-child></nuxt-child>

            <div class="paginator">
                <div class="overflow-auto">
                    <b-pagination-nav :link-gen="linkGen" :limit="10" :hide-goto-end-buttons="true" :number-of-pages="10" align="center" use-router>
                        <template #prev-text><span><img src="/images/icons/svg/chevron-left.svg" alt=""></span></template>
                        <template #next-text><span><img src="/images/icons/svg/chevron-right.svg" alt=""></span></template>
                    </b-pagination-nav>
                </div>
            </div>

        </div>
    </section>
</template>

<script>
import MainCategories from '~/components/Categories/RealestateMainCategories';
import SingleRealestate from '~/components/Vendor/SingleRealestate';

export default {
    components: {
        appMainCategories: MainCategories,
        appSingleRealestate: SingleRealestate
    },
    data () {
        return {

        }
    },
    methods: {
      linkGen(pageNum) {
        return pageNum === 1 ? '?' : `?page=${pageNum}`
      }
    }
}
</script>