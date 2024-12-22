<script>
export default {

}


</script>


<template>
    <div id="dev" class="container">
        <div class="line"></div>
        <div class="dev-title">
            <h1>Развиваем:</h1>
        </div>
    </div>


</template>

<style scoped>
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

@media screen and (min-width: 2100px) {
    h1 {
        font-size: 110px;
    }
}

@media screen and (max-width: 768px) {
    h1 {
        font-size: 40px;
    }
}
</style>