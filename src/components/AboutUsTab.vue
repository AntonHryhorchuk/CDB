<template>
  <section class="about-us">
    <div class="tabs">
      <a-tabs default-active-key="1" >
        <a-tab-pane class="tabs__title" key="1" tab="WHAT IS CBD?">
          <div class="about-us__wrapper">
            <div class="about-us__wrapper-description">
              <h4 class="about-us__wrapper-description-title">
                WHAT IT IS AND HOW IT WORKS
              </h4>
              <p class="about-us__wrapper-description-text">
                CBD is short for cannabidiol. It is a phytocannabinoid found in
                hemp and known for supporting the body and mind in many ways.*
                Charlotte’s Web products have cannabinoids with CBD extract.
              </p>
              <p class="about-us__wrapper-description-text">
                Not to be confused with oil from hemp seeds (which doesn’t
                contain cannabinoids), CBD comes from the flowers and leaves of
                the hemp plant.
              </p>
              <p class="about-us__wrapper-description-text">
                Why does CBD work? The human body has a vast network of
                receptors, the endocannabinoid system.
              </p>
            </div>
            <div class="about-us__wrapper-images">
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg.png"
                />
              </div>
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg2.png"
                />
              </div>
            </div>
          </div>
        </a-tab-pane>
        <a-tab-pane class="tabs__title" key="2" tab="BENEFITS" force-render>
          <div class="about-us__wrapper">
            <div class="about-us__wrapper-description">
              <h4 class="about-us__wrapper-description-title">
                WHAT IT IS AND HOW IT WORKS
              </h4>
              <p class="about-us__wrapper-description-text">
                CBD is short for cannabidiol. It is a phytocannabinoid found in
                hemp and known for supporting the body and mind in many ways.*
                Charlotte’s Web products have cannabinoids with CBD extract.
              </p>
              <p class="about-us__wrapper-description-text">
                Not to be confused with oil from hemp seeds (which doesn’t
                contain cannabinoids), CBD comes from the flowers and leaves of
                the hemp plant.
              </p>
              <p class="about-us__wrapper-description-text">
                Why does CBD work? The human body has a vast network of
                receptors, the endocannabinoid system.
              </p>
            </div>
            <div class="about-us__wrapper-images">
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg.png"
                />
              </div>
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg2.png"
                />
              </div>
            </div>
          </div>
        </a-tab-pane>
        <a-tab-pane class="tabs__title" key="3" tab="OUR DIFFERENCE">
          <div class="about-us__wrapper">
            <div class="about-us__wrapper-description">
              <h4 class="about-us__wrapper-description-title">
                WHAT IT IS AND HOW IT WORKS
              </h4>
              <p class="about-us__wrapper-description-text">
                CBD is short for cannabidiol. It is a phytocannabinoid found in
                hemp and known for supporting the body and mind in many ways.*
                Charlotte’s Web products have cannabinoids with CBD extract.
              </p>
              <p class="about-us__wrapper-description-text">
                Not to be confused with oil from hemp seeds (which doesn’t
                contain cannabinoids), CBD comes from the flowers and leaves of
                the hemp plant.
              </p>
              <p class="about-us__wrapper-description-text">
                Why does CBD work? The human body has a vast network of
                receptors, the endocannabinoid system.
              </p>
            </div>
            <div class="about-us__wrapper-images">
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg.png"
                />
              </div>
              <div class="about-us__wrapper-images-img">
                <img
                  class="about-us__wrapper-images-img-img"
                  src="../assets/aboutImg2.png"
                />
              </div>
            </div>
          </div>
        </a-tab-pane>
      </a-tabs>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.tabs {
  width: 70%;
}
.about-us {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #F7F8F3;
}
.about-us__wrapper {
  width: 100%;
  max-width: 900px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
  padding-top: 30px;
}
.about-us__wrapper-description-title {
  color: #000000;
  font-family: "Oswald", sans-serif;
  font-weight: 400;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 3px;
  max-width: 220px;
  margin-bottom: 40px;
}
.about-us__wrapper-description-text {
  padding: 10px 140px 10px 0px;
  color: #000000;
  font-family: "Oswald", sans-serif;
  font-weight: 300;
  font-size: 16px;
  margin-bottom: 10px;
}
.about-us__wrapper-images {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.about-us__wrapper-images-img {
  width: 300px;
  height: 0;
  padding-bottom: 66.67%;
  border: 2px solid white;
  position: relative;
}
.about-us__wrapper-images-img-img {
  width: 100%;
  position: absolute;
  object-fit: cover;
}
</style>
