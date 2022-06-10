<template>
  <HeaderTemp />
  <SectionTemp />
  <FooterTemp url_name="Roman Matviy 2022" />
</template>

<script>
//jQuery
import $ from 'jquery';

//GSAP
import gsap from 'gsap';
// get GSAP other plugins:

//GSAP ScrollTrigger
import { ScrollTrigger } from "gsap/ScrollTrigger";

// import { TimelineMax } from 'gsap';
// import Flip from "gsap/Flip";
// import Draggable from "gsap/Draggable";

gsap.registerPlugin(ScrollTrigger);

import HeaderTemp from './components/HeaderTemp.vue';
import SectionTemp from './components/SectionTemp.vue';
import FooterTemp from './components/FooterTemp.vue';

export default {
  name: 'App',
  components: {
    HeaderTemp,
    SectionTemp,
    FooterTemp,
  },
};

$(document).ready(function fixedHeader() {

  //point
  $('.point').on('click', function () {
    if ($(this).hasClass('active')) {
      $(this).removeClass('active');
    } else {
      $(this).addClass('active');
    }
    $('.point').not(this).removeClass('active');
  });

  //ball call
  var windows = $(window);
  var screenSize = windows.width();

  windows.on('scroll', function () {
    var scroll = windows.scrollTop();
    var sticky = $('#header');
    var headerHeight = sticky.height();

    //#btn-order
    var ball = $('#btn-order');
    var blockPos = $('.howWork-section').position().top;

    if (scroll) {
      ball.css('transform', 'translate(0, 70px)');
      ball.css('width', '176px');
      ball.css('height', '176px');

      if (scroll > blockPos) {
        ball.css('transform', 'translate(0, 300px)');
        ball.css('display', 'none');

      } else {
        ball.css('transform', 'translate(0, 70px)');
        ball.css('display', 'block');
      }

    } else {
      ball.css('transform', 'translate(0, 0)');
      ball.css('width', '195px');
      ball.css('height', '195px');
      ball.css('display', 'block');
    }

    //#header
    if (screenSize >= 320) {
      if (scroll < headerHeight) {
        sticky.removeClass('is-sticky');
      } else {
        sticky.addClass('is-sticky');
      }
    }
  });
});

gsap.config({
  nullTargetWarn: false,
  trialWarn: false,
});

import { CSSPlugin } from 'gsap/CSSPlugin';
gsap.registerPlugin(CSSPlugin);

function slideElem(elem) {

  $('.howWork-wrapper__image').removeClass('active');

  var item = $(`#${elem}`);
  item.addClass('active');

  var animateIn = gsap.timeline({
    scrollTrigger: {
      start: "top top",
      markers: false,
      toggleActions: "play none none reverse",
    }
  });

  animateIn.fromTo(item, {
    right: '-140vw',
    left: 'none',
  }, {
    right: '0vw',
    left: 'none',
    ease: "power4",
    duration: 2,
  });


  gsap.to('progress', {
    value: 50,
    ease: 'none',
    scrollTrigger: {
      trigger: "#mySection",
      scrub: 0.2,
      start: "-600px top"
    }
  });
}

// wait until DOM is ready
document.addEventListener('DOMContentLoaded', function (event) {
  event.init;

  // wait until window is loaded - all images, styles-sheets, fonts, links, and other media assets
  // you could also use addEventListener() instead
  window.onload = function () {
    // OPTIONAL - waits til next tick render to run code (prevents running in the middle of render tick)
    window.requestAnimationFrame(function () {
      var windows = $(window);
      var screenSize = windows.width();

      $('.menu .menu-item').on('click', function () {
        const toActive = $(this).addClass('active');
        const thisSlide = $(this).data('elem');
        slideElem(thisSlide);

        $('.howWork-wrapper .howWork-wrapper__image').removeClass('fixed');

        $('#slide1').addClass('fixed');
        $(`#${thisSlide}`).addClass('fixed').css('display', 'block');

        $('.menu .menu-item').each(function () {
          const getText = $(this).text();
          const newText = getText.replace('→', '');
          $(this).text(newText);
        });

        $('.menu .menu-item').removeClass('active');
        const text = $(this).text();
        $(this).text('→' + text);

        gsap.to(toActive, { opacity: 1 }, { opacity: '0.7' })
        $(toActive).addClass('active');
      });


      if (screenSize > 991) {

        //Order button

        Order.prototype.enterAnimation = function () {
          gsap.to(this.el, { duration: .5, scale: 1, delay: 1.3, onComplete: this.infinityRotate });
        }

        Order.prototype.infinityRotate = function () {
          gsap.to(this.text, { rotation: 360, repeat: -1, ease: 'none', duration: 40 });
        }

        Order.prototype.addEvents = function () {
          window.addEventListener('mousemove', this.move);
          this.el.addEventListener('mouseenter', this.onEnter);
          this.el.addEventListener('mouseleave', this.onLeave);
        }

        Order.prototype.calculateDistance = function (rect, mouseX, mouseY) {
          return Math.floor(Math.sqrt(Math.pow(mouseX - (rect.centerX), 2) + Math.pow(mouseY - (rect.centerY), 2)));
        }

        Order.prototype.onEnter = function () {
          gsap.to(this.background, { duration: .4, scale: 1 });
        }

        Order.prototype.onLeave = function () {
          gsap.to(this.background, { duration: .4, scale: .77 });
        }

        Order.prototype.move = function (event) {
          const rect = this.el.getBoundingClientRect();
          rect.centerX = rect.x + (rect.width / 2);
          rect.centerY = rect.y + (rect.height / 2) + window.scrollY;

          const mouseX = event.pageX;
          const mouseY = event.pageY;
          const deltaX = Math.floor((rect.centerX - mouseX)) * -0.45;
          const deltaY = Math.floor((rect.centerY - mouseY)) * -0.45;
          const distance = this.calculateDistance(rect, mouseX, mouseY);

          if (window.innerWidth > 767) {
            if (distance < this.distance) {
              gsap.to(this.el, { duration: .4, x: deltaX, y: deltaY, ease: 'power2.out' });
              gsap.to(this.textWrap, { duration: .4, x: deltaX / 2, y: deltaY / 2, ease: 'power2.out' });
            } else {
              gsap.to(this.el, { duration: .45, x: 0, y: 0 });
              gsap.to(this.textWrap, { duration: .45, x: 0, y: 0 });
            }
          }
        }

        const order = new Order(document.getElementById('btn-order'));
        order.init;

        // MoveCard
        moveCart('#card1', 80, 1);
        moveCart('#card2', 120, 2);
        moveCart('#card3', 160, 3);
        moveCart('#card4', 200, 4);

        // MoveHowWorkBlock
        moveHowWorkBlockElem('.howWork-wrapper__left-text', 50, 3);
        moveHowWorkBlockElem('.howWork-wrapper__right-text', 50, 3);

        $('.project').each(function () {
          var menu = $(this).find('.howWork-wrapper__menu');
          var projectInfo = $(this).find('.howWork-wrapper__image');

          var animateIn = gsap.timeline({
            scrollTrigger: {
              trigger: menu,
              start: "-500px center",
              markers: false,
              toggleActions: "play none none reverse",
            }
          });

          var upImg = gsap.timeline({
            scrollTrigger: {
              trigger: '#block1',
              start: "-100px center",
              markers: false,
              toggleActions: "play none none reverse",
            }
          });

          upImg.fromTo(projectInfo, {
            top: '50px',
          }, {
            top: 0,
            transform: 'ease',
            ease: "power4",
            duration: 1,
          });

          animateIn.fromTo(projectInfo, {
            left: '-10vw',
            scale: 0.8,
          }, {
            left: '0vw',
            scale: 1,
            transform: 'none',
            ease: "power4",
            duration: 2,
          });

          animateIn.fromTo(menu, {
            left: '-40vw'
          }, {
            left: '0vw',
            ease: "power4",
            duration: 0.5,
            // start: "-800px top",
          });


        });

        gsap.to('progress', {
          value: 50,
          ease: 'none',
          scrollTrigger: {
            trigger: "#mySection",
            scrub: 0.2,
            start: "-600px top"
          }
        });
      }
    });
  };
});

function Order(el) {
  if (el === null) {
    return;
  }

  this.el = el;
  this.textWrap = el.querySelector('.btn-order-text-wrap');

  this.text = el.querySelector('.btn-order-text');
  this.background = el.querySelector('.btn-order-background');
  this.distance = 150;

  this.move = this.move.bind(this);
  this.infinityRotate = this.infinityRotate.bind(this);
  this.onEnter = this.onEnter.bind(this);
  this.onLeave = this.onLeave.bind(this);

  this.addEvents();
  this.enterAnimation();
}


function moveCart(elem, pos, sec = 1) {
  ScrollTrigger.create({
    trigger: '.clear-wrapper',
    animation: gsap.fromTo(elem, { top: pos }, { top: 0 }),
    pin: true,
    start: '-500 top',
    end: 'bottom bottom',
    scrub: sec, // I like the 1 sec delay, set to true for exact anime on scroll
    markers: false,
  });
}

function moveHowWorkBlockElem(elem, pos, sec = 1) {
  ScrollTrigger.create({
    trigger: '#block1',
    animation: gsap.fromTo(elem, { top: pos }, { top: 0 }),
    pin: true,
    start: '-600 top',
    end: 'bottom bottom',
    scrub: sec, // I like the 1 sec delay, set to true for exact anime on scroll
    markers: false,
  });
}

</script>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.container {
  max-width: 1740px;
  width: 100%;
  margin: 0 auto;

  @media (max-width: 1380px) {
    max-width: 1320px;
  }

  @media (max-width: 1200px) {
    max-width: 1140px;
  }

  @media (max-width: 992px) {
    max-width: 960px;
  }

  @media (max-width: 768px) {
    max-width: 720px;
  }

  @media (max-width: 576px) {
    max-width: 540px;
  }
}
</style>
