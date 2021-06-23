<template>
  <section class="reviews">
      <div class="container-85">
          <h2 class="text-center">People are praising Maxcoach</h2>
          <h1 class="text-center">What make they love us?</h1>
          <div class="review-list">
              <div class="review">
                <div class="transparent"></div>
                 <p class="purple">Lorem ipsum dolor sit amet.</p>
                 <p class="grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, in?</p>
                 <div class="user">
                     <img src="../assets/testimonial-avata-01.jpg" alt="">
                     <div class="name">
                        <p class="purple text-uppercase">Florence Themes</p>
                        <p class="grey smaller">/ Multimedia admin</p>
                     </div>
                 </div>
              </div>
              <div class="review">
                 <p class="purple">Lorem ipsum dolor sit amet.</p>
                 <p class="grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, in?</p>
                 <div class="user">
                     <img src="../assets/testimonial-avata-02.jpg" alt="">
                     <div class="name">
                        <p class="purple text-uppercase">Mina Hollace</p>
                        <p class="grey smaller">/ Freelancer</p>
                     </div>
                 </div>
              </div>
              <div class="review">
                <div class="transparent"></div>
                 <p class="purple">Lorem ipsum dolor sit amet.</p>
                 <p class="grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, in?</p>
                 <div class="user">
                     <img src="../assets/testimonial-avata-03.jpg" alt="">
                     <div class="name">
                        <p class="purple text-uppercase">Madley Pondor</p>
                        <p class="grey smaller">/ IT Specialist</p>
                     </div>
                 </div>
              </div>
          </div>
           <div class="slider text-center">
              <i class="fas fa-circle"></i>
              <i class="fas fa-circle"></i>
              <i class="fas fa-circle"></i>
              <i class="fas fa-circle"></i>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Reviews'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

p {
    font-size: $h5;
    color: $darkPurple;
    font-weight: 600;
}
h2 {
    font-size: $h2;
    color: $mainGreen;
}
h1 {
    font-size: $h1;
    color: $mainText;
    font-weight: 600;
}

.reviews {
    background-color: $exploreGrey;
    padding: 80px 0;
}

.review-list {
    @include flex;
    flex-wrap: wrap;

    .review {
        width: calc(33% - 10px);
        margin: 5px;
        background-color: $white;
        padding: 30px;
        border-radius: 6px;
        position: relative;

        .transparent {
            position: absolute;
            background-color: rgba($color: $white, $alpha: 0.6);
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .grey {
                color: $mainGrey;
                font-weight: normal;
                margin: 0;
            }

        .user {
            @include flex-space-between;
            padding-top: 30px;

            img {
                width: 60px;
                border-radius: 50%;
            }

            .name {
                margin-left: 20px;

                & p {
                    margin: 0;
                }

                .smaller {
                    font-size: $smallText;
                }
            }
        }
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