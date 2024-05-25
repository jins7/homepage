<template>
    <div class="item">
        <div style="height: 100px;"></div>
        <div class="title" id="Publications">
            <div style="margin-left: 350px; margin-right: 350px;">
                <h1>Selected Publications</h1>
                <hr>
                <div v-for="item in publications" class="card mb-3" style="max-width: 1000px; border: none;">
                    <div class="row no-gutters">
                        <div class="col-md-5">
                            <img :src="item.img" alt="..." style="height: 300px; width: 400px;">
                        </div>
                        <div class="col-md-7">
                            <div class="card-body">
                                <h5 class="card-title">{{ item.name }}</h5>
                                <p class="card-text" style="font-size: 17px;">
                                    {{ item.writers }}
                                </p>
                                <p class="card-text" style="font-size: 17px;">{{ item.type }}</p>
                                <table>
                                    <tr>
                                        <td>
                                            <img src="../assets/icon/paper.png" alt=""
                                                style="height: 23px; width: 23px;">

                                            <a :href="item.paperUrl"
                                                style="font-size: 17px; text-decoration: none; color: #000;">paper</a>
                                        </td>
                                        <td>
                                            <img src="../assets/icon/paper.png" alt=""
                                                style="height: 23px; width: 23px;">

                                            <a :href="item.codeUrl"
                                                style="font-size: 17px; text-decoration: none; color: #000;">code</a>
                                        </td>
                                        <td>
                                            <img src="../assets/icon/paper.png" alt=""
                                                style="height: 23px; width: 23px;">
                                            <a :href="item.OpenReviewUrl"
                                                style="font-size: 17px; text-decoration: none; color: #000;">OpenReview</a>
                                        </td>
                                    </tr>
                                </table>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            publications: [
                {
                    name: 'publication1',
                    writers: 'Jack Marry Tom Mike Kite...',
                    type: 'Conference1',
                    paperUrl: 'https://github.com/',
                    codeUrl: 'https://github.com/',
                    OpenReviewUrl: 'https://github.com/',
                    img: 'src/static/people.png'
                },
                {
                    name: 'publication2',
                    writers: 'Jack Tom Mike Kite...',
                    type: 'Conference2',
                    paperUrl: 'https://github.com/',
                    codeUrl: 'https://github.com/',
                    OpenReviewUrl: 'https://github.com/',
                    img: 'src/static/people.png'
                },
                {
                    name: 'publication3',
                    writers: 'Jack Mike Kite...',
                    type: 'Conference3',
                    paperUrl: 'https://github.com/',
                    codeUrl: 'https://github.com/',
                    OpenReviewUrl: 'https://github.com/',
                    img: 'src/static/people.png'
                }
            ]
        }
    },
}
</script>