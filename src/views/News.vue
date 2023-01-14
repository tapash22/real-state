<template>
<div class="news-letter">
    <v-container>
        <h2>NewsLetters login</h2>
        <div class="box">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis maxime reprehenderit a, repudiandae architecto repellat doloremque obcaecati aliquam eaque! Natus?</p>
        </div>
        <div class="form">
            <div class="box2">
                <v-text-field v-model="text" outlined dense hide-details />
                <v-btn large color="primary">send</v-btn>
            </div>
        </div>

    </v-container>
</div>
</template>

<style scoped>
h2 {
    display: flex;
    justify-content: center;
    font-size: 2rem;
    font-weight: 700;
    padding: 20px;
}

.box {
    padding: 5px;
    margin: 0;
    display: flex;
    justify-content: center;
}

.box p {
    width: 60%;
    font-size: 1rem;
    font-weight: 400;
    text-align: center;
    padding: 0;
    margin: 0;
}
.form{
    display: flex;
    justify-content: center;
}

.form .box2 {
    display: flex;
    justify-content: stretch;
    width: 50%;
    margin-top: 5px;
}
</style>
