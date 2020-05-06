<template>
    <div class="menu">
        <div class="menu__header">
            <h1 class="menu__title"><span class="color-purple">Nerd</span>Off</h1>
        </div>
        <div class="menu__actions">
            <div class="menu__action"><button class="project-btn">Create post</button></div>
            <div class="menu__action"><button class="menu__icon-btn"><img src="../../img/icons/notification.svg" alt=""></button></div>
            <div class="menu__action"><button class="menu__icon-btn" @click="showSidemenu"><img src="../../img/icons/menu-icon.svg" alt=""></button></div>
        </div>
        <div class="sidemenu-ctn" v-if="isSidemenuOpened" @click="hideSidemenu">
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
                    <li class="sidemenu__nav-item" @click="showFriends">
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
            <div class="friends" v-if="isFriendsOpened">
                <div class="friends__header">
                    <img src="../../img/icons/arrow-back.svg" alt="" @click="hideFriends">
                </div>
                <div class="friends__header">@TODO ADD SEARCHBAR</div>
                <ul class="friends__nav-list">
                    <li class="friends__nav-item">
                        <a href="#" class="friends__link">
                            <img src="../../img/avatar.svg" alt="post">
                            <span class="friends__link-text">Friend 1 <span class="friends__online"></span></span>
                        </a>
                    </li>
                    <li class="friends__nav-item">
                        <a href="#" class="friends__link">
                            <img src="../../img/avatar.svg" alt="post">
                            <span class="friends__link-text">Friend 2 <span class="friends__online"></span></span>
                        </a>
                    </li>
                    <li class="friends__nav-item">
                        <a href="#" class="friends__link">
                            <img src="../../img/avatar.svg" alt="post">
                            <span class="friends__link-text">Friend 3 <span class="friends__online"></span></span>
                        </a>
                    </li>
                    <li class="friends__nav-item">
                        <a href="#" class="friends__link">
                            <img src="../../img/avatar.svg" alt="post">
                            <span class="friends__link-text">Friend 4 <span class="friends__online"></span></span>
                        </a>
                    </li>
                    <li class="sidemenu__nav-item"><button class="project-btn">Create post</button></li> 
                </ul>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Menu',
    data() {
        return {
            isSidemenuOpened: false,
            isFriendsOpened: false
        }
    },
    methods: {
        showSidemenu() {
            this.isSidemenuOpened = true;
        },
        hideSidemenu(e) {
            if (e.target.classList.contains('sidemenu-ctn')) {
                this.isSidemenuOpened = false;
                this.isFriendsOpened = false;
            }
        },
        showFriends() {
            this.isFriendsOpened = true;
        },
        hideFriends() {
            this.isFriendsOpened = false;
        }
    }    
}
</script>