<script>
    import { onMount } from "svelte";

    import { Swiper, SwiperSlide } from "swiper/svelte";
    import { Navigation, Pagination, EffectCards } from "swiper";
    import Hero from "../lib/Hero.svelte";

    import AOS from "aos";

    onMount(() => {
        let aosSections = document.querySelectorAll("section");
        aosSections.forEach((item, i) => {
            item.setAttribute("data-aos", "fade-up");
        });

        AOS.init({
            duration: 1000,
            once: false,
        });

        window.scrollTo(0, 0);
    });
</script>

<Hero chapterCode="2" bgCode="023">
    <svelte:fragment slot="header">3부</svelte:fragment>
    <svelte:fragment slot="title">삼척 맹방리 상엿집 도면</svelte:fragment>
</Hero>

<section class="article-container">
    <div class="article">
        <p class="article-text">
            3부의 상엿집 도면은 강원대학교 건축학과 최장순 교수팀에서
            제작하였습니다.
        </p>
    </div>
</section>

<div class="w-100 vh-100">
    <Swiper
        spaceBetween="{0}"
        slidesPerView="{1}"
        modules="{[Navigation, Pagination]}"
        navigation
        pagination
        on:slideChange="{() => console.log('slide change')}"
        on:swiper="{(e) => console.log(e.detail[0])}"
        class="w-100 vh-100">
        {#each Array(8) as item, index}
            <SwiperSlide>
                <img
                    src="./chapter03/Binder1_Page_{index + 1}.jpg"
                    alt=""
                    class="w-100 h-100"
                    style="object-fit: scale-down" />
            </SwiperSlide>
        {/each}
    </Swiper>
</div>
