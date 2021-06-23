<template>
  <section class="subscribe">
      <div class="circle"></div>
      <img src="../assets/maxcoach-shape-09.png" alt="" class="decoration dec-1">
      <img src="../assets/maxcoach-shape-02.png" alt="" class="decoration dec-2">
      <div class="container-80 text-center">
          <div class="subscribe-action">
            <h1>Subscribe <span class="green">Newsletters</span></h1>
            <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
            <form>
              <div class="input-group mb-3">
                <input type="text" class="form-control" placeholder="Enter your email">
                <span class="input-group-text">Subscribe</span>
                </div>
            </form>
            </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Subscribe'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

    .subscribe {
        padding: 80px 0;
        position: relative;

        .circle {
            position: absolute;
            border: 6px solid $mainGreen;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            left: 100px;
            top: 120px;
        }

        .decoration {
            position: absolute;
            right: 200px;
        }

        .dec-1 {
            width: 160px;
            top: 40px;
        }

        .dec-2 {
            width: 100px;
            top: 110px;
        }

    }

    .subscribe-action {
        width: 40%;
        margin: auto;

        h1 {
            font-size: $h1;
            color: $mainText;
            font-weight: 600;

            .green {
                color: $mainGreen;
                font-weight: 400;
                }
        }

        p {
        font-size: $h5;
        color: $mainGrey;
        font-weight: 500;
        }   


    }

    .form-control {
        background-color: $exploreGrey;
        border: none;
        font-size: $h5;
    }

    .input-group-text {
        border: none;
        background-color: $mainGreen;
        color: $white;
        font-size: $h5;
        font-weight: 600;
        padding: 10px 30px;
    }
    
    

</style>