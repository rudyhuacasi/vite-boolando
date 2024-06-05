<script>
export default {
    name: app,
    data() {
        return {
            title: "La mia prima app con Vite!"
        };
    }
}
</script>
<template>
    <footer>
        <div class="container">
            <div class="flex">
                <div class="medium">
                    <strong>Booleando s.r.l.</strong><br>
                    <p class="top">Informazioni legali Inormativa sulla privacy Diritto di recesso</p>
                    
                </div>
                <div class=" right-1 medium">
                    <p>Trovaci anche su</p>
                        <i class="fa-brands fa-square-twitter"></i>
                        <i class="fa-brands fa-square-facebook"></i>
                        <i class="fa-brands fa-square-instagram"></i>
                        <i class="fa-brands fa-square-pinterest"></i>
                        <i class="fa-brands fa-square-youtube"></i>
                    
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss">
%flex{
    display: flex;
    align-items: center;
}
footer{
    @extend %flex;
    background-color: black;
    height: 75px;
    .flex{
        @extend %flex;
    }
    .medium{
        color: white;
        width: 50%;
    }
    .right-1{
        text-align: right;
    }
    p{
        margin-bottom: 5px;
    }
    .top{
        margin-top: 5px;
    }
}
</style>