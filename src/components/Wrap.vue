<script>
export default {

}

</script>

<template>
    <div class="wrap">
        <div class="container">
            <div class="wrap-inner">
                <h1>MTUCI</h1>
                <p>Московский Технический Университет Связи и Информатики</p>
            </div>
        </div>
    </div>



</template>

<style scoped>
.wrap {
    margin-bottom: 10em;
}

.wrap-inner {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 2em;
}

h1 {
    font-size: 22rem;
    font-weight: 800;
    color: var(--viol);
    margin: .2em 0 .3em 0;
}

p {
    color: gray;
    font-size: 44px;
    letter-spacing: -1px;
    line-height: 120%;
    text-align: center;
}


@media screen and (min-width: 2300px) {
    h1 {
        font-size: 42rem;
        margin: .1em 0 .1em 0;
    }

    p {
        font-size: 75px;
    }

}

@media screen and (max-width: 1300px) {
    h1 {
        font-size: 18rem;
    }

    br {
        display: none;
    }
}

@media screen and (max-width: 1024px) {
    h1 {
        display: none;
    }

    p {
        font-size: 30px;
        margin-top: 5em;
    }


}

@media screen and (max-width: 768px) {

    p {
        font-size: 30px;
        text-align: left;
        font-weight: 700;
    }


}
</style>