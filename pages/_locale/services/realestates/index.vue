<template>
    <div class="realestates">
        <div class="row">
            <div class="col-4" v-for="realestate in 9" :key="realestate">
                <app-single-realestate></app-single-realestate>
            </div>
        </div>
    </div>
</template>

<script>
import SingleRealestate from '~/components/Vendor/SingleRealestate';

export default {
    components: {
        appSingleRealestate: SingleRealestate
    },
    data () {
        return {

        }
    }
}
</script>