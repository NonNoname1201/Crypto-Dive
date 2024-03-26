<script setup>
import IconLogo from "@/components/icons/page_first/IconLogo.vue";
</script>

<template>
    <section class="footer">
        <section class="footer-container">
            <IconLogo/>
            <div class="line"/>
            <div class="info">
                <h3>Informacja</h3>
                <p>cryptodive.pl@gmail.com</p>
                <p>+48 123 456 789</p>
                <p>Poland, Warszawa Mazowieckie</p>
            </div>
        </section>
        <p class="copyright">2024 Wszelkie prawa zastrzeżone &copy</p>
    </section>
</template>

<style scoped>
.footer {
    padding: 30px;
    background-color: #000000;
    border-top-left-radius: 100px;
    border-top-right-radius: 100px;
    width: 100%;
    min-height: 200px;
    .footer-container {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        height: 150px;
        .line {
            width: 10px;
            height: 100%;
            background: linear-gradient(to bottom, rgb(51, 255, 0), rgb(0, 117, 255), rgb(112, 0, 255));
            border-radius: 5px;
        }
        h3 {
            color: #FFFFFF;
            font-size: 20px;
            font-weight: 700;
            margin-bottom: 5px;
        }
        p {
            margin-bottom: 3px;
        }
    }
    .copyright {
        margin-top: 20px;
        color: #FFFFFF80;
        font-size: 15px;
        font-weight: 700;
        text-align: center;
    }
}

</style>