<template>
  <section class="explore">
      <div class="container-60">
          <h2 class="text-center">Let's Dream Big Together</h2>
          <h1 class="text-center">Explore How can I help you</h1>
          <div class="features text-center">
              <div class="card shadow p-0 rounded">
                <img src="../assets/home-business-service-slide-01-480x298.jpg" alt="training">
                    <div class="card-body">
                        <h2 class="card-title">Consultative Training</h2>
                        <p class="card-text">With a coach addressing multiple issues that are off balance, affecting your business in various unconsidered ways.</p>
                    </div>  
                    <ul class="list-group list-group-flush">
                        <li class="list-group-item"><a href="">Discover now <i class="fas fa-arrow-right"></i></a></li>
                    </ul>
              </div>
              <div class="card shadow p-0 rounded">
                <img src="../assets/home-business-service-slide-02-480x298.jpg" alt="anywhere">
                    <div class="card-body">
                        <h2 class="card-title">Real Deal Coaching</h2>
                        <p class="card-text">Brings an exceptionally powerful opportunity. Being able to accept, to work with that opportunity.</p>
                    </div> 
                    <ul class="list-group list-group-flush">
                        <li class="list-group-item"><a href="">Discover now <i class="fas fa-arrow-right"></i></a></li>
                    </ul> 
              </div>
              <div class="card shadow p-0 rounded">
                <img src="../assets/home-business-service-slide-03-480x298.jpg" alt="chronometer">
                    <div class="card-body">
                        <h2 class="card-title">Advisor Training Program</h2>
                        <p class="card-text">Getting high quality, entrepreneur mindset driven online business coaching, is what is needed.</p>
                    </div>  
                    <ul class="list-group list-group-flush">
                        <li class="list-group-item"><a href="">Discover now <i class="fas fa-arrow-right"></i></a></li>
                    </ul>
              </div>
          </div>
          <div class="slider text-center">
              <i class="fas fa-circle"></i>
              <i class="fas fa-circle"></i>
              <i class="fas fa-circle"></i>
          </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Explore'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

.explore {
    padding: 100px 0;
    background-color: $exploreGrey;

        h2 {
            font-size: $h2;
            color: $mainGreen;
        }

        h1 {
            font-size: $h1;
            color: $mainText;
            font-weight: 600;
        }
}

.features {
    display: flex;
    flex-wrap: wrap;
    margin-top: 50px;

    a {
        @include link-clean;
        font-size: $mediumSmallText;
        color: $mainGreen;
        font-weight: 600;

        i {
            margin-left: 10px;
            font-size: $smallText;
        }
    }

        .card {
        width: calc(33% - 18px);
        margin: 10px;
        @include flex;
        align-items: flex-start;
        
        & img {
            width: 100%;
            }
        }

        p {
            font-size: $mediumSmallText;
            color: $mainGrey;
            height: 100%;
        }

        h2 {
            color: $mainText;
            font-weight: 500;
        }

        .card-body {
            padding: 18px;
        }

        .list-group {
            text-align: center;
            width: 100%;
            border-top: 1px solid $jumbotron;
        }
}

.slider {
    margin-top: 20px;
    
    i {
        font-size: 6px;
        padding: 0 8px;
        color: $silver;

       &:nth-child(1) {
            color: $mainText;
            font-size: $smallText;
        }
    }
}

</style>
