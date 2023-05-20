<script>
    export default {
        name:"AppFooter"
    }
</script>

<template>
    <div class="footer text-white">
        <div class="container">
            <div class="row">
                <div class="col-6 d-flex py-5">
                    <div class="col-4">
                        <h4>DC COMICS</h4>
                        <p>CHARACTERS</p>
                        <p>COMICS</p>
                        <p>MOVIE</p>
                        <p>TV</p>
                        <p>GAMES</p>
                        <p>Videos</p>
                        <p>News</p>
                        
                        <h4 class="pt-3">SHOP</h4>
                        <p>SHOP DC</p>
                        <p>SHOP DC Collectionables</p>
                    </div>
                    <div class="col-4">
                        <h4>DC</h4>
                        <p>Terms Of Use</p>
                        <p>Privacy policy (New)</p>
                        <p>Ad choices</p>
                        <p>Advertising</p>
                        <p>Jobs</p>
                        <p>Subscriptions</p>
                        <p>Talent Workshop</p>
                        <p>CPSC Certificates</p>
                        <p>Ratings</p>
                        <p>Shop Help</p>
                        <p>Contact Us</p>
                    </div>
                    <div class="col-4">
                        <h4>SITES</h4>
                        <p>CD</p>
                        <p>MAD Magazine</p>
                        <p>DC Kids</p>
                        <p>DC Universe</p>
                        <p>DC Power Visa</p>
                    </div>
                </div>
                <!-- <div class="col-6">
                    <img src="../assets/dc-logo-bg.png" alt="">
                </div> -->
                <div class="col-6">
                    <img src="../assets/dc-logo-bg.png" class="z-0" alt="...">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

    img{
        width: 600px;
        height: 500px;
        object-fit: cover;
    }

    h4{
        font-size: 21px;
        font-weight: 700;
    }
    p{
        font-size: 14px;
        color: #b3b1b1;
        margin-bottom: 0px;
    }

    .footer{
        background-image: url(../assets/footer-bg.jpg);
        max-height: 500;
    }
</style>
