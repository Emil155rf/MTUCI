<script>
export default {

}

</script>

<template>
    <div class="footer">
        <div class="container">
            <div class="footer-inner">
                <div class="footer-address">
                    <h1>МТУСИ</h1>
                    <p class="address-1">Москва 2024</p>
                    <p class="address-2">Москва <br> Авиамоторная ул., 8, стр. 2</p>
                </div>
                <div id="contacts" class="footer-contact">
                    <a href="tel:+74959577731">+7 (495) 957-77-31</a>
                    <a  href="mailto:mtuci@mtuci.ru">mtuci@mtuci.ru</a>
                </div>

            </div>
        </div>
    </div>


</template>

<style scoped>
.footer {
    background-color: #171717;
    height: 200px;
}

.footer-inner {
    color: #F8F8F8;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 3em;
}

.footer-address {
    display: flex;
    flex-direction: column;

}

.address-2 {
    display: none;
}

.footer-address h1 {
    text-transform: uppercase;
    font-size: 30px;
    margin-bottom: 10px;

}

.footer-contact {
    display: flex;
    flex-direction: column;
    text-align: right;
    color: var(--color-name);
}

.footer-contact a {
    font-size: 25px;
    margin-bottom: 10px;
}

.footer-contact a:hover {
    color: #F8F8F8;
    transition: .3s ease;
}

@media screen and (max-width: 1024px) {
    .address-1 {
        display: none;
    }

    .address-2 {
        display: flex;
        line-height: 25px;
    }

}

@media screen and (min-width: 1024px) {
    .address-1 {
        display: flex;
    }

    .address-2 {
        display: none;
    }


}

@media screen and (max-width: 768px) {
    .footer-inner {
        margin-top: 4em;
    }

    .footer-address h1 {
        font-size: 30px;

    }

    .footer-contact a {
        font-size: 20px;
    }

}

@media screen and (max-width: 500px) {
    .footer {
        height: 300px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .footer-inner {
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-top: 1.5em;
    }

    .footer-address {
        margin-bottom: 2em;
    }
    .footer-contact {
        text-align: center;
    }
}
</style>