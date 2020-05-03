<template>
    <div class="sidemenu">
        <div class="sidemenu__header">
            <h2 class="sidemenu__title"><span class="color-purple">Nerd</span>Off</h2>
        </div>
        <ul class="sidemenu__nav-list">
            <li class="sidemenu__nav-item">
                <a href="#" class="sidemenu__link">
                    <img src="../../img/icons/post.svg" alt="post">
                    <span class="sidemenu__link-text">Posts</span>
                </a>
            </li>
            <li class="sidemenu__nav-item">
                <a href="#" class="sidemenu__link">
                    <img src="../../img/icons/person.svg" alt="post">
                    <span class="sidemenu__link-text">My profile</span>
                </a>
            </li>
            <li class="sidemenu__nav-item">
                <a href="#" class="sidemenu__link">
                    <img src="../../img/icons/friends.svg" alt="post">
                    <span class="sidemenu__link-text">Friends</span>
                </a>
            </li>
            <li class="sidemenu__nav-item">
                <a href="#" class="sidemenu__link">
                    <img src="../../img/icons/logout.svg" alt="post">
                    <span class="sidemenu__link-text">Log out</span>
                </a>
            </li>
            <li class="sidemenu__nav-item"><button class="project-btn">Create post</button></li> 
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Sidemenu'
}
</script>