<template>
    <div class="account-info">
        <div class="head">
            <h3>Account Info</h3>
            <button class="btn">Save Changes</button>
        </div>
        <div class="account-form">
            <div class="form-row justify-content-between">
                <div class="form-group col-md-6">
                    <label for="firstName">First Name</label>
                    <input
                    type="text"
                    class="form-control form-control-lg"
                    id="firstName"
                    />
                </div>
                <div class="form-group col-md-6">
                    <label for="lastName">Last Name</label>
                    <input
                    type="text"
                    class="form-control form-control-lg"
                    id="lastName"
                    />
                </div>
                <div class="form-group col-md-6">
                    <label for="email">Email</label>
                    <input
                    type="text"
                    class="form-control form-control-lg"
                    id="email"
                    />
                </div>
                <div class="form-group col-md-6">
                    <label for="phone">Mobile Number</label>
                    <input
                    type="text"
                    class="form-control form-control-lg"
                    id="phone"
                    />
                </div>
                <div class="form-group col-md-6">
                    <label for="password">Password</label>
                    <input
                    type="password"
                    class="form-control form-control-lg"
                    id="password"
                    />
                </div>
                <div class="form-group col-md-6">
                    <label for="country">Country</label>
                    <select id="country" class="form-control form-control-lg">
                        <option>Egypt</option>
                        <option>syria</option>
                    </select>
                </div>
                <div class="form-group col-md-6">
                    <label for="governorate">Governorate</label>
                    <select id="governorate" class="form-control form-control-lg">
                        <option>Egypt</option>
                        <option>syria</option>
                    </select>
                </div>
                <div class="form-group col-md-6">
                    <label for="city">City</label>
                    <select id="city" class="form-control form-control-lg">
                        <option>Egypt</option>
                        <option>syria</option>
                    </select>
                </div>
                <div class="form-group col-md-12">
                    <label for="address">Address</label>
                    <input
                    type="text"
                    class="form-control form-control-lg"
                    id="address"
                    />
                </div>
            </div>
        </div>
    </div>
</template>