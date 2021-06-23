<template>
  <section class="jumbotron">
      <div class="container-60">
          <div class="content">
              <h2>New Challenges, New Skills</h2>
              <h1>BUILD YOUR OWN LIFE COACHING BUSINESS</h1>
              <h5>Whole-Life Business Coaching for committed entrepreneurs</h5>
              <button class="button-full">Get started today</button>
          </div>
          <div class="images">
              <img src="../assets/home-business-hero-global-image.png" alt="globe" id="jumbo-globe">
              <img src="../assets/home-business-hero-avatar.png" alt="avatar" id="jumbo-avatar">
          </div>
      </div>
      <div class="bookmark">
          <ul>
              <li><img src="../assets/square-ruler.png" alt="ruler"></li>
              <li><img src="../assets/life-saver.png" alt="lifesaver"></li>
              <li><img src="../assets/book.png" alt="book"></li>
              <li><img src="../assets/cart.png" alt="cart"></li>
          </ul>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Jumbotron'

}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

.jumbotron {
    background-color: $jumbotron;
    position: relative;

    .container-60 {
        @include flex;
        align-items: flex-start;

        .content {
            padding: 80px 0;
            width: 40%;

            & * {
                margin: 12px 0;
            }

            h1 {
            font-size: $h1;
            font-weight: 700;
            color: $mainText;
            }
            h2 {
                font-size: $h2;
                color: $mainGreen;

            }
            h5 {
                font-size: $h5;
                color: $mainGrey;
                line-height: 24px;
            }

        }

        .images {
            position: relative;
            width: 60%;
            display: flex;
            justify-content: center;
            padding-left: 50px;

            #jumbo-globe {
            position: absolute;
            top: -5px;
            left: 15%;
            width: 90%;
            transform: rotate(270deg);
            }

            #jumbo-avatar {
                padding-top: 40px;
                z-index: 2;
                width: 70%;
            }
        }


    }

    .bookmark {
        position: absolute;
        top: 100px;
        right: 0px;
        background-color: $white;
        padding: 10px;
        border-top-left-radius: 4px;
        border-bottom-left-radius: 4px;

        ul {
            @include ul-clean;
            list-style: none;

            li:not(:first-child) {
                margin-top: 10px;
            }

            li:hover {
                cursor: pointer;
            }

            & li img {
                width: 14px;
                
            }
        }
    }
}
</style>