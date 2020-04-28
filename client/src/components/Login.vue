<template>
    <div class="login">
        <div class="login__form-ctn">
            <div class="login__form">
                <div class="login__title">
                    <h1 class="header-1">Log in</h1>
                </div>
                <form>
                    <div class="login__form-input">
                        <img src="../img/icons/person.svg" alt="">
                        <label for="email" class="sr-only">Email</label>
                        <input type="email" id="email" class="form-input" placeholder="Email">
                    </div>
                    <div class="login__form-input">
                        <img src="../img/icons/lock.svg" alt="">
                        <label for="password" class="sr-only">Email</label>
                        <input type="password" id="password" class="form-input" placeholder="Password">
                    </div>
                    <div class="login__submit-btn-ctn">
                        <button class="project-btn" type="submit">Sign in</button>
                    </div>
                </form>
                <div class="login__actions">
                    <div>New account? <a href="#" class="link">Register</a></div>
                    <div><a href="#" class="link">Forgot password?</a></div>
                </div>
            </div>
        </div>
        <div class="login__img-ctn">
            <img src="../img/loginBG.svg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Login'
}
</script>