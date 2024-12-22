<script>
export default {


}

</script>

<template>
    <div id="services" class="trust">
        <div class="container">
            <div class="line"></div>
            <div class="trust-partners">
                <h1>Нам доверяют</h1>
                <p>Работаем совместно с крупными компаниями. <br> Доказываем профессионализм не на словах, а на деле.
                </p>
            </div>
        </div>
    </div>


</template>

<style scoped>
.trust {
    margin-top: 5em;
}

.line {
    height: 1px;
    background-color: var(--color-name);
    opacity: .5;
}

h1 {
    color: var(--color-text);
    font-size: 68px;
    font-family: 'Involve Bold';
    margin-top: .5em;
}

.trust-partners {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.trust-partners p {
    font-size: 32px;
    color: var(--color-name);
    margin-top: 1em;

}

@media screen and (min-width: 2100px) {
    h1 {
        font-size: 110px;
    }

    .trust-partners p {
        font-size: 65px;
    }

}

@media screen and (max-width: 768px) {
    h1 {
        font-size: 40px;
    }

    .trust-partners p {
        font-size: 25px;
    }

}
</style>