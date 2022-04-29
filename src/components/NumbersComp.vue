<template>
    <div class="numbers">
      <!-- Number 1 -->
      <div class="number-1">
        <div class="number-1-content">
          <h2>Tell us what you have in mind</h2>
          <div class="number">01</div>
          <div class="description">
            <div class="upper-text">
              Manual ingredients selection
            </div>
            <p>
              Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius Ut eu laoreet ex.
              Aliquam erat volutpat. Nullam quit saggitis nibh. Morbi consectetur ultricies ante ac congue.
              Donec lorem erat, finibus in velit placerat, rutrum augue.
            </p>
          </div>
        </div>
      </div>

      <!-- Number 2 -->
      <div class="number-2">
        <div class="number-2-content">
          <div class="number-2-content-shadow">
            <h2>We start baking</h2>
            <div class="number">02</div>
            <div class="description">
              <div class="upper-text">
                Sweet & delicious
              </div>
              <p>
                Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius Ut eu laoreet ex.
                Aliquam erat volutpat. Nullam quit saggitis nibh. Morbi consectetur ultricies ante ac congue.
                Donec lorem erat, finibus in velit placerat.
              </p>
            </div>
          </div>
        </div>

        <div class="number-2-text">
          <div class="upper-text">Dont just take our word for it</div>
          <h2>"Finally found an alternative to the mass produced products.
              Something that incorporates real organic ingredients, nutrient dense wellness while
              promoting sustainability and activity."
          </h2>
          <p class="author">Rachel Cooper, Founder</p>
        </div>
      </div>

      <!-- Number 3 -->
      <div class="number-3">
        <div class="number-3-content">
          <h2>Delivered to your home</h2>
          <div class="number">03</div>
          <div class="description">
            <div class="upper-text">
              Manual ingredients selection
            </div>
            <p>
              Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius Ut eu laoreet ex.
              Aliquam erat volutpat. Nullam quit saggitis nibh. Morbi consectetur ultricies ante ac congue.
              Donec lorem erat, finibus in velit placerat, rutrum augue.
            </p>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'NumbersComp',
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

    .numbers {
      margin: 100px 0;
    }

    // Number 1
    .number-1 {
      background-image: url('../assets/img/bakery-process-1.jpg');
      background-size: cover;
      background-repeat: no-repeat;
      height: 80vh;
      margin-bottom: 25px;
    }

    .number-1-content {
      display: flex;
      justify-content: space-between;
      height: 100%;
      background-color: rgba($color: $cod-gray, $alpha: 0.5);
      color: $white;
      position: relative;
      padding: 50px;
    }

    h2 {
      font-family: 'Libre Bodoni', serif;
      font-size: 40px;
      font-weight: bold;
    }

    .number-1-content h2 {
      width: 50%;
    }

    .number {
      font-size: 60px;
    }

    .description {
      width: 50%;
      position: absolute;
      bottom: 50px;
      right: 50px;
    }

    .upper-text {
      display: block;
      font-size: 12px;
      font-weight: 500;
      text-transform: uppercase;
      color: $mamba;
    }

    .description p {
      font-size: 14px;
      line-height: 25px;
      margin-top: 15px;
    }

    // Number 2
    .number-2 {
      display: flex;
      gap: 0 20px;
      margin-bottom: 25px;
    }

    .number-2-content {
      width: 50%;
      height: 500px;
      color: $white;
      background-image: url("../assets/img/bakery-process-2.jpg");
      background-size: cover;
      background-position: -60px;
      background-repeat: no-repeat;
    }

    .number-2-content-shadow {
      display: flex;
      justify-content: space-between;
      background-color: rgba($color: $cod-gray, $alpha: 0.5);
      width: 100%;
      height: 100%;
      padding: 50px;
      position: relative;
    }

    .number-2-content h2 {
      font-size: 35px;
    }

    .number-2-content .description {
      position: absolute;
      left: 50px;
      bottom: 50px;
    }

    .number-2-content .upper-text {
      color: $white;
    }

    .number-2-text {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      width: 50%;
      height: 500px;
      background-color: $pearl-bush;
      padding: 0 50px;
    }

    .number-2-text h2 {
      font-size: 32px;
      color: $daisy-bush;
      margin: 30px 0;
    }

    .number-2-text .author {
      font-size: 14px;
      color: $mamba;
    }

    // Number 3
    .number-3 {
      display: flex;
      width: 100%;
      height: 500px;
      background-image: url('../assets/img/bakery-process-3.jpg');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      color: white;
    }

    .number-3-content {
      display: flex;
      justify-content: space-between;
      background-color: rgba($color: $cod-gray, $alpha: 0.5);
      width: 100%;
      height: 100%;
      padding: 50px;
      position: relative;
    }

    .number-3 .description {
      position: absolute;
      left: 50px;
      bottom: 50px;
    }

</style>