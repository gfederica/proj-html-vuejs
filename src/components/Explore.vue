<template>

<div class="explore-all">
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
    <section class="explore-white-bg">
        <div class="container-85">
            <h2 class="text-center">Let's Dream Big Together</h2>
            <h1 class="text-center">Explore How can I help you</h1>
            <div class="features nowrap">
                <div class="card hero text-white rounded">
                    <img src="../assets/course-02-443x600.jpg" class="card-img" alt="background">
                    <div class="hero-card"></div>
                    <div class="card-img-overlay">
                        <h2 class="card-title">$40.<span class="smaller">00</span></h2>
                        <h2 class="card-text">Learning to Write as a Professional Author</h2>
                    </div>
                </div>
                <div class="card hero text-white rounded">
                    <img src="../assets/stock-full-hd-03-443x600.jpg" class="card-img" alt="background">
                    <div class="hero-card"></div>
                    <div class="card-img-overlay">
                        <h2 class="card-title">Free</h2>
                        <h2 class="card-text">Customer-centric Info-Tech Strategies</h2>
                    </div>
                </div>
                <div class="card hero text-white rounded">
                    <img src="../assets/stock-full-hd-04-443x600.jpg" class="card-img" alt="background">
                    <div class="hero-card"></div>
                    <div class="card-img-overlay">
                        <h2 class="card-title">$19.<span class="smaller">00</span></h2>
                        <h2 class="card-text">Open Programming Courses for Everyone: Python</h2>
                    </div>
                </div>
                <div class="card hero text-white rounded">
                    <img src="../assets/stock-full-hd-06-443x600.jpg" class="card-img" alt="background">
                    <div class="hero-card"></div>
                    <div class="card-img-overlay">
                        <h2 class="card-title">$26.<span class="smaller">00</span></h2>
                        <h2 class="card-text">Academic Listening and Note-taking</h2>
                    </div>
                </div>
            </div>
            <div class="view-all-courses">
                <p class="text-center">Take the control of their life back and start doing things to make their dream come true. <span><a href="">View all courses <i class="fas fa-arrow-right"></i></a></span></p>
            </div>
        </div>
    </section>
</div>
</template>

<script>
export default {
    name: 'Explore'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

h2 {
    font-size: $h2;
    color: $mainGreen;
}
h1 {
    font-size: $h1;
    color: $mainText;
    font-weight: 600;
}


.explore,
.explore-white-bg {
    padding: 100px 0;
}

.explore {
    background-color: $exploreGrey;
}
.explore-white-bg {
    background-color: $white;
}

// prima sezione
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

        .hero {
            width: 25%;
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


// seconda sezione
// overlay
.hero-card::after {
    content: "";
    position: absolute;
    top:0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(to bottom, transparent 60%, black 100%);
    background-blend-mode: overlay;
}

.nowrap {
    flex-wrap: nowrap;
}

.card-img-overlay {
    top: 68%;

    h2:not(.card-text) {
        font-size: $h2;
        color: $mainGreen;
        font-weight: 700;
    }

    h2 {
        color: $white;
    }

    .smaller {
        font-size: $h5;
    }
}

.view-all-courses {
    width: 35%;
    margin: auto;
    padding-top: 30px;

    p {
        font-size: $mediumSmallText;
        font-weight: 600;
        color: $mainGrey;
        line-height: 24px;

        a {
           color: $mainText;
           font-weight: 700;
           text-underline-offset: 4px;
           text-decoration-color: $silver;
        }
    }
}

</style>
