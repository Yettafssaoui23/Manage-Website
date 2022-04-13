<script>
export default {
    data() {
        return {
            navLinks: [
                { id: 1, name: 'Home', link: '#' },
                { id: 2, name: 'Features', link: '#' },
                { id: 3, name: 'Pricing', link: '#' },
                { id: 4, name: 'FAQs', link: '#' },
                { id: 5, name: 'About', link: '#' },
            ]
        }
    },

    props: ['websiteName']
}
</script>

<template>
    <header class="d-flex flex-wrap justify-content-center py-3 mb-4 border-bottom">
        <a
            href="/"
            class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none"
        >
            <span class="fs-4">{{ websiteName }}</span>
        </a>

        <ul class="nav nav-pills">
            <li class="nav-item" v-for="navLink in navLinks" v-bind:key="navLink.id">
                <a v-bind:href="navLink.link" class="nav-link">{{navLink.name}}</a>
            </li>
        </ul>
    </header>
</template>

<style>
</style>