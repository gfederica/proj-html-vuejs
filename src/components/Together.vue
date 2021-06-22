<template>
  <section class="together">
      <div class="container-60">
          <h2 class="text-center">Let's Dream Big Together</h2>
          <p class="big-paragraph text-center">We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization.</p>
          <div class="features">
              <div class="card">
                <img src="../assets/brotherhood.png" alt="one-to-one">
                    <div class="card-body">
                        <h2 class="card-title">One to One</h2>
                        <p class="card-text">Getting the necessary clarity about the current state to help you improve your game.</p>
                    </div>  
              </div>
              <div class="card">
                <img src="../assets/pin.png" alt="anywhere">
                    <div class="card-body">
                        <h2 class="card-title">Anywhere</h2>
                        <p class="card-text">Access to valuable and portable program which allow you to setup and live anywhere you want.</p>
                    </div>  
              </div>
              <div class="card">
                <img src="../assets/chronometer.png" alt="chronometer">
                    <div class="card-body">
                        <h2 class="card-title">On Time</h2>
                        <p class="card-text">Punctuality is our top priority because it's an essential criteria to assess a program quality.</p>
                    </div>  
              </div>
              <div class="card">
                <img src="../assets/laptop.png" alt="online-course">
                    <div class="card-body">
                        <h2 class="card-title">Online Courses</h2>
                        <p class="card-text">Online business coaching now offers you a very powerful way to empower your business into success.</p>
                    </div>  
              </div>
              <div class="card">
                <img src="../assets/consulting.png" alt="consulting">
                    <div class="card-body">
                        <h2 class="card-title">Consulting</h2>
                        <p class="card-text">You will get a clear sense of direction for your business, thorough assessment and faster results.</p>
                    </div>  
              </div>
              <div class="card">
                <img src="../assets/gears.png" alt="gears">
                    <div class="card-body">
                        <h2 class="card-title">Self Development</h2>
                        <p class="card-text">Business coaching often keep your focus and develop you both in a professional and personal way.</p>
                    </div>  
              </div>
          </div>
          <div class="actions text-center">
              <button class="button-empty">Learn more</button>
              <button class="button-full">Get started today</button>
          </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Together'
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

.together {
    padding: 80px 0;

        h2 {
            font-size: $h2;
            color: $mainGreen;
        }

        .big-paragraph {
            font-size: 24px;
            font-weight: 600;
            padding: 20px 50px;
            color: $mainText;
        }
}

.features {
    display: flex;
    flex-wrap: wrap;

        .card {
        width: 33%;
        @include flex;
        flex-direction: row;
        align-items: flex-start;
        border: none;
        padding: 10px;
        
        & img {
            width: 10%;
            padding-top: 20px;
            }
        }

        p {
            font-size: $h5;
            color: $mainGrey;
        }

        h2 {
            color: $mainText;
            font-weight: 500;
        }
}

.actions {
    margin-top: 30px;
    
    button {
    margin: 0 20px;
    }
}

</style>
