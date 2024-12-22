<script>
export default {

}
</script>

<template>
    <div class="container">
        <div class="map-card">
            <h1>Наш адрес:</h1>
            <p>Москва <br> Авиамоторная ул., 8, <br> стр. 2</p>
            <div class="map-btn">
                <button><i class="bi bi-telegram"></i></button>
                <button><i class="bi bi-youtube"></i></button>
                <button><i class="bi bi-instagram"></i></button>
            </div>
        </div>
    </div>
    <iframe
        src="https://yandex.ru/map-widget/v1/?um=constructor%3A5fed11a1a8a1b0c0ab3717f387f775f482b2fa4a6bc15053ccc77cc793a5827c&amp;source=constructor"
        width="100%" height="400" frameborder="0"></iframe>

</template>

<style scoped>
.map-card {
    position: absolute;
    font-family: 'Involve Bold';
    background-color: #fff;
    padding: 50px;
    margin: 3em 0 0 4em;
    color: #020402;

}

.bi {
    font-size: 25px;
}

button {
    background-color: transparent;
    margin: 1em .7em 0 0;

}

.map-btn {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

h1 {
    color: var(--viol);
    padding-bottom: 1em;
}

p {
    font-size: 18px;
    line-height: 25px;

}

@media screen and (max-width: 1024px) {
    .map-card {
        display: none;
    }

}
</style>