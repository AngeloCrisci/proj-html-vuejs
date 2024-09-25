<script>
export default {
    name: 'MainLeagueTable',
    props: {

    },
    data() {
        return {

        }
    }
}
</script>

<template>
<div class="container d-flex main-container bg-primary gap-5">
    <div class="league-table d-flex flex-column">
        <div class="title d-flex justify-content-center">
            <h1>League Table</h1>
        </div>
        <div class="main-table">
            <div></div>
        </div>
    </div>

    <div class="fixtures-results d-flex">
        <div class="title d-flex justify-content-center">
            <h1>Fixtures & Results</h1>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
.main-container {
    padding: 0;
    .league-table{
        flex-basis: 50%;
        background-color: red;
    }
    .fixtures-results {
        flex-basis: 50%;
        background-color: green;
    }
}

.title, .main-table {
    width: 100%;
}
</style>