<template>
  <div>
    <div class="contact">
      <div class="container">
        <div class="info fl-left">
          <h2>contact me</h2>
          <p>
            lorem ipsum dolor sit anemt,ea doming until epicuri iudicabit nam,
            te usu vritute placerat. purto brute disputando cu est. te usu
            vritute placerat. purto brute disputando cu est.
          </p>
          <p>
            Aleppo New name street<br />
            aleppo<br />
            S7K 123
          </p>
          <p>
            <strong>Email:</strong>Me@gmail.com<br />
            <strong>phone :</strong>0940052969
          </p>
        </div>
        <div class="smal">
          <form class="form fl-left ">
            <span>Name *</span>
            <input type="text" />
            <span>Email *</span>
            <input type="text" />
            <span>phone *</span>
            <input type="text" />

            <input type="submit" value="Send" />
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
/* start contact me*/
.contact {
  background-color: #f6f6f6;
  overflow: hidden;
  padding-top: 50px;
  padding-bottom: 70px;
  margin-top: 50px;
}
.contact .info {
  width: 50%;
  margin-right: 5%;
}
.contact h2 {
  color: #000000;
  margin-left: 40px;
}

.contact p {
  color: #000000;
  margin-left: 40px;
  line-height: 1.5;
  font-size: 23px;
}

.contact p stong {
  color: #d1d6da;
}

.contact .form {
  width: 45%;
}

.contact .form span {
  display: block;
  color: #000000;
  margin: 20px 0;
}
.contact .form input[type="text"] {
  appearance: none;
  background-color: transparent;
  border: none;
  border-radius: 0;
  border-bottom: solid 1px #c9c9c9;
  color: inherit;
  display: block;
  outline: 0;
  padding: 0;
  text-decoration: none;
  width: 90%;
}

.contact .form input[type="submit"] {
  box-shadow: none;
  background-color: #585858;
  color: #ffffff !important;
  padding: 10px 20px;
  border: 0;
  margin-top: 10px;
  display: block;
}
.fl-left {
  float: left;
}

/* end contact me */

@media screen and (max-width: 736px) {
  .contact {
    max-width: 736px;
    margin-left: 0px;
  }
  .contact .info {
    width: 50%;
    margin-right: 3%;
  }
  .contact .info h2 {
    margin-left: 0px;
  }
  .contact p {
    margin-left: 0px;
    line-height: 1.2;
    font-size: 14px;
  }

  .contact .form {
    width: 45%;
  }
}
/*
@media screen and (max-width: 480px) {
}*/
</style>
