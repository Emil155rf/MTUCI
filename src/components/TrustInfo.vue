<script>
export default {

}
</script>

<template>
    <div class="trust-container">
        <div class="container">
            <div class="trust-grid">
                <div class="info">
                    <h1>>13000</h1>
                    <p>Студентов</p>
                </div>
                <div class="info">
                    <h1>>1500</h1>
                    <p>Бюджетных мест</p>
                </div>
                <div class="info">
                    <h1>>200</h1>
                    <p>Компаний партнеров</p>
                </div>
                <div class="info">
                    <h1>>100</h1>
                    <p>Лабораторий</p>
                </div>
            </div>
        </div>
    </div>


</template>

<style scoped>
.trust-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-attachment: local;
    background-image: radial-gradient(ellipse at 50% 10rem, var(--viol), #0000 70%);
    background-position: bottom;
    background-color: #040404;
    background-repeat: no-repeat;
    height: 500px;
    background-size: 100% 25%;
    margin-top: 3em;

}

.trust-grid {
    display: grid;
    justify-content: center;
    align-items: center;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 180px;
    grid-row-gap: 50px;
    
    text-align: center;

}

.info {
    color: #fff;
}

h1 {
    font-size: 50px;
    padding-bottom: 10px;
}

p {
    font-size: 25px;
}


@media screen and (min-width: 2100px) {
    .trust-container {
        height: 700px;
    }

    .trust-grid {
        grid-row-gap: 100px;

    }

    h1 {
        font-size: 70px;
    }

    p {
        font-size: 35px;
    }

}


@media screen and (max-width: 768px) {
    .trust-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-column-gap: 50px;
        grid-row-gap: 50px;
    }

    h1 {
        font-size: 35px;
    }

    p {
        font-size: 20px;
    }

}


@media screen and (max-width: 500px) {
    .trust-grid {
        grid-column-gap: 30px;
    }

}

@media screen and (max-width: 400px) {
    .trust-grid {
        grid-column-gap: 10px;
    }

}

@media screen and (max-width: 360px) {
    .trust-grid {
        display: grid;
        grid-template-columns: 1fr;
        text-align: center;
    }

}
</style>
