<template>
  <section class="reviews">
      <div class="container-85">
          <h2 class="text-center">People are praising Maxcoach</h2>
          <h1 class="text-center">What make they love us?</h1>
          <div class="review-list">
              <div class="review">
                 <h2 class="purple">Lorem ipsum dolor sit amet.</h2>
                 <h2 class="smaller">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius impedit ad dolorum voluptatum debitis non laborum distinctio dolore veniam fugiat, nulla, nobis necessitatibus! Corporis iste possimus provident? Enim, eius eveniet.</h2>
                 <div class="user">
                 </div>
              </div>
              <div class="review">
                 <h2 class="purple">Lorem ipsum dolor sit amet.</h2>
                 <h2 class="smaller">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius impedit ad dolorum voluptatum debitis non laborum distinctio dolore veniam fugiat, nulla, nobis necessitatibus! Corporis iste possimus provident? Enim, eius eveniet.</h2>
                 <div class="user">
                 </div>
              </div>
              <div class="review">
                 <h2 class="purple">Lorem ipsum dolor sit amet.</h2>
                 <h2 class="smaller">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius impedit ad dolorum voluptatum debitis non laborum distinctio dolore veniam fugiat, nulla, nobis necessitatibus! Corporis iste possimus provident? Enim, eius eveniet.</h2>
                 <div class="user">
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

h2 {
    font-size: $h2;
    color: $mainGreen;
}
h1 {
    font-size: $h1;
    color: $mainText;
    font-weight: 600;
}
h3 {
    font-size: $h3;
    color: $mainText;
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

        .smaller {
                color: $mainGreen;
                font-weight: normal;
                margin: 0;
            }

        .info {

            h3 {
                margin-top: 8px;
            }
            span {
                font-size: $smallText;
                color: $mainGrey;
                & p {
                    margin-left: 6px;
                    display: inline;
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