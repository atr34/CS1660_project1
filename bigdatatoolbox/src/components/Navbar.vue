<template>
    <nav>
        <v-navigation-drawer app class="primary" v-model="drawer">
            <v-list>
                <v-list-item v-for="link in links" :key="link.text">
                    <v-list-item-action>
                        <v-icon class="white--text" @click="$router.push(`${link.route}`)">
                            {{ link.icon }}
                        </v-icon>
                    </v-list-item-action>
                    <v-list-item-content>
                        <v-list-item-title class="white--text">{{ link.text }}</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-navigation-drawer>        
        <v-app-bar flat app>
            <v-app-bar-nav-icon class="grey--text" @click="drawer=!drawer"></v-app-bar-nav-icon>
            <v-app-bar-title class="text-uppercase grey--text">
                <span class="font-weight-light">Welcome to Big Data Tool Box Application</span>
            </v-app-bar-title>
        </v-app-bar>
    </nav>
</template>

<script>
export default {
    data () {
        return {
            drawer: false,
            links: [
                { icon: 'folder', text: 'My Projects', route: '/projects' },
                { icon: 'person', text: 'Team', route: '/team' },                
            ]
        }
    }
}
</script>

<style>

</style>