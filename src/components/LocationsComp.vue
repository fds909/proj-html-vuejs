<template>
    <div id="locations">
      <div class="upper-text">Locations</div>
      <h2>Visit our Bakeries</h2>

      <div class="locations">
        <!-- New York -->
        <div class="location" id="newyork">
            <img src="../assets/img/new-york-bk.jpg" alt="New York">
            <div class="location-text">
                <h2>New York</h2>
                <div class="info">
                    <div class="info-col">
                        <div class="upper-text">Call us</div>
                        <p>1.800.458.566</p>
                    </div>
                    <div class="info-col">
                        <div class="upper-text">Open all week</div>
                        <p>9:00 AM - 6:00 PM</p>
                    </div>
                    <div class="info-col">
                        <a class="btn btn-white" href="#">View Map</a>
                    </div>
                </div>
            </div>
        </div>

        <!-- London -->
        <div class="location" id="london">
            <img src="../assets/img/london-bk.jpg" alt="London">
            <div class="location-text">
                <h2>London</h2>
                <div class="info">
                    <div class="info-col">
                        <div class="upper-text">Call us</div>
                        <p>1.800.458.566</p>
                    </div>
                    <div class="info-col">
                        <div class="upper-text">Open all week</div>
                        <p>9:00 AM - 6:00 PM</p>
                    </div>
                    <div class="info-col">
                        <a class="btn btn-white" href="#">View Map</a>
                    </div>
                </div>
            </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'LocationsComp',
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

    #locations {
        margin: 100px 0;
    }

    .upper-text {
      display: block;
      font-size: 12px;
      font-weight: 500;
      text-transform: uppercase;
      color: $mamba;
      text-align: center;
    }

    h2 {
        font-family: 'Libre Bodoni', serif;
        font-size: 28px;
        color: $daisy-bush;
        text-align: center;
        margin: 30px 0;
    }

    img {
        max-width: 100%;
    }

    .locations {
        display: flex;
    }

    .location {
        width: 50%;
    }

    #newyork {
        background-color: #f1f9fb;
    }

    #london {
        background-color: #faf3e3;
    }

    .location-text {
        margin: 40px 0;
    }

    .info {
        display: flex;
        flex-direction: row;
    }

    .info-col {
        width: calc(100% / 3);
        text-align: center;
    }

    .info p {
        font-size: 14px;
        color: $mamba;
        margin-top: 5px;
    }
</style>