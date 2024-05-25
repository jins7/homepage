<template>
    <div class="item">
        <div style="height: 100px;"></div>
        <div style="margin-left: 350px; margin-right: 350px;">
            <h1>News</h1>
            <hr>
            <ul>
                <li v-for="item in news">
                    {{ item.time }} : {{ item.event }}
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            news: [
                { time: ' Jan. 2024', event: 'even 1' },
                { time: ' Feb. 2023', event: 'even 2' },
                { time: ' Oct. 2021', event: 'even 3' },
                { time: ' Aug. 2021', event: 'even 4' },
            ]
        }
    }
}
</script>