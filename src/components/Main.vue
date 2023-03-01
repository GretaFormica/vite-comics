<script>
    export default {
        data () {
            return {

            }
        },

        props: {
            comics: Array
        }
    }
</script>

<template>
  <main>

    <section class="black">

        <div class="container-m">
            <ul class="ul-thumb">
                <li
                v-for="comic in comics">

                <img :src= comic.thumb>
                {{ comic.series }}

                </li>
            </ul>
        </div>

    </section>

    <section class="blue">

        <div class="container-m">
            <ul class="ul-m">
                <li> <img src="../../vue-dc-comics-1/img/buy-comics-digital-comics.png"> <a href="#">DIGITAL COMICS</a></li>
                <li> <img src="../../vue-dc-comics-1/img/buy-comics-merchandise.png"> <a href="#">DC MERCHANDISE</a></li>
                <li> <img src="../../vue-dc-comics-1/img/buy-comics-subscriptions.png"> <a href="#">SUBSCRIPTION</a></li>
                <li> <img src="../../vue-dc-comics-1/img/buy-comics-shop-locator.png"> <a href="#">XOMIC SHOP LOCATOR</a></li>
                <li> <img src="../../vue-dc-comics-1/img/buy-dc-power-visa.svg"> <a href="#">DC POWER VISA</a></li>
            </ul>
        </div>

    </section>

    <section class="jumbo">

        <div class="container-m">

            <div class="half">
                <ul>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                    <li>comics</li>
                </ul>

            </div>

            <div class="half bg">

            </div>

        </div>

    </section>

  </main>

</template>

<style lang="scss">

.black{
    background-color: black;
    padding: 50px;
    color: white;
}

.blue{
    background-color: rgb(68, 86, 226);
    height: 100px;
}

.container-m{
  max-width: 1200px;
  margin: 0 auto;
  height: 100%;
  color: white;
  display: flex;
  align-items: center;
}

.ul-m{
    display: flex;
    justify-content: space-between;
    width: 100%;

    li{
        display: flex;
        align-items: center;
        gap: 10px;

        img{
            width: 30px;
        }
    }
}

.ul-thumb{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    li{
        width: calc(100% / 7);
        height: 200px;
        margin-top: 50px;
        margin-bottom: 50px;

        img{
            object-fit: cover;
            object-position: center;
            height: 100%;
        }
    }
}

.jumbo{
    height: 55vh;
    background-image: url('../../vue-dc-comics-1/img/footer-bg.jpg');
}

.half{
    width: 50%;
    height: 100%;

    ul{
        margin-top: 50px;

        li{
            margin-top: 10px;
        }
    }

}

.bg{
    background-image: url('../../vue-dc-comics-1/img/dc-logo-bg.png');
    background-size: cover;
    background-position: center;
}
</style>