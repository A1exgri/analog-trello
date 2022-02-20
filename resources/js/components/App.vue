<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="container">
                <ul class="navbar-nav">
                    <li class="nav-item active">
                        <router-link class="nav-link" :to="{ name: 'home'}">Главная</router-link>
                    </li>
                    <li class="nav-item active">
                        <router-link class="nav-link" :to="{ name: 'desks'}">Доски</router-link>
                    </li>
                </ul>
            </div>
        </nav>
        <p>

        </p>
        <div class="container">
            <router-view></router-view>
        </div>
    </div>
</template>

<script>
export default {
    name: "App"
}
</script>

