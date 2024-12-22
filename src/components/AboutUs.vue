<script>
export default {

}

</script>

<template>
    <div class="container">
        <div class="line"></div>
        <div id="aboutUs" class="about-text">
            <h1>Об Университете</h1>
            <p>МТУСИ – лидирующий университет в стране, научно-образовательная деятельность которого осуществляется в
                области телеком и IT-индустрии.</p>
        </div>
    </div>


</template>

<style scoped>
.line {
    height: 1px;
    background-color: var(--color-name);
    opacity: .5;
}

.bi {
    position: relative;
    bottom: 2px;
    margin: 0 2em;
    font-size: 30px;
}

.about-text {
    display: flex;
    justify-content: space-between;
}

.about-text h1 {
    color: var(--color-text);
    font-size: 68px;
    font-family: 'Involve Bold';
    margin-top: .5em;
}

.about-text p {
    font-size: 38px;
    color: var(--color-text);
    font-family: 'Involve Bold';
    max-width: 650px;
    margin-top: 1em;
    width: 100%;
}


img {
    height: 350px;
    border-radius: 25px;
}



@media screen and (min-width: 2100px) {
    .about-text h1 {
        font-size: 110px;
    }

    .about-text p {
        font-size: 65px;
        max-width: 1000px;
    }

}

@media screen and (max-width: 1024px) {
    .about-text {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        text-align: left;
    }

}



@media screen and (max-width: 768px) {
    .about-text h1 {
        font-size: 40px;
    }

    .about-text p {
        font-size: 28px;
    }


}


</style>