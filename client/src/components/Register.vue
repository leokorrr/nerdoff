<template>
    <div class="register">
        <div class="register__form-ctn">
            <div class="register__form">
                <div class="register__title">
                    <h1 class="header-1">Get started for free</h1>
                </div>
                <form>
                    <div class="register__form-input">
                        <img src="../img/icons/person.svg" alt="">
                        <label for="email" class="sr-only">Email</label>
                        <input type="email" id="email" class="form-input" placeholder="Email">
                    </div>
                    <div class="register__form-input">
                        <img src="../img/icons/lock.svg" alt="">
                        <label for="password" class="sr-only">Password</label>
                        <input type="password" id="password" class="form-input" placeholder="Password">
                    </div>
                    <div class="register__submit-btn-ctn">
                        <button class="project-btn" type="submit">Next</button>
                    </div>
                </form>
                <div class="register__actions">
                    <div>Have an account? <a href="#" class="link">Log in</a></div>
                    <div><a href="#" class="link">Forgot password?</a></div>
                </div>
                <form>
                    <div class="register__form-input register__form-input--full-width">
                        <label for="name" class="sr-only">Name</label>
                        <input type="name" id="name" class="form-input" placeholder="Name">
                    </div>
                    <div class="register__form-row">
                        <div class="register__form-input register__form-input--half-width">
                            <label for="age" class="sr-only">Age</label>
                            <input type="age" id="age" class="form-input" placeholder="Age">
                        </div>
                        <div class="register__form-input register__form-input--half-width">
                            <label for="gender" class="sr-only">Gender</label>
                            <select id="gender" class="form-input form-select" placeholder="Gender">
                                <option value="volvo">Man</option>
                                <option value="saab">Woman</option>
                                <option value="mercedes">Other</option>
                            </select>
                        </div>
                    </div>
                    <div class="register__form-input register__form-input--full-width">
                        <label for="password" class="sr-only">Location</label>
                        <input type="password" id="password" class="form-input" placeholder="Location">
                    </div>
                    <div class="register__submit-btn-ctn">
                        <button class="project-btn" type="submit">Next</button>
                    </div>
                </form>
                <form>
                    <div class="register__form-input register__form-input--full-width">
                        <label for="name" class="sr-only">Name</label>
                        <select id="gender" class="form-input form-select" placeholder="Gender">
                            <option @click="selectPassion" class="red" v-bind:class="{ active: isActive }" v-for="(passion, index) of passions" :key="index" :value="passion">{{passion}}</option>
                        </select>
                    </div>
                    <div class="register__selected-tags">
                        <div class="tag">
                            <div>Lol</div>
                            <div class="tag__close"><img src="../img/icons/close.svg" alt=""></div>
                        </div>
                        <div class="tag">
                            <div>Lol</div>
                            <div class="tag__close"><img src="../img/icons/close.svg" alt=""></div>
                        </div>
                        <div class="tag">
                            <div>Lol</div>
                            <div class="tag__close"><img src="../img/icons/close.svg" alt=""></div>
                        </div>
                    </div>
                    <div class="register__submit-btn-ctn">
                        <button class="project-btn" type="submit">Sign up</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Register',
    data() {
        return {
            passions: [
                'League of Legends',
                'Beer',
                'Sweets'
            ],
            selectedPassions: [],
            isActive: false
        }
    },
    methods: {
        selectPassion() {
            this.isActive = !this.isActive
            console.log('aaa')
        }
    }
}
</script>