<script>
export default {
    data() {
        return {
            skills: [
                { id: 1, name: 'HTML & CSS', percentage: '100' },
                { id: 2, name: 'JavaScript', percentage: '90' },
                { id: 3, name: 'Laravel', percentage: '80' },
                { id: 4, name: 'Django', percentage: '70' },
            ]
        }
    }
}
</script>

<template>
    <div class="p-4 p-md-5 mb-4 rounded bg-light">
        <div class="row align-items-center">
            <h1 class="display-6">My Skills</h1>
            <ul class="list-group list-group-flush">
                <li class="list-group-item" v-for="skill in skills" v-bind:key="skill.id">
                    <p>{{ skill.name }}</p>
                    <div class="progress">
                        <div
                            class="progress-bar"
                            role="progressbar"
                            v-bind:style="{ width: skill.percentage + '%' }"
                            v-bind:aria-valuenow="skill.percentage"
                            aria-valuemin="0"
                            aria-valuemax="100"
                        >{{ skill.percentage }}%</div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>