<template>
    <div class="comment">
        <div class="banner-bg" id="top">
            <div class="banner-overlay"></div>
            <div class="welcome-text">
                <h2>Bank | "Tree PreOrders"</h2>
                <h5>you can’t buy happiness but you can buy plants and that’s the same thing
                    <hr>
                    <br>
                    - ซื้อความสุขไม่ได้
                    <br>
                    - แต่ซื้อต้นไม้ได้นะ 😉
                    <br>
                    - ส่งจันทร์/พุธ
                    <br>
                    - ตอบข้อความ 24 ชั่วโมง </h5>
            </div>
        </div>
    </div>
</template>
<script>
export default {
}
</script>
<style scoped>
    .comment {
        margin-left: 10px;
        margin-top: 10px;
        margin-right: 10px;
    }
    .banner-bg {
	    padding: 190px 80px;
	    position: relative;
	    background-position: center;
	    background-size: cover;
	    z-index: 2;
    }
    .banner-overlay {
        position: absolute;
        width: 100%;
        height: 125vh;
        background: rgba(231, 231, 231, 0.192);
        top: 0;
        right: 0;
        z-index: 3;
    }
    
    img {
        width: 100%;
        height: 100%;
    }
</style>