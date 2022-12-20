<script>
    import { onMount } from "svelte";
    import Hero from "../lib/Hero.svelte";
    import Image from "../lib/Image.svelte";
    import Subhero from "../lib/Subhero.svelte";

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

    function imgPath(chapterCode, imgCode) {
        return "./chapter0" + chapterCode + "/" + imgCode + ".webp";
    }
</script>

<Hero chapterCode="2" bgCode="017">
    <svelte:fragment slot="header">2부</svelte:fragment>
    <svelte:fragment slot="title"
        >삼척 맹방리 상엿집의
        <br>
         건축학적 특징</svelte:fragment>
</Hero>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <Subhero chapterCode="2" imgCode="012">
        <svelte:fragment slot="header"
            >망자의 마지막 길을 위한 <br>
            예의, 꽃상여</svelte:fragment>

        <svelte:fragment slot="desc">
            “미국에선 롤스로이스로, 한국에선 꽃상여를 태워 보낸다.”고 하는
            우스갯소리가 있습니다. 예로부터 우리 조상들은 이승에서 저승으로 가는
            망자의 마지막 길을 초라하지 않도록 대우해 주는 것이 망자에 대한
            예의라고 생각했습니다. 화려하게 장식한 꽃상여는 망자가 이승에서의
            미련을 버리고 편안히 저승으로 가길 바라는 조상들의 마음이
            담겨있습니다. 이처럼 마을의 주민들이 초상이 났을 때 공동으로 이용할
            수 있도록 상여와 장례 용구들을 보관하는 장소가 바로 상엿집입니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">상여 (이창호 기증)</svelte:fragment>
    </Subhero>
</div>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="013">
                <svelte:fragment slot="desc">하맹방리 상엿집</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            삼척 하맹방리 상엿집은 상여를 보관하는 목적에 따라 전면 3칸, 측면
            1칸이라는 최소 규모로 축조하였습니다. 중앙 어칸의 기둥 간격이 가장
            크고, 좌우 양 측면의 협칸은 각각 어칸보다는 작으면서도 좌우 기둥의
            간격을 서로 다르게 축조하였습니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="2" imgCode="014">
                <svelte:fragment slot="desc">
                    하맹방리 상엿집의 측면
                </svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            내부 마루는 상여 등을 보존하기 위해 바닥으로 습기를 막고 통기를 시켜
            줄 요량으로 최소한의 높이로 설치하였습니다. 기단 없이 주춧돌을 놓아
            축조하였으며, 기둥 위에는 하나의 보를 걸치고 중심에 동자대공을 놓아
            종도리를 받치는 가장 간단한 3량집 구조입니다.
        </p>
    </div>
</section>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <Subhero chapterCode="2" imgCode="015">
        <svelte:fragment slot="header"
            >삼척 맹방리 상엿집의 <br /> 건축학적 특징</svelte:fragment>

        <svelte:fragment slot="desc">
            벽체는 자귀로 치목한 송판 널을 사용하였으며, 문은 두 개의 두껍고
            넓은 송판 널로 문둔테와 돌저귀순을 갖춘 판문입니다. 이는 간이한
            구조로 해체 수리가 쉬운 사개맞춤과 긴 장부맞춤 등의 기법으로
            축조하였다는 점 등은 하맹방리 상엿집에서 눈여겨볼 건축적
            특징들이라고 할 수 있습니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">하맹방리 상엿집</svelte:fragment>
    </Subhero>
</div>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="016">
                <svelte:fragment slot="desc">하맹방리 상엿집</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <h3 class="article-title">(1) 평면(平面)</h3>
            <hr />
            <p class="article-desc">
                평면은 전면 3칸, 측면 1칸으로 ‘ㅡ자형’입니다. 전면 기둥의 간격은
                중앙 어칸이 가장 큰 2,380mm이고, 좌우 양 측면의 협칸은 각각
                1,760mm, 1,330mm로 좌우 기둥 간격이 서로 다른 것이 특징입니다.
                양 측면의 기둥 간격은 각각 1,930mm입니다. 이를 자로 환산하면
                전면 중앙 칸은 8자 정도이고, 좌측과 우측 칸은 각각 5.8자, 4.4자
                정도이며 좌우 양 측면 칸은 6.4자 정도입니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="2" imgCode="017">
                <svelte:fragment slot="desc">
                    하맹방리 상엿집의 측면
                </svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            배면 기둥에는 상여를 받치는 데 쓰이는 연초대를 올려놓을 수 있도록 두
            개의 ‘ㄱ자형’ 구조재가 있습니다. 이것은 짧은 기둥(150X150mm) 머리를
            반턱으로 파서 그 위에 짧은 보(100X100mm)를 배면의 기둥에 장부를 파서
            끼우고 단주 위에 걸쳐놓은 형태로 되어 있습니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="018">
                <svelte:fragment slot="desc">
                    하맹방리 상엿집의 출입구와 마루
                </svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0 order-1 order-md-2">
            출입구에서 보았을 때 전체 2/3는 당초 지반인 모랫바닥으로 되어있고,
            우측 1/3은 마루로 되어있습니다. 마루는 기둥에 고정되어 있지 않고
            전면과 우측면의 벽에 붙여 시설한 것이 특징입니다. 크기는 우측 칸
            크기의 3/4 정도로 구조방식은 밑에 세로재(140X140mm)로 받치고 그 위에
            가로재(140X90mm)를 대어 장마루 널이 세로로 길게 놓아져 있습니다.
        </p>
    </div>
</section>

<section class="article-containe pb-0r">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="2" imgCode="019" />
        </div>
        <p class="article-text p-md-0">
            사람이 기거하거나 사용할 용도가 아니고 목재로 만들어진 상여 등을
            오래도록 보존하기 위해 모랫바닥으로부터 올라오는 습기를 막아주고
            통기를 시켜줄 요량으로 시설한 것이기 때문에 마룻바닥은 일반 민가에
            설치된 마룻바닥보다는 높이가 훨씬 낮습니다. 집에서 생활하는 살림
            용도의 마루는 높이가 일반적으로 450mm 이상이 되어야 하나, 상엿집에
            설치된 마루는 그 높이가 300mm 정도로 다소 낮습니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="016">
                <svelte:fragment slot="desc">하맹방리 상엿집</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <h3 class="article-title">(2) 좌향(坐向)</h3>
            <hr />
            <p class="article-desc">
                좌향이란 건물이 등을 지고 앉은 좌(坐)와 바라보는 향(向)을 합한
                말을 뜻합니다. 이 상엿집의 평면은 ‘ㅡ자형’ 즉, 일직선상에
                놓이기에 현 상엿집의 좌향은 남동향에 해당합니다. 이는 과거
                집터를 정할 때 동쪽은 부자, 남쪽은 장수, 서쪽은 가난, 북쪽은
                단명이라 보았기에 이 상엿집은 하맹방리 마을 주민의 건강과 부를
                염원하기 위해 남동향으로 배치하였다는 것을 알 수 있습니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article">
        <div class="article-text">
            <h3 class="article-title">(3) 초석(礎石)</h3>
            <hr />
            <p class="article-desc">
                그 외에도 경상남도 창원시 북면 화천리 시화마을의 선돌형
                장승(이관호·오세길 조사, 1996년 7월 31일)과 경상북도 긍릉군
                아포면 송천리 숭산마을의 문인석 장승(정승모 조사, 1989년 2월
                22일)이 있습니다. 이들 장승은 본래 장승으로 만들어진 것은 아니나
                마을 사람들이 후에 장승의 기능을 부여하여 마을의 수호신으로 삼은
                것이 특징입니다.
            </p>
        </div>
        <div class="row m-0 row-cols-1 row-cols-lg-3">
            <img
                src="{imgPath('2', '021-1')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('2', '021-2')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('2', '021-3')}"
                alt=""
                class="col"
                style="padding: 1ch" />
        </div>
        <p class="article-image-desc m-0 p-0">하맹방리 상엿집의 주춧돌</p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="022">
                <svelte:fragment slot="desc">하맹방리 상엿집</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <h3 class="article-title">(4) 기둥(柱)</h3>
            <hr />
            <p class="article-desc">
                기둥(180X180mm)은 입면의 수직적 요소로서 지붕의 용마루선 처마선
                등의 수평적 요소에 대비되는데 여기에 사용된 기둥은 단면이
                각형으로 4각 기둥입니다. 이러한 기둥은 20세기 중반 이후 목재소
                제대목을 쓸 때 많이 이용되었습니다. 보통 4치 정도를 많이 쓰는데
                본 상엿집에서는 6치를 쓴 것으로 보아 건립 당시에 매우 튼튼하게
                지어졌음을 알 수 있습니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="2" imgCode="023">
                <svelte:fragment slot="desc">중앙 가구</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0">
            <h3 class="article-title">(5) 가구(架構)</h3>
            <hr />
            <p class="article-desc">
                양 기둥 위에 하나의 보를 걸치고 그 위에 양 처마도리(180X140mm)를
                놓고 보 가운데 동자대공을 설치하고 그 위에 종도리(180X180mm)를
                놓아 서까래를 종도리와 처마도리 위에 놓아 지붕을 받치는 가장
                간단한 3량집입니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="024">
                <svelte:fragment slot="desc">인방 장부맞춤</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <p class="article-desc">
                이러한 3량집은 목구조 가운데 가장 간단한 구조로서 이러한 집을
                다른 말로 ‘세마루집’이라고도 합니다. 이것은 간편하게 짓는 헛간과
                같은 창고건물에 일반적으로 사용되는 구조로 기둥 상하에 사개맞춤
                구멍을 뚫고 처마도리와 토대, 보를 연결하고 돌보 위에 동자대공을
                이용하여 종도리를 받치게 되어있는 구법입니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div style="display: grid; gap: 2ch; place-items: center">
            <Image chapterCode="2" imgCode="025-2">
                <svelte:fragment slot="desc">
                    하맹방리 상엿집의 벽체
                </svelte:fragment>
            </Image>
        </div>
        <div class="place-self-center " style="display: grid; gap: 2ch">
            <div class="order-2 order-md-1">
                <Image chapterCode="2" imgCode="025-1" />
            </div>
            <div class="article-text p-md-0 order-1 order-md-2">
                <h3 class="article-title">(6) 벽체</h3>
                <h1><hr /></h1>
                <p class="article-desc">
                    벽은 송판으로 된 빈지벽으로 두께 30mm 정도의 두꺼운
                    나무판자(松板)를 하인방과 상인방에 만든 홈 사이에 송판을
                    세로로 끼워 벽체를 만들었습니다. 이러한 벽을 이 지역에서는
                    빈지벽, 널판벽, 널벽이라 하는데 널판을 전통 기법인 자귀로
                    깎고 다듬은 것으로 보아 상당히 오래되었을 것으로 추정됩니다.
                </p>
            </div>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article">
        <div class="article grid-2">
            <Image chapterCode="2" imgCode="26-1" />
            <Image chapterCode="2" imgCode="26-2" />
        </div>
        <p class="article-image-desc">강원도 정선군 북평면 숙암리 가옥</p>
        <p class="article-text">
            일반적으로 영동 남부권에서는 송판을 주로 상인방과 중인방 그리고
            하인방 사이의 벽 전체에 끼우고 영동 북부권에서는 중인방과 하인방
            사이에 널판을 끼우며, 영동 중부권에서는 혼재되어 중간적 성격을 띠고
            있습니다. 이 상엿집에서는 건물의 처마 높이가 낮아 중인방이 없는
            관계로 상인방과 하인방 사이에 송판을 끼워넣어 4면 모두가 통기가
            잘되는 빈지벽으로 되어있습니다. 상엿집은 사람이 기거하는 용도가 아닌
            장례에 필요한 물건을 보관하는 수납 목적의 창고 역할을 하는
            고방이기에 이러한 구조로 만들었습니다.
        </p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div
            style="display: grid; gap: 2ch; place-items: center; place-self:center; grid-template-rows: min-content min-content">
            <Image chapterCode="2" imgCode="027-4" />
            <Image chapterCode="2" imgCode="027-1">
                <svelte:fragment slot="desc">
                    하맹방리 상엿집의 양여닫이 판문, 문둔테와 돌귀저순
                </svelte:fragment>
            </Image>
        </div>
        <div class="place-self-center " style="display: grid; gap: 2ch">
            <div class="order-2 order-md-1">
                <Image chapterCode="2" imgCode="027-2" />
            </div>
            <p class="article-text p-md-0 order-1 order-md-2">
                출입문은 2개의 두껍고 넓은 송판 널로 된 판문으로서 바깥으로
                열게끔 되어있는 양여닫이 판문입니다. 상‧하인방 사이에 문설주를
                세우고 바깥쪽으로 상‧하인방에 문둔테를 붙인 뒤 구멍에 판문을
                달아 문을 여닫을 수 있도록 하였습니다. 판문의 한쪽 옆에는 아래
                위로 돌저귀순이 있고, 문꼴의 아랫귀에는 돌저귀순이 들어갈
                문둔테를 두고 돌저귀순을 끼워 넣어 판문을 여닫을 수 있게
                만들었습니다. 그러나 현재 상부 문둔테가 떨어져 나가 판문의 상부
                1/3지점에 철제 경첩을 달아 문을 여닫았던 흔적이 보입니다.
            </p>
            <div class="order-3">
                <Image chapterCode="2" imgCode="027-3" />
            </div>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article">
        <div class="article-text p-md-0">
            <h3 class="article-title">(7) 맞춤</h3>
            <h1><hr /></h1>
            <p class="article-desc">
                본 상엿집의 맞춤이란 기둥을 주초 위에 놓는 방법과 기둥머리에서
                보와 도리가 만나는 4부재 맞춤, 동자주의 상하 맞춤, 기타 기둥과
                인방과의 맞춤 등을 말합니다. 기둥머리에는 보와 도리가 얹어져
                짜맞춰지는데 소규모 건물에서는 대개 3가지 방법이 통용됩니다.
                이것은 우리나라 어느 지역에서나 통용되는 사항으로 하나는 촉꽂이
                맞춤이고 다른 하나는 사개맞춤이며, 또 다른 하나는
                장부맞춤입니다.
            </p>
        </div>
        <div class="article grid-2">
            <Image chapterCode="2" imgCode="028-1" />
            <Image chapterCode="2" imgCode="028-2" />
        </div>
        <p class="article-image-desc">상엿집의 맞춤</p>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="2" imgCode="029">
                <svelte:fragment slot="desc">기둥 사개맞춤</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <p class="article-desc">
                이 상엿집의 기둥 위에는 사개맞춤이 사용되었는데, 이것은 도리와
                보의 맞춤이 기둥 위에서 이루어지는 것으로 우리나라 전 지역에서
                가장 흔하게 사용되는 기법입니다. 사개란 기둥머리 네 귀에 보와
                도리가 같은 수평면으로 맞춤이 되도록 끼울 수 있게 만든 것입니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pb-0">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="2" imgCode="030">
                <svelte:fragment slot="desc">
                    동자대공 상하 맞춤
                </svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            보 위의 동자대공 상하 맞춤은 밑은 장부로 만들어 박고, 위는 종도리의
            단면을 반턱으로 따내고 거기에 동자대공을 통으로 끼워 넣는 수법을
            사용했습니다. 인방재의 맞춤은 긴 장부맞춤으로 하였는데, 인방에 긴
            장부를 만들어 끼워 긴 장부 끝이 기둥 밖으로 내밀도록 하고, 장부와
            기둥 구멍 사이에는 쐐기를 박아 고정되도록 하였습니다. 이러한 기법은
            강원도 지역에서 주로 볼 수 있는 기법이며, 간이한 건물이기에 해체나
            수리를 간단하게 할 수 있는 장점이 있습니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article">
        <div class="article-text">
            <h3 class="article-title">(8) 지붕</h3>
            <hr />
            <p class="article-desc">
                마을에서 가장 연장자인 홍영표 씨(1938년생)에 의하면, 당초 상엿집
                지붕에는 구운 토기와를 올렸으나 1970년대에 현재의 위치로
                옮기면서 골슬레이트로 지붕을 교체하였다고 합니다. 당시 사용했던
                암기와의 일부는 골슬레이트 지붕의 용마루를 뒤집어서 덮는 2단의
                암마룻장 기와로 사용하였습니다. 지붕의 형태는 맞배지붕으로
                지붕을 제외한 모든 재료는 당초 그대로 재사용하였다고 합니다.
            </p>
        </div>
        <div class="row m-0 row-cols-1 row-cols-lg-3">
            <img
                src="{imgPath('2', '031-1')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('2', '031-2')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('2', '031-3')}"
                alt=""
                class="col"
                style="padding: 1ch" />
        </div>
        <p class="article-image-desc m-0 p-0">하맹방리 상엿집 지붕</p>
    </div>
</section>

<div style="background-color:#212529; color: white">
    <section class="sub-hero-container">
        <div class="sub-hero">
            <div class="sub-hero-text">
                <h1 class="sub-hero-header">
                    삼척 맹방리 상엿집의<br>
                     건축학적 의의
                </h1>
                <hr />
                <p class="sub-hero-desc">
                    삼척 근덕면 맹방리에 소재한 상엿집은 120년 이상이나 된
                    오래된 연혁(1899년 중수)과 건축적 가치로 판단했을 때 과거
                    우리네의 의식주와 신앙, 행사 등에 관한 풍속이나 관습과
                    관련되어 사용되었던 건축물입니다. 삼척 맹방리 상엿집을
                    통해서 우리 민족의 가장 기본적인 건축문화의 특색을 살펴볼 수
                    있었습니다.
                </p>
            </div>
            <div>
                <Image chapterCode="2" imgCode="032-1">
                    <svelte:fragment slot="desc">
                        <slot name="imgDesc" />
                    </svelte:fragment>
                </Image>
                <Image chapterCode="2" imgCode="032-2">
                    <svelte:fragment slot="desc">
                        <slot name="imgDesc" />
                    </svelte:fragment>
                </Image>
            </div>
        </div>
    </section>
</div>
