<script>
import { ref } from 'vue';


export default {
    setup() {
        const isAnimated = ref(false)
        const theme = ref('light')
        const isHidden = ref(false)
        let prevScrollPos = window.scrollY


        const toggleTheme = () => {
            theme.value = theme.value === 'light' ? 'dark' : 'light'
            document.body.classList.toggle('dark')
            isAnimated.value = !isAnimated.value
        }
        const handleScroll = () => {
            const currentScrollPos = window.scrollY
            if (prevScrollPos > currentScrollPos) {
                isHidden.value = false
            } else if (currentScrollPos > 200) {
                isHidden.value = true
            }

            prevScrollPos = currentScrollPos
        }

        window.addEventListener('scroll', handleScroll)

        return {
            isAnimated,
            toggleTheme,
            theme,
            isHidden,
            headerItems: [
                { label: 'О нас', id: 'aboutUs' },
                { label: 'перспективы', id: 'dev' },
                { label: 'преимущества', id: 'services' },
                { label: 'контакты', id: 'contacts' }
            ],
            scrollToSection(index) {
                const sectionId = this.headerItems[index].id
                const sectionElement = document.getElementById(sectionId)
                if (sectionElement) {
                    sectionElement.scrollIntoView({ behavior: 'smooth' })
                }
            }
        }
    }
}
</script>


<template>
    <div class="header" :class="{ 'hidden': isHidden }"
        :style="{ transform: isHidden ? 'translateY(-100%)' : 'translateY(0)' }">
        <div class="container">
            <div class="header-inner">
                <div class="header-list">
                    <ul>
                        <li v-for="(item, index) in headerItems" :key="index" @click="scrollToSection(index)">
                            <button class="project-btn">{{ item.label }}</button>
                        </li>
                    </ul>
                </div>
                <div class="header-h1">
                    <h1>MTUCI</h1>
                </div>
                <div class="header-buttons">
                    <button class="button connect-btn">Обсудить с нами</button>

                    <button class="toggle-btn" :class="{ active: isAnimated }" @click="toggleTheme">
                        <i class="bi bi-circle-fill" :class="{ moved: isAnimated }"></i>
                    </button>
                </div>
            </div>
        </div>
    </div>




</template>


<style scoped>
.header {
    position: fixed;
    width: 100%;
    height: 80px;
    background-color: var(--back);
    z-index: 9999;
    transition: transform 0.5s ease-in-out;

}

.header.hidden {
    transform: translateY(-80px);

}

h1 {
    font-size: 3rem;
    font-weight: 700;
    color: var(--viol);
}

.header-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
    color: var(--color-text);
}


.header-list ul {
    display: flex;
}

.header-list li {
    margin-right: 1em;
}

.header-list button {
    font-family: 'Involve Bold';
    font-size: 20px;
    text-transform: uppercase;
    color: var(--color-text);
    background-color: transparent;
}

.header-list button:hover {
    color: var(--color-name);
    transition: .2s ease;
}

.header-buttons {
    display: flex;
    align-items: center;
}

.connect-btn {
    padding: 7px 20px;
    margin-right: 1em;
    background-color: var(--viol);
    color: var(--color-text);
    border-radius: 10px;
}

.connect-btn:hover {
    background-color: var(--color-text);
    color: var(--viol);
    font-weight: 800;
    transition: .5s ease;
}

.toggle-btn {
    width: 80px;
    height: 43px;
    background-color: var(--color-head);
    border-radius: 100px;
    display: flex;
    cursor: pointer;
    transition: background-color 0.3s ease;

}

.bi-circle-fill {
    position: relative;
    bottom: 2px;
    font-size: 33px;
    padding-left: 5px;
    color: var(--back);
    transition: transform 0.3s ease, color 0.5s ease;
}


.toggle-btn.active i.moved {
    transform: translateX(100%);
}

@media screen and (min-width: 2100px) {
    .header {
        height: 120px;
    }
    .header-list button {
        font-size: 35px;
    }

    .connect-btn {
        font-size: 35px;
    }

    .toggle-btn {
        width: 118px;
        height: 70px;

    }

    .bi-circle-fill {
        font-size: 52px;
        padding-left: 5px;
    }

}

@media screen and (max-width: 1024px) {
    .header-list {
        display: none;
    }


}

@media screen and (min-width: 1025px) {
    h1 {
        display: none;
    }

}

@media screen and (max-width: 650px) {
    .connect-btn {
        display: none;
    }

    h1 {
        font-size: 32px;
    }

    .bi-circle-fill {
        position: relative;
        top: 2.5px;
    }

}
</style>