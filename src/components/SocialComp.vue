<template>
  <div id="social">
      <div class="row">
        <div class="col-3">
            <img src="../assets/img/social-1.jpg" alt="Social">
        </div>

        <div class="col-6">  
            <div class="social-frame">
                <div class="upper-text">Made for sharing</div>
                <h2>Let's stay in touch</h2>
                <a class="btn btn-purple" href="#"><i class="fa-brands fa-instagram"></i>  Follow Us</a>
            </div>
        </div>

        <div class="col-3">
            <img src="../assets/img/social-2.jpg" alt="Social">
        </div>
      </div>

      <div class="row">
        <div class="col-3">
            <img src="../assets/img/social-3.jpg" alt="Social">
        </div>
        
        <div class="col-3">
            <img src="../assets/img/social-4.jpg" alt="Social">
        </div>
        
        <div class="col-3">
            <img src="../assets/img/social-5.jpg" alt="Social">
        </div>
        
        <div class="col-3">
            <img src="../assets/img/social-6.jpg" alt="Social">
        </div>
      </div>

  </div>
</template>

<script>
export default {
  name: 'SocialComp',
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

    #social {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        margin: 100px 0;
    }

    .social-frame {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100%;
        background-color: $pearl-bush;
    }

    .upper-text {
        display: block;
        font-size: 12px;
        font-weight: 500;
        text-transform: uppercase;
        color: $mamba;
    }

    h2 {
        font-family: 'Libre Bodoni', serif;
        font-size: 26px;
        font-weight: bold;
        color: $daisy-bush;
        margin: 20px 0;
    }
</style>