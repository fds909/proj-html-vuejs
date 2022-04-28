<template>
    <div class="numbers">
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
      padding: 50px 0;
    }

    .number-1 {
      background-image: url('../assets/img/bakery-process-1.jpg');
      background-size: cover;
      background-repeat: no-repeat;
      height: 80vh;
    }

    .number-1-content {
      display: flex;
      justify-content: space-between;
      height: 100%;
      background-color: rgba($color: $cod-gray, $alpha: 0.5);
      color: white;
      position: relative;
      padding: 50px;
    }

    .number-1-content h2 {
      font-family: 'Libre Bodoni', serif;
      font-size: 40px;
      width: 50%;
      font-weight: bold;
    }

    .number {
      font-size: 60px;
    }

    .description {
      width: 40%;
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

</style>