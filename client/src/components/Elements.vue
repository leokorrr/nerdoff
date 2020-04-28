<template>
    <div>
        <h1 class="header-1">Header 1</h1>
        <h2 class="header-2">Header 2</h2>
        <h3 class="header-3">Header 3</h3>
        <a href="#" class="link">link</a>
        <br>
        <button class="project-btn">Sign in</button>
        <button class="project-btn project-btn--red">Delete</button>
        <form>
            <div class="form-label"><label for="fname">First name:</label></div>
            <input type="text" id="fname" name="fname" class="form-input">
            <br>
            <label for="select" class="sr-only">First name:</label>
            <select id="select" class="form-input form-select">
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="mercedes">Mercedes</option>
                <option value="audi">Audi</option>
            </select>
            <br>
            <label for="textarea" class="sr-only">First name:</label>
            <textarea id="w3mission" rows="4" cols="50" class="form-input form-textarea">
                At w3schools.com you will learn how to make a website. We offer free tutorials in all web development technologies.
            </textarea>
        </form>
        <div class="tag">
            <div>Lol</div>
            <div class="tag__close"><img src="../img/icons/close.svg" alt=""></div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'Elements',
    props: {
        msg: String
    }
}
</script>

