<template>
    <section class="profile-page">
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="menu">
                        <div class="head">
                            <div class="profile-img">
                                <img :src="image" alt="">
                            </div>
                            <div class="title">
                                <h4>Tom Hanks</h4>
                                <div class="form-group">
                                    <label for="profile">Upload Photo</label>
                                    <input
                                        type="file"
                                        class="form-control"
                                        id="profile"
                                        @change="onImagePicked($event)"
                                        hidden
                                    />
                                </div>
                            </div>
                        </div>
                        <ul>
                            <li>
                                <nuxt-link to="/eg-en/profile" exact>
                                    <img class="icon" src="/images/icons/svg/profile-user.svg" alt="">
                                    <span>Account Info</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/eg-en/profile/wishlist">
                                    <img class="icon" src="/images/icons/svg/profile-heart.svg" alt="">
                                    <span>Wishlist</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/eg-en/profile/orders">
                                    <img class="icon" src="/images/icons/svg/profile-cart.svg" alt="">
                                    <span>Orders</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/eg-en/profile/user-reservations">
                                    <img class="icon" src="/images/icons/svg/profile-doctor.svg" alt="">
                                    <span>Reservations</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/eg-en/profile/subscribed-auctions">
                                    <img class="icon" src="/images/icons/svg/profile-auction.svg" alt="">
                                    <span>Subscribed Auctions</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/eg-en/profile/my-auctions">
                                    <img class="icon" src="/images/icons/svg/profile-auction.svg" alt="">
                                    <span>My Auctions</span>
                                    <img class="arrow" src="/images/icons/svg/profile-arrow.svg" alt="">
                                </nuxt-link>
                            </li>
                        </ul>
                        <div class="logout">
                            <button class="btn">Log out</button>
                        </div>
                    </div>
                </div>
                <div class="col-8">
                    <div class="profile-content">
                        <nuxt-child></nuxt-child>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    layout: 'withoutNavbar',
    data() {
        return {
            image: "https://orbitermag.com/wp-content/uploads/2017/03/default-user-image-300x300.png",
        }
    },
    methods: {
        onImagePicked(event) {
            console.log("picked");
            let file = event.target.files[0];

            if (file) {
                const fileReader = new FileReader();
                fileReader.addEventListener("load", () => {
                this.image = fileReader.result;
                console.log("image >> ", this.image);
                });
                fileReader.readAsDataURL(file);
            }
        },
    }
}
</script>