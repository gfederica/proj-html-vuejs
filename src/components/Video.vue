<template>
  <section class="video">
      <img src="../assets/background-map-dots-top-right-transparent.png" alt="map" id="background">
      <img src="../assets/maxcoach-shape-07.png" alt="square" id="square">
      <div class="container-80">
          <div class="youtube">
              <img src="../assets/home-business-video-poster-670x450.jpg" alt="video" class="yt">
              <img src="../assets/icon-youtube-play.png" alt="play" id="yt-button">
          </div>
          <div class="plan">
              <h1>To Thrive in Business Today, You'll Need a Good Plan</h1>
              <ul class="fa-ul">
                  <li><span class="fa-li"><i class="fas fa-angle-up active"></i></span>                      
                      <div class="content">
                          <h3 class="active">How can we help?</h3>
                          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eligendi officia sed obcaecati quo laudantium. Fugiat et aperiam unde a esse ipsa sequi molestiae sint labore libero molestias laboriosam blanditiis voluptates temporibus <br><br> quia maiores obcaecati quisquam laudantium nesciunt, adipisci similique vel numquam animi quos? Dicta delectus tenetur nihil quisquam repellendus cum.</p>
                      </div>
                  </li>
                  <li><span class="fa-li"><i class="fas fa-angle-down"></i></span>                      
                      <div class="content">
                          <h2>Why would I need a business COACH?</h2>
                      </div>
                  </li>
                  <li><span class="fa-li"><i class="fas fa-angle-down"></i></span>                      
                      <div class="content">
                          <h2>What is one-on-one coaching?</h2>
                      </div>
                  </li>
              </ul>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Video'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

.video  {
    background-color: $darkPurple;
    padding: 80px 0;
    position: relative;

        #background {
            position: absolute;
            top: 0;
            right: 0;
            width: 55%;
        }
        #square {
            position: absolute;
            bottom: 18px;
            left: 160px;
            width: 150px;
        }

    .container-80 {
        @include flex-space-evenly;
        
        .youtube {
            width: 40%;
            position: relative;

            .yt {
                width: 100%;
                border-radius: 4px;

            }

            #yt-button {
                width: 80px;
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
            }

        }

        .plan {
            width: 30%;

            h1 {
                font-size: $h1;
                color: $white;
            }

            h2 {
                font-size: $h2;
            }
            h3{
                font-size: $h3;
            }
            .active {
                color: $mainGreen;
            }

            p {
                font-size: $smallText;
                padding: 10px;
            }

            ul {
                margin-top: 20px;
                margin-left: 20px;

                .fa-li i{
                    border: 2px solid;
                    border-radius: 50%;
                    width: 64%;

                    .fa-li i .active {
                        border: $mainGreen;
                    }
                }

                li {
                    padding: 16px 0;
                    color: $white;
                    border-bottom: 1px solid $mainGrey;
                   
                }
            }
        }
    }
}
</style>