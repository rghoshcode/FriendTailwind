<template>
    <li class="h-48 bg-indigo-400 items-center p-5 w-1/4 mr-8 text-center flex flex-col justify-between">
        <h2 v-html="name"></h2>
        <ul v-if="detailsAreVisible" >
            <li class="flex justify-center">
                <strong>Phone:</strong>
                <div v-html="phone"></div>
            </li>
            <li class="flex justify-center">
                <strong>Email:</strong>
                <div v-html="email"></div>
            </li>
        </ul>
        <button @click="toggleDetails" class="bg-green-400 p-2 text-center">{{!this.detailsAreVisible? `Show Details` : `Hide Details` }}</button>

    </li>
</template>

<script>
    export default {
        props: ['id', 'name', 'phone', 'email'],
        data() {
            return {
                detailsAreVisible: false,
            };
        },
        methods: {
            toggleDetails() {
                this.detailsAreVisible = !this.detailsAreVisible;
            }
        }
    };
</script>