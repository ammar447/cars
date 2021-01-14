<template>
  <div>
    <!-- Cars -->
    <h1>cars for Sale</h1>
    <section class="tiles">
      <article class="style1">
        <span class="image">
          <img src="../../assets/selse/1.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>
      <article class="style2">
        <span class="image">
          <img src="../../assets/selse/2.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>
      <article class="style3">
        <span class="image">
          <img src="../../assets/selse/3.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>

      <article class="style4">
        <span class="image">
          <img src="../../assets/selse/4.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>

      <article class="style5">
        <span class="image">
          <img src="../../assets/selse/5.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>

      <article class="style6">
        <span class="image">
          <img src="../../assets/selse/6.jpg" alt="" />
        </span>
        <a href="car-details.html">
          <h2>Lorem ipsum dolor sit amet, consectetur</h2>

          <p><del>$11 999</del> <strong>$11 779</strong></p>

          <p>
            <i class="fa fa-dashboard"></i> 130 000km &nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cube"></i> 1800 cc&nbsp;&nbsp;&nbsp;&nbsp;
            <i class="fa fa-cog"></i> Manual
          </p>
        </a>
      </article>
    </section>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
h1 {
  color: rgb(134, 121, 121);
  margin-left: 40px;
  margin-top: 45px;
}
.tiles {
  display: flex;
  position: relative;
  flex-wrap: wrap;

  margin-left: 5px;
}

.tiles article {
  transition: transform 0.5s ease, opacity 0.5s ease;
  position: relative;
  width: calc(33.3333333333% - 2.5em);
  margin: 2.5em 0 0 2em;
}

.tiles article > .image {
  transition: transform 0.5s ease;
  position: relative;
  display: block;
  width: 100%;
  border-radius: 4px;
  overflow: hidden;
}

.tiles article > .image img {
  display: block;
  width: 100%;
}

.tiles article > .image:before {
  pointer-events: none;

  transition: background-color 0.5s ease, opacity 0.5s ease;
  content: "";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 1;
  z-index: 1;
  opacity: 0.6;
}

.tiles article > a {
  display: flex;

  flex-direction: column;

  align-items: center;

  justify-content: center;

  transition: background-color 0.5s ease, transform 0.5s ease;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 1em;
  border-radius: 4px;
  border-bottom: 0;
  color: #ffffff;
  text-align: center;
  text-decoration: none;
  z-index: 3;
}

.tiles article > a > :last-child {
  margin: 0;
}

.tiles article > a:hover {
  color: #ffffff !important;
}

.tiles article > a h2 {
  margin: 0;
}

.tiles article > a .content {
  transition: max-height 0.5s ease, opacity 0.5s ease;
  width: 100%;
  max-height: 0;
  line-height: 1.5;
  margin-top: 0.35em;
  opacity: 0;
}

.tiles article > a .content > :last-child {
  margin-bottom: 0;
}

.tiles article.style1 > .image:before {
  background-color: #f2849e;
}

.tiles article.style2 > .image:before {
  background-color: #7ecaf6;
}

.tiles article.style3 > .image:before {
  background-color: #7bd0c1;
}

.tiles article.style4 > .image:before {
  background-color: #c75b9b;
}

.tiles article.style5 > .image:before {
  background-color: #ae85ca;
}

.tiles article.style6 > .image:before {
  background-color: #8499e7;
}

body:not(.is-touch) .tiles article:hover > .image {
  transform: scale(1.1);
}

body:not(.is-touch) .tiles article:hover > .image:before {
  background-color: #333333;
  opacity: 0.35;
}

body:not(.is-touch) .tiles article:hover > .image:after {
  opacity: 0;
}

body:not(.is-touch) .tiles article:hover .content {
  max-height: 15em;
  opacity: 1;
}

body.is-preload .tiles article {
  transform: scale(0.9);
  opacity: 0;
}

body.is-touch .tiles article .content {
  max-height: 15em;
  opacity: 1;
}

@media screen and (max-width: 1280px) {
  .tiles {
    margin: -1.25em 0 0 -1.25em;
  }

  .tiles article {
    width: calc(33.3333333333% - 1.25em);
    margin: 1.25em 0 0 1.25em;
  }
}

@media screen and (max-width: 980px) {
  .tiles {
    margin: -2.5em 0 0 -2.5em;
  }

  .tiles article {
    width: calc(50% - 2.5em);
    margin: 2.5em 0 0 2.5em;
  }
}

@media screen and (max-width: 736px) {
  .tiles {
    margin: -1.25em 0 0 -1.25em;
  }

  .tiles article {
    width: calc(50% - 1.25em);
    margin: 1.25em 0 0 1.25em;
  }

  .tiles article:hover > .image {
    -moz-transform: scale(1);
    -webkit-transform: scale(1);
    -ms-transform: scale(1);
    transform: scale(1);
  }
}

@media screen and (max-width: 480px) {
  .tiles {
    margin: 0;
  }

  .tiles article {
    width: 100%;
    margin: 1.25em 0 0 0;
  }
}
</style>
