<script>
export default {
    name: "AppNavbar",
    data() {
        return {
            navLink : [
                {
                    path:"#",
                    text:"CHARACTERS",
                },
                {
                    path:"#",
                    text:"COMICS",
                },
                {
                    path:"#",
                    text:"MOVIE",
                },
                {
                    path:"#",
                    text:"TV",
                },
                {
                    path:"#",
                    text:"GAMES",
                },
                {
                    path:"#",
                    text:"VIDEOS",
                },
                {
                    path:"#",
                    text:"FANS",
                },
                {
                    path:"#",
                    text:"NEWS",
                },
                {
                    path:"#",
                    text:"SHOP",
                },
            ]
        }
    },
    methods: {
        
    },
}
</script>

<template>
    <div class="nav d-flex justify-content-between align-items-center">
        <div class="p-2">
            <img class="logo" src="../assets/dc-logo.png" alt="">
        </div>
        <div class="h-100 d-flex px-2">
            <div v-for="link in navLink" class="h-100 test d-flex align-items-center">
                <a :href="link.path"> {{ link.text}} </a>
            </div>
        </div>
    </div>
</template>

<style  scoped>
.logo:hover {
    rotate: 180deg;
    animation-name: Rotate;
    animation-duration: 3s;
}

@keyframes Rotate {
    0% {
        rotate: 0deg;
    }

    20% {
        rotate: 50deg;
    }

    30% {
        rotate: 100deg;
    }
    
    40% {
        rotate: 150deg;
    }

    50% {
        rotate: 200deg;
    }

    60% {
        rotate: 250deg;
    }

    70% {
        rotate: 300deg;
    }

    80% {
        rotate: 360deg;
    }

    90% {
        rotate: 0deg
    }
}

a {
    padding: 5px;
    font-weight: 800;
    color: #000;
    text-decoration: none;
}

a:hover {
    color: royalblue;
}

.test:hover {
    border-bottom: 2px solid royalblue;
}

.nav {
    height: 120px;
}</style>
