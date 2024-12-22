<script>
export default {

}

</script>


<template>
    <div class="org">
        <div class="container">
            <div class="org-partners">
                <h1>Проверены временем</h1>
                <p>Университет уже 103 года выпускает настоящих профессионалов разных отраслей. <br> <a href="https://mtuci.ru/?ysclid=m4l0qu1322873525756">познакомься</a> с нами ближе, узнай о факультетах, проходных баллах.</p>
            </div>
            <div class="end">
                <p class="more">И о многом другом...</p>
            </div>
        </div>
    </div>



</template>


<style scoped>
.org {
    margin: 6em 0 4em 0;
}

h1 {
    color: var(--color-text);
    font-size: 68px;
    font-family: 'Involve Bold';
    margin-top: .5em;
}

.org-partners {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.org-partners p {
    font-size: 32px;
    color: var(--color-name);
    margin-top: 1em;
    line-height: 1.3;
    text-decoration: underline;
    text-decoration-skip-ink: none;
    text-underline-offset: 5px;
}

.org-partners a {
    font-size: 32px;
    color: var(--viol);

}
.org-partners a:hover {
    color: var(--color-text);
    transition: .2s ease;
}

.end {
    display: flex;
    justify-content: right;
    align-items: flex-end;
    margin-top: 5em;
}

.more {
    font-size: 30px;
    color: var(--color-text);
}

@media screen and (min-width: 2100px) {
    h1 {
        font-size: 110px;
    }

    .org-partners p {
        font-size: 65px;
    }

    .end p {
        font-size: 55px;
    }

}

@media screen and (max-width: 768px) {
    h1 {
        font-size: 40px;
    }

    .org-partners p {
        font-size: 30px;
    }

}
</style>