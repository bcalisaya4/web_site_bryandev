
<script setup>
</script>
<template>
    <div style="padding: 0 10%;">
        <section class="education" id="education">
            <h2 class="heading">My <span>Journey</span></h2>

            <div class="education-row">
                <div class="education-column">
                    <h3 class="title">Education</h3>
                    <div class="education-box">
                        <div class="education-content">
                            <div class="content">
                                <div class="year">
                                    <img class="calendar-icon" src="src\assets\icons\calendar-icon.png" alt="Calendario">
                                     2017 - 2022
                                </div>
                                <h3>Master Degree - University</h3>
                                <p>
                                    Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                                    Dolore amet rem nulla voluptas temporibus, excepturi tempora
                                    repellendus eveniet sint sed maiores deleniti! Qui quis
                                    distinctio quo nam sunt commodi eveniet!
                                </p>
                            </div>
                        </div>
                        <!--div class="education-content">
                            <div class="content">
                                <div class="year">
                                    <img class="calendar-icon" src="src\assets\icons\calendar-icon.png" alt="Calendario">
                                     2017 - 2022
                                </div>
                                <h3>Master Degree - University</h3>
                                <p>
                                    Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                                    Dolore amet rem nulla voluptas temporibus, excepturi tempora
                                    repellendus eveniet sint sed maiores deleniti! Qui quis
                                    distinctio quo nam sunt commodi eveniet!
                                </p>
                            </div>
                        </div-->
                    </div>
                </div>
                <div class="education-column">
                    <h3 class="title">Experience</h3>
                    <div class="education-box">
                        <div class="education-content">
                            <div class="content">
                                <div class="year">
                                    <img class="calendar-icon" src="src\assets\icons\calendar-icon.png" alt="Calendario">
                                     2021 - 2023
                                </div>
                                <h3>Developer - VEOX</h3>
                                <p>
                                    Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                                    Dolore amet rem nulla voluptas temporibus, excepturi tempora
                                    repellendus eveniet sint sed maiores deleniti! Qui quis
                                    distinctio quo nam sunt commodi eveniet!
                                </p>
                            </div>
                        </div>
                        <!--div class="education-content">
                            <div class="content">
                                <div class="year">
                                    <img class="calendar-icon" src="src\assets\icons\calendar-icon.png" alt="Calendario">
                                     2017 - 2022
                                </div>
                                <h3>Master Degree - University</h3>
                                <p>
                                    Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                                    Dolore amet rem nulla voluptas temporibus, excepturi tempora
                                    repellendus eveniet sint sed maiores deleniti! Qui quis
                                    distinctio quo nam sunt commodi eveniet!
                                </p>
                            </div>
                        </div-->
                    </div>

                </div>

            </div>

        </section>
    </div>
</template>
<style scope>
.heading {
    font-size: 5rem;
    margin-bottom: 3rem;
    text-align: center;
}

.education {
    padding: 0 10%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: auto;
    padding-bottom: 5rem;
}

.education .education-row {
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;
}

.education-row .education-column {
    flex: 1 1 25rem;
}

.education-column .title {
    font-size: 2.5rem;
    margin: 0 0 1.5rem 2rem;
}

.education-column .education-box {
    border-left: .2rem solid #0080b3;
}

.education-box .education-content {
    position: relative;
    padding-left: 2rem;
}

.education-content .content {
    position: relative;
    padding: 1.5rem;
    border: .2rem solid #0080b3;
    border-radius: .6rem;
    margin-bottom: 2rem;
}

.education-content .content .year {
    font-size: 1.5 rem;
    color: #0080b3;
    padding-bottom: .5rem;
}/*
.education-content .content .year i {
padding-right: .5rem;
}*/

.education-content .content h3 {
    font-size: 2rem;
}
.education-content .content p {
    font-size: 1.6rem;
    padding-top: 0.5rem;
}
.calendar-icon {
    filter: saturate(100%) hue-rotate(180deg);
    width: 20px;
    height: auto;
}


/*
.education    
*/</style>