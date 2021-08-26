<template>
  <Scroll/>
</template>

<script>
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";

gsap.registerPlugin(ScrollTrigger);
export default {
  mounted() {
         const tl_intro = gsap.timeline({
                                scrollTrigger: {
                                    trigger: ".trigger-one",
                                    start: "2%",
                                    end: "110%",
                                    scrub: true,
                                    //pin: true,
                                    //    pinSpacing: false,
                                       markers: true,
                                    id: "scrub"
                                  //  onEnter: () => $(".studio__header__logo").addClass('active'),
                                  //  onLeaveBack: () => $(".studio__header__logo").removeClass('active'),
                                }

                            });

                            tl_intro
                                .to(".background-image__two", {opacity: 1}, 0)

     const tl_intro_2 = gsap.timeline({
                                scrollTrigger: {
                                    trigger: ".trigger-two",
                                    start: "2%",
                                    end: "110%",
                                    scrub: true,
                                    //pin: true,
                                    //    pinSpacing: false,
                                       markers: true,
                                    id: "scrub"
                                  //  onEnter: () => $(".studio__header__logo").addClass('active'),
                                  //  onLeaveBack: () => $(".studio__header__logo").removeClass('active'),
                                }

                            });

                            tl_intro_2
                                .to(".background-image__three", {opacity: 1}, 0)


     const tl_intro_logo = gsap.timeline({
                                scrollTrigger: {
                                    trigger: ".trigger-logo",
                                    start: "2%",
                                    end: "110%",
                                    scrub: true,
                                    //pin: true,
                                    //    pinSpacing: false,
                                       markers: true,
                                    id: "scrub"
                                  //  onEnter: () => $(".studio__header__logo").addClass('active'),
                                  //  onLeaveBack: () => $(".studio__header__logo").removeClass('active'),
                                }

                            });

                            tl_intro_logo
                                .to(".logo", {scale: 0.5}, 0)
                               

                        
  }
}
</script>
