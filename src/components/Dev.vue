<script>
export default {

}


</script>

<template>
    <div class="container">
        <div class="develop">
            <div class="develop-card">
                <div class="card">
                    <h1>IT-индустрию</h1>
                    <p>МТУСИ — лидер в подготовке ИТ-специалистов, активно развивающий образовательные программы в
                        соответствии с потребностями рынка. Университет внедряет инновационные технологии обучения и
                        тесно сотрудничает с ведущими компаниями отрасли. </p>
                </div>
                <div class="card">
                    <h1>Сетевые технологии</h1>
                    <p>МТУСИ является ведущим центром подготовки в области сетевых технологий. Университет активно
                        сотрудничает с
                        отраслевыми компаниями, предоставляя студентам доступ к реальным
                        проектам.</p>
                </div>
                <div class="card">
                    <h1>Soft-skills</h1>
                    <p>МТУСИ уделяет большое внимание развитию soft skills у студентов, интегрируя их в учебные
                        программы и внеучебную деятельность. Университет предлагает различные курсы, тренинги и
                        мастер-классы, направленные на развитие коммуникативных навыков,</p>
                </div>
                <div class="card">
                    <h1>Отношения с партнерами</h1>
                    <p>МТУСИ активно развивает сотрудничество с ведущими ИТ-компаниями, создавая площадки для
                        совместных проектов, стажировок и трудоустройства студентов. Партнерство обеспечивает доступ
                        к передовым технологиям и актуальным задачам отрасли, </p>
                </div>
            </div>
        </div>
    </div>



</template>

<style scoped>
.develop {
    display: flex;
    justify-content: center;
    align-items: center;
}
.develop-card {
    display: grid;
    justify-content: space-between;
    align-items: center;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 100px;
    grid-row-gap: 50px;

    margin-top: 4em;
}

.card {
    display: flex;
    flex-direction: column;
    text-align: left;
    border: 2px solid var(--color-text);
    cursor: pointer;
    padding: 40px;
    height: 100%;
    width: 100%;
    overflow: hidden;
}

.card:hover {
    background-color: var(--viol);
    transition: .2s ease;
}

.card h1 {
    font-size: 22px;
    font-family: 'Involve Bold';
    color: var(--color-text);

}

.develop p {
    font-size: 20px;
    font-family: 'Involve Bold';

}

.card p {
    font-size: 18px;
    font-family: 'Involve Bold';
    color: var(--color-name);
    padding-top: 20px;

}

.compet {
    display: flex;
    flex-direction: row;
    margin-top: 5em;
}

@media screen and (max-width: 768px) {
    .develop-card {
        display: grid;
        grid-template-columns: 1fr;
    }
    
}
</style>