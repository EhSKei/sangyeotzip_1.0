<script>
    import { onMount } from "svelte";
    import Hero from "../lib/Hero.svelte";
    import Image from "../lib/Image.svelte";

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

<Hero chapterCode="5" bgCode="062-1">
    <svelte:fragment slot="header">5부</svelte:fragment>
    <svelte:fragment slot="title">삼척과 동해 지역의 상엿집들</svelte:fragment>
    <svelte:fragment slot="desc">
        국립민속박물관 상엿집 조사팀은 맹방리 상엿집 외에 다른 상엿집들을
        조사하였습니다. 많은 상엿집을 찾지는 못했으나 삼척과 동해 지역의
        전형적인 상엿집들의 모습이라고 생각되어 소개합니다. 삼척 맹방리 상엿집에
        비해서 건축된 시기가 늦은 상엿집들입니다. 벽돌, 슬레이트지붕,
        시멘트마감이 되어 있는 것이 특징입니다. 상엿집들은 대부분 마을 사람들의
        기억 속에서 조차 사라진지 오래인 것들이 많아서 위치를 찾기도 매우
        어려웠습니다. 또한 상엿집의 관리 상태도 매우 부실하여 접근조차 힘든
        곳들도 있었습니다.
    </svelte:fragment>
</Hero>

<section class="article-container">
    <div class="article">
        <div class="article grid-2">
            <Image chapterCode="5" imgCode="060-1" />
            <Image chapterCode="5" imgCode="060-2" />
        </div>
        <p class="article-image-desc">동해시 구미동 상엿집</p>
        <div>
            <span class="article-title d-block"
                >5-1. 동해시 구미동 상엿집
                <hr /></span>
            <p class="article-text">
                동해시 구미동 상엿집은 마을에서 공동으로 관리하던 상엿집이
                아니라 인근의 공동묘지에서 장례용으로 사용되던 상여를 보관하던
                곳입니다. 상엿집의 상태는 매우 불량하여 곧 벽체가 무너질 것처럼
                위태로워 보였습니다. 내부에 상여는 없었고 쓰레기들과
                잡동산이들만 있었고, 풀이 무성해서 접근하기가 어려운
                상태였습니다. 건축된 시기는 1970년대 정도로 추정됩니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pt-0">
    <div class="article">
        <div class="article grid-2">
            <Image chapterCode="5" imgCode="061-1" />
            <Image chapterCode="5" imgCode="061-2" />
        </div>
        <p class="article-image-desc">동해시 북평동 상엿집</p>
        <div>
            <span class="article-title d-block">
                5-2. 동해시 북평동 상엿집

                <hr /></span>
            <p class="article-text">
                동해시 북평동 상엿집은 마을에서 공동으로 관리하던 상엿집입니다.
                다만 현재 내부에 상여는 없었고 쓰레기와 잡동산이만 있었습니다.
                벽돌로 쌓은 벽체에 슬레이트 지붕을 올린 형태로 지붕 일부가
                떨어져 나가서 매우 흉물스러운 모습니다. 건축된 시기는 1970년대
                정도로 추정됩니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pt-0">
    <div class="article">
        <div class="article grid-2">
            <Image chapterCode="5" imgCode="062-1" />
            <Image chapterCode="5" imgCode="062-2" />
        </div>
        <p class="article-image-desc">삼척시 양리 상엿집</p>
        <div>
            <span class="article-title">
                5-3. 삼척시 양리 상엿집

                <hr /></span>

            <p class="article-text">
                삼척시 양리 상엿집은 현재도 마을에서 관리가 되는 상엿집입니다.
                크기는 가로 429센치미터, 높이 190센치미터, 폭은
                280센치미터입니다. 지붕은 슬레이트 지붕이고 벽은 벽돌을 쌓고
                시멘트로 마감하였습니다. 마을에서 따로 관리자를 지정하여
                관리하고 있으며 열쇠로 문이 잠겨 있습니다. 비교적 관리 상태는
                좋았습니다. 마을의 원로인 홍두의씨(1944년생)에 의하면
                지금으로부터 7~8년 전인 2015년 경에 전선녀 할머님의 상례 때
                상여를 사용한 것이 마지막이었다고 합니다. 상엿집 안에는 나무로
                틀을 짜고 철제 장식이 달린 상여가 보관되어 있다고 합니다. 상여꾼
                8명이 메는 큰 상여라고 합니다.
            </p>
        </div>
    </div>
</section>
