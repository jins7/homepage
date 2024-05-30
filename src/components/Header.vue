<template>
    <section class="sticky-top">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="container-fluid" style="text-align: center;">
                <div class="navbar-brand" style="font-size: 25px;">Homepage</div>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                    aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#About"
                                style="font-size: 22px;">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#Publications"
                                style="font-size: 22px;">Publications</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#Education"
                                style="font-size: 22px;">Education</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                                data-bs-toggle="dropdown" aria-expanded="false" style="font-size: 22px;">
                                Other
                            </a>
                            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                                <li>
                                    <a class="dropdown-item" href="#Academic" style="font-size: 22px;">Academic
                                        Service</a>
                                </li>
                                <li>
                                    <a class="dropdown-item" href="#Award" style="font-size: 22px;">Award</a>
                                </li>
                                <li>
                                    <a class="dropdown-item" href="#Work" style="font-size: 22px;">Work Experience</a>
                                </li>
                                <li>
                                    <hr class="dropdown-divider">
                                </li>
                                <li>
                                    <a class="dropdown-item" href="#Interests" style="font-size: 22px;">Interests</a>
                                </li>
                                <li>
                                    <a class="dropdown-item" href="#Friends" style="font-size: 22px;">Friends</a>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </section>

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