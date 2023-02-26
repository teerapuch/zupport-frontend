<template>
  <section class="gradient-bg">
    <div class="cirle-bg">
        <div class="bg" data-bg="images/bg/circle.png" style="background-image: url(&quot;images/bg/circle.png&quot;);"></div>
    </div>
    <div class="container">
        <div class="join-wrap fl-wrap">
            <div class="flex flex-row">
                <div class="basis-3/4">
                    <h3>Do You Have Questions ?</h3>
                    <p>Lorem ipsum dolor sit amet, harum dolor nec in, usu molestiae at no.</p>
                </div>
                <div class="basis-1/4"><a href="contacts.html" class="join-wrap-btn">Get In Touch <i class="fa fa-envelope-o"></i></a></div>
            </div>
        </div>
    </div>
  </section>
</template>

<style scoped>
section {
    float: left;
    width: 100%;
    position: relative;
    padding: 80px 0;
    overflow: hidden;
    background: #fff;
    z-index: 1;
}
.gradient-bg {
  background: -webkit-linear-gradient(top, #3efddd, #91efb2);
}
.cirle-bg {
    position: absolute;
    right: 10%;
    width: 500px;
    height: 500px;
    bottom: -70%;
    z-index: 1;
    opacity: 0.1;
}
.container {
    max-width: 1224px;
    width: 92%;
    margin: 0 auto;
    position: relative;
    z-index: 5;
}
.join-wrap {
    padding: 10px 0 10px 30px;
    border-left: 1px solid rgba(255,255,255,0.21);
}
.fl-wrap {
    float: left;
    width: 100%;
    position: relative;
}
.join-wrap h3 {
    float: left;
    width: 100%;
    text-align: left;
    font-size: 34px;
    font-weight: 700;
    padding-bottom: 20px;
    color: #fff;
}
.join-wrap p {
    text-align: left;
    color: green;
    font-size: 18px;
}
p {
    font-size: 12px;
    line-height: 24px;
    padding-bottom: 10px;
    font-weight: 500;
    color: #4cc55e;
}
.join-wrap-btn {
    display: inline-table;
    padding: 20px 55px;
    text-transform: uppercase;
    background: #fff;
    border-radius: 30px;
    font-size: 11px;
    font-weight: 700;
    position: relative;
    top: 15px;
    box-shadow: 0px 0px 0px 7px rgb(255 255 255 / 40%);
}
</style>