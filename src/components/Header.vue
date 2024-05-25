<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container-fluid" style="text-align: center;">
            <div class="navbar-brand" style="font-size: 25px;">Homepage</div>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a @click="goToAnchor('#About')" class="nav-link active" aria-current="page" href="#"
                            style="font-size: 22px;">About</a>
                    </li>
                    <li class="nav-item">
                        <a @click="goToAnchor('#Publications')" class="nav-link active" aria-current="page" href="#"
                            style="font-size: 22px;">Publications</a>
                    </li>
                    <li class="nav-item">
                        <a @click="goToAnchor('#Education')" class="nav-link active" aria-current="page" href="#"
                            style="font-size: 22px;">Education</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                            data-bs-toggle="dropdown" aria-expanded="false" style="font-size: 22px;">
                            Other
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li>
                                <a @click="goToAnchor('#Academic')" class="dropdown-item" href="#"
                                    style="font-size: 22px;">Academic Service</a>
                            </li>
                            <li>
                                <a @click="goToAnchor('#Award')" class="dropdown-item" href="#"
                                    style="font-size: 22px;">Award</a>
                            </li>
                            <li>
                                <a @click="goToAnchor('#Work')" class="dropdown-item" href="#"
                                    style="font-size: 22px;">Work Experience</a>
                            </li>
                            <li>
                                <hr class="dropdown-divider">
                            </li>
                            <li>
                                <a @click="goToAnchor('#Interests')" class="dropdown-item" href="#"
                                    style="font-size: 22px;">Interests</a>
                            </li>
                            <li>
                                <a @click="goToAnchor('#Friends')" class="dropdown-item" href="#"
                                    style="font-size: 22px;">Friends</a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    methods: {
        goToAnchor(selector) {
            document.querySelector(selector).scrollIntoView({
                behavior: "smooth", // 平滑过渡
                block: "start" // 上边框与视窗顶部平齐
            });
        }
    }
}
</script>