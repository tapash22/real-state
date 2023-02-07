<template>
<div class="news-letter">
    <v-container class="my-3">
        <h2 class="text-h6 font-weight-bold">NewsLetters</h2>

        <p class="text-body-2 d-flex justify-center mt-n2">Enter your email for connectin with us</p>

        <div class="form">
            <div class="box2">
                <v-text-field v-model="text" outlined dense hide-details />
                <v-btn class="btn" large color="primary">send</v-btn>
            </div>
        </div>

    </v-container>
</div>
</template>

<script>
export default {
    data() {
        return {
            text: ''
        }
    }
}
</script>

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

.form {
    display: flex;
    justify-content: center;
}

.form .box2 {
    display: flex;
    justify-content: stretch;
    width: 50%;
    margin-top: 5px;
}

@media only screen and (max-width: 600px) {
    .form {
        display: flex;
        justify-content: center;
    }

    .form .box2 {
        display: block;
        justify-content: stretch;
        width: 70%;
        margin-top: 5px;
    }

    .form .box2 .btn {
        margin-left: 30%;
        padding: 5px;
    }
}
</style>
