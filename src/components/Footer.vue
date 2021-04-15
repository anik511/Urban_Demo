<template>
  <div class="main-container footer-con">
    <footer class="footer-section">
      <div class="sub-con">
        <div class="footer-content">
          <div class="row">
            <div class="col span_1_of_5">
              <div class="footer-widget">
                <div class="footer-logo">
                  <a href="#"
                    ><img
                      src="../assets/Logo Footer.png"
                      class="img-fluid"
                      alt="logo"
                  /></a>
                </div>
                <div class="footer-social-icon">
                  <a href="#"
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-facebook"
                    >
                      <path
                        d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"
                      ></path></svg
                  ></a>
                  <a href="#"
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-twitter"
                    >
                      <path
                        d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"
                      ></path></svg
                  ></a>
                  <a href="#"
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-linkedin"
                    >
                      <path
                        d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                      ></path>
                      <rect x="2" y="9" width="4" height="12"></rect>
                      <circle cx="4" cy="4" r="2"></circle></svg
                  ></a>
                  <a href="#"
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-youtube"
                    >
                      <path
                        d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.25 29 29 0 0 0-.46-5.33z"
                      ></path>
                      <polygon
                        points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02"
                      ></polygon></svg
                  ></a>
                  <a href="#"
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-instagram"
                    >
                      <rect
                        x="2"
                        y="2"
                        width="20"
                        height="20"
                        rx="5"
                        ry="5"
                      ></rect>
                      <path
                        d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"
                      ></path>
                      <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg
                  ></a>
                </div>
                <div class="footer-text">
                  <p>
                    Every spring I start going through dress withdrawals and go
                    crazy over all the pretty.
                  </p>
                </div>
              </div>
            </div>
            <div class="col span_1_of_5">
              <div class="footer-widget pd-l">
                <ul>
                  <li v-for="(manulist, index) in manulists" :key="index">
                    <a :href="manulist.url">{{ manulist.title }}</a>
                  </li>
                </ul>
              </div>
            </div>
            <div class="col span_1_of_5">
              <div class="footer-widget pd-l">
                <Lists :lists="supportlists" />
              </div>
            </div>
            <div class="col span_1_of_5">
              <div class="footer-widget">
                <Lists :lists="tearmslists" />
              </div>
            </div>
            <div class="col span_1_of_5">
              <div class="footer-widget">
                <div class="footer-text">
                  <h3>Subscribe</h3>
                </div>
                <div class="subscribe-form">
                  <form action="#">
                    <input
                      class="icon-input-text-field"
                      type="text"
                      placeholder="your email"
                    />
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather feather-arrow-right icon-input-icon"
                    >
                      <line x1="5" y1="12" x2="19" y2="12"></line>
                      <polyline points="12 5 19 12 12 19"></polyline>
                    </svg>
                  </form>
                </div>
                <div class="send-mail">
                  <h4>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="40"
                      height="40"
                      viewBox="0 0 24 24"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="3"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      class="feather-m feather-mail mail"
                    >
                      <path
                        d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"
                      ></path>
                      <polyline points="22,6 12,13 2,6"></polyline></svg
                    ><span>mail@example.com</span>
                  </h4>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Lists from "./footerComp/Lists.vue";
export default {
  components: { Lists },
  name: "Footer",
  data() {
    return {
      manulists: [
        {
          url: "#",
          title: "Shop",
        },
        {
          url: "#",
          title: "Products",
        },
        {
          url: "#",
          title: "Collections",
        },
        {
          url: "#",
          title: "About us",
        },
        {
          url: "#",
          title: "Company",
        },
        {
          url: "#",
          title: "Blog",
        },
      ],
      supportlists: [
        {
          url: "#",
          title: "Support",
        },
        {
          url: "#",
          title: "Reviews",
        },
        {
          url: "#",
          title: "Careers ",
        },
        {
          url: "#",
          title: "Contact us",
        },
        {
          url: "#",
          title: "Privacy Policy",
        },
        {
          url: "#",
          title: "Refund Policy",
        },
      ],
      tearmslists: [
        {
          url: "#",
          title: "Tearms & Condition",
        },
        {
          url: "#",
          title: "FAQ’s Delivery",
        },
        {
          url: "#",
          title: "Returns ",
        },
      ],
    };
  },
};
</script>

<style scoped>
.footer-con {
  margin-top: 6rem;
}
.sub-con {
  padding: 0 6rem;
  box-sizing: border-box;
  margin: 0 auto;
  font-family: Open Sans;

  font-size: 18px;
  line-height: 27px;
}
ul {
  margin: 0px;
  padding: 0px;
}
.footer-section {
  background: #6e98a6;
  position: relative;
  border-radius: 1rem;
  color: #fff;
  padding: 5rem 0;
}
a {
  color: #fff;
}

.footer-content {
  position: relative;
  z-index: 2;
}
.footer-pattern img {
  position: absolute;
  top: 0;
  left: 0;
  height: 330px;
  background-size: cover;
  background-position: 100% 100%;
}
.footer-logo {
  margin-bottom: 2rem;
}
.footer-logo img {
  max-width: 11.8rem;
}
.footer-text p {
  padding-top: 2rem;
  font-size: 1.4rem;
  line-height: 2.8rem;
}
.footer-text h3 {
  font-size: 1.8rem;
}

.footer-social-icon a {
  font-size: 16px;
  margin-right: 15px;
}

.footer-widget ul li {
  width: 50%;
  margin-bottom: 12px;
}
.footer-widget ul li a:hover {
  color: #878787;
}
.footer-widget ul li a {
  text-transform: capitalize;
}
.subscribe-form {
  position: relative;
  overflow: hidden;
}
.subscribe-form input {
  width: 100%;
  padding: 0.5rem 0;
  border: 0px !important;
  background: #92b2bc;
  border-bottom: 1px solid #fff !important;
  color: #fff;
}
input:focus {
  background: #92b2bc;
  border: 0px !important;
  border-bottom: 1px solid #fff !important;
}
.pd-l {
  padding-left: 6rem;
}
.feather {
  width: 20px;
  height: 20px;
  stroke: currentColor;
  stroke-width: 1;
  stroke-linecap: round;
  stroke-linejoin: round;
  fill: none;
}
.feather-m {
  width: 22px;
  height: 22px;
  stroke: currentColor;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
  fill: none;
}
.mail {
  top: 0%;
  transform: translateY(14%);
}
.icon-input-icon {
  position: absolute;
  top: 50%;
  right: 0.5rem;
  transform: translateY(-50%);
}
form ::placeholder {
  color: #fff;
  opacity: 0.8;
  font-size: 1.2rem;
}

.send-mail {
  padding-top: 2rem;
}
.send-mail span {
  margin-left: 0.5rem;
  font-family: Open Sans;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 25px;
  letter-spacing: 0em;
  text-align: left;
}
</style>
