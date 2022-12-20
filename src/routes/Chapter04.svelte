<script>
    import { onMount } from "svelte";
    import { fade } from "svelte/transition";
    import Hero from "../lib/Hero.svelte";
    import Image from "../lib/Image.svelte";
    import Navbar from "../lib/Navbar.svelte";
    import Subhero from "../lib/Subhero.svelte";

    import AOS from "aos"

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

    function imgPath(chapterCode, imgCode) {
        return "./chapter0" + chapterCode + "/" + imgCode + ".webp";
    }
</script>

<Hero chapterCode="4" bgCode="043">
    <svelte:fragment slot="header">4부</svelte:fragment>
    <svelte:fragment slot="title"
        >삼척 맹방리 상엿집 안에서 <br>
        발견된 것들</svelte:fragment>
</Hero>

<section class="article-container pb-0">
    <div class="article">
        <p class="article-text">
            홍영택씨에 의하면 20여 년 전만 하더라도 상엿집 안에 관을 싣는 상과
            관을 덮는 집 모양의 장막, 장식물 등이 보존되어 있었다고 합니다.
            그러나 현재는 상여를 운구할 때 사용하는 긴 장대 멜대 7개와 용도를 알
            수 없는 사각형 상자 2개, 관을 덮는 집 모양 장식, 위에 얹는 용도로
            보이는 둥근 반원통형 덮개 정도만 있었습니다.
        </p>
        <div class="article grid-2">
            <Image chapterCode="4" imgCode="035-1" />

            <Image chapterCode="4" imgCode="035-2" />
        </div>
        <p class="article-image-desc">상엿집 내부의 여러 가지 물건들</p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="4" imgCode="036">
                <svelte:fragment slot="desc"
                    >상엿집 안의 물건들을 꺼내는 조사자들.</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            상엿집 내부는 사람이 선뜻 들어가기에는 다소 무서운 공간이었습니다.
            먼지도 너무 많고 죽은 쥐도 있었습니다. 그럼에도 불구하고 용감한(?)
            조사자들은 상엿집 안의 모든 물건들을 꺼내서 조사하였습니다.
        </p>
    </div>
</section>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <Subhero chapterCode="4" imgCode="039">
        <svelte:fragment slot="header">4-1. 상여 장식</svelte:fragment>

        <svelte:fragment slot="desc">
            삼척 맹방리 상엿집 안에는 5개의 상여 장식이 남아 있었습니다. 상여
            장식 중 사람모양 인형을 꼭두라 부릅니다. 상여장식은 모양이 예쁘기
            때문에 도난당하기 쉽습니다. 삼척 맹방리 상엿집의 상여장식도 대부분
            도난당한 것으로 보이며 봉황 3개, 구슬 1개, 새모양 1개만
            남아있었습니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">상여 (이창호 기증)</svelte:fragment>
    </Subhero>
</div>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <Subhero chapterCode="4" imgCode="044">
        <svelte:fragment slot="header">4-2. 요여(腰輿)</svelte:fragment>

        <svelte:fragment slot="desc">
            <p class="article-desc">
                요여는 죽은 이를 매장한 후에 혼백과 신주를 모시고 돌아오는데
                사용되는 작은 가마입니다. 영여(靈輿)라고도 하는데 상여가 묘지로
                향할 때 맨 앞에 명정(銘旌: 죽은 이의 성명, 관직 등을 기록한
                기)이 서고 다음에 공포(功布: 관을 닦는 삼베) 그리고 요여와 상여
                순으로 행렬이 이루어 집니다.
            </p>
            <p class="article-desc" style="font-size: 0.9em">
                <i>
                    “요여는 손자나 큰 사위가 들고 간다. 요즘은 망자의 사진으로
                    요여를 대신한다. 회양에서는 상여가 나갈 때 하얀 꽃을 뿌렸다.
                    그리고 산에ᄁᆞ지 아이들이 따라오면 싸가지고 갔던 떡을 나누어
                    주었다.”
                    <br />
                </i>
                - 홍옥순(강원도 화천군 용담2리)
            </p>
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">수습된 요여 부속들</svelte:fragment>
    </Subhero>
</div>

<section class="article-container ">
    <div class="article">
        <div class="article-text">
            <p class="article-desc">
                삼척 맹방리 상엿집 안에 있던 요여는 상태가 매우 좋지 않았습니다.
                요여의 손잡이 부분과 하단부는 온전하였으나, 상단부는 지붕과 벽체
                일부만 남아있었습니다. 이 정도라도 남아있는 것이 다행이었습니다.
            </p>
        </div>
        <div class="row m-0 m-0 m-0 m-0 m-0 row-cols-1 row-cols-lg-3">
            <div class="col">
                <Image chapterCode="4" imgCode="045">
                    <svelte:fragment slot="desc">지붕</svelte:fragment>
                </Image>
            </div>
            <div class="col">
                <Image chapterCode="4" imgCode="046">
                    <svelte:fragment slot="desc">
                        하단부와 손잡이
                    </svelte:fragment>
                </Image>
            </div>
            <div class="col">
                <Image chapterCode="4" imgCode="047">
                    <svelte:fragment slot="desc">
                        측면 벽체 부속
                    </svelte:fragment>
                </Image>
            </div>
        </div>
    </div>
</section>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <section class="sub-hero-container">
        <div class="sub-hero">
            <div class="sub-hero-text">
                <h1 class="sub-hero-header">
                    4-3. 상여 상부 덮개
                    <br />
                    [유개: 帷蓋]와 기타 부속들
                    <hr />
                </h1>
                <p class="sub-hero-desc">
                    유개(帷蓋)는 상여의 맨 위 상부에서 관을 덮는 용도로 사용되는
                    덮개입니다. 목재로 만든 틀에 천을 둥글게 고정하여
                    만들었으며, 전면부에는 죽은 이의 극락왕생(極樂往生)을
                    기원하는 의미에서 연꽃 그림을 그려 넣었습니다.
                </p>
            </div>
            <div>
                <Image chapterCode="4" imgCode="048">
                    <svelte:fragment slot="desc">유개</svelte:fragment>
                </Image>
                <Image chapterCode="4" imgCode="049">
                    <svelte:fragment slot="desc">
                        유개 전면의 봉황그림
                    </svelte:fragment>
                </Image>
            </div>
        </div>
    </section>
</div>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="4" imgCode="050">
                <svelte:fragment slot="desc">운반대</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            상여를 운반하는데 쓰이는 기다란 장대입니다. 상엿집 내부에도 여러
            개가 있었으며, 상엿집 외부 벽체에도 3개가 놓여 있었습니다.
            상엿꾼들이 상여를 들고 운반할 때 손으로 잡는 장대입니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="4" imgCode="051">
                <svelte:fragment slot="desc">무명줄</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            무명으로 만든 매우 질긴 줄입니다. 상여를 들어서 운반할 때 상여를
            동여 메는데 사용하기도 하고, 상엿꾼들이 운반대를 잡기 편하게
            무명줄을 묶어서 잡기도 합니다. 10미터 이상의 긴 줄이었습니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="4" imgCode="052">
                <svelte:fragment slot="desc">운반대</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            유개(帷蓋) 위를 덮는 것으로 추정되는 천입니다. 테두리를 파랗게
            물들인 것이 특징입니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="4" imgCode="053">
                <svelte:fragment slot="desc">부속재료</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">상여의 기타 부속품입니다.</p>
    </div>
</section>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <section class="sub-hero-container">
        <div class="sub-hero">
            <div class="sub-hero-text">
                <h1 class="sub-hero-header">
                    4-4. 상여 부속 보관함,
                    <br />
                    나무그릇, 기와
                    <hr />
                </h1>
                <p class="sub-hero-desc">
                    삼척 맹방리 상엿집 안에는 상여부속들을 보관하기 위한 상자가
                    있었습니다. 발견 당시에는 상여 부속들이 상엿집 안에
                    아무렇게나 놓여져 있었습니다.
                </p>
            </div>
            <div>
                <Image chapterCode="4" imgCode="054">
                    <svelte:fragment slot="desc"
                        >발견당시 보관함</svelte:fragment>
                </Image>
            </div>
        </div>
    </section>
</div>

<section class="article-container pb-0">
    <div class="article">
        <Image chapterCode="4" imgCode="055">
            <svelte:fragment slot="desc">상여 부속 보관함</svelte:fragment>
        </Image>
        <p class="article-text">
            상여의 부속품들을 보관하는데 사용되는 나무 상자입니다. 상여를 사용한
            후 부속들을 해체하여 나무 상자 안에 보관합니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article">
        <div
            style="display:grid; grid-template-columns: repeat(2,1fr); align-items: flex-end">
            <Image chapterCode="4" imgCode="056">
                <svelte:fragment slot="desc">나무그릇 전면</svelte:fragment>
            </Image>
            <Image chapterCode="4" imgCode="057">
                <svelte:fragment slot="desc">나무그릇 후면</svelte:fragment>
            </Image>
        </div>
        <p class="article-text">
            상엿집 안에 있던 나무그릇입니다. 본래는 칠이 되어 있던 것으로
            보이는데 비바람에 상해서 칠이 벗겨지고 상태가 매우 좋지 않았습니다.
            상여가 가는 길에 여러 차례 제사를 지내는데, 그 때 이 나무그릇에
            음식들을 올려 놓고 사용했던 것으로 추정됩니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="4" imgCode="058">
                <svelte:fragment slot="desc">정리된 보관함</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            상엿집 안의 물건들을 모두 조사하고서 보관함에 물건들을 가지런히
            정리해서 다시 상엿집 안에 넣어 두었습니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="4" imgCode="059">
                <svelte:fragment slot="desc">기와</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            흙으로 빚어서 구워 만든 기와입니다. 상엿집의 기와가 많이 상해서
            현재는 슬레이트가 덮여 있는데 남아 있는 기와가 일부 슬레이트 지붕
            위에 올려져 있었습니다.
        </p>
    </div>
</section>
