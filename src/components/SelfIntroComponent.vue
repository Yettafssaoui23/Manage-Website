<script>
export default {
    data() {
        return {
            selfIntroContent: 'Software student engineer at the Faculty of Science and Technologies Marrakech (FSTG)'
        }
    }
}
</script>

<template>
    <div class="p-4 p-md-5 mb-4 text-white rounded bg-dark">
        <div class="col-md-12 px-2">
            <h1 class="display-4 fst-italic">Hello, I am Youssef. Welcome to My Portfolio.</h1>
            <p class="my-3">{{ selfIntroContent }}</p>
        </div>
    </div>
</template>