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

<Hero chapterCode="1" bgCode="008">
    <svelte:fragment slot="header">1부</svelte:fragment>
    <svelte:fragment slot="title">삼척 맹방리 상엿집의 역사</svelte:fragment>
</Hero>

<section class="article-container">
    <div class="article">
        <p class="article-text">
            1부, 2부는 최장순,「삼척 근덕면 하맹방마을 상엿집 고찰」을 바탕으로
            작성하였습니다.
        </p>
    </div>
</section>

<div class="" style="background-color: #212529; color: white">
    <Subhero chapterCode="1" imgCode="001">
        <svelte:fragment slot="header"
            >마을공동체 문화의 상징, <br /> 상여와 상엿집</svelte:fragment>
        <svelte:fragment slot="desc">
            상례(喪禮)는 우리 조상들이 옛부터 중요하고 여겼던 4가지 예법인
            관혼상제(冠婚喪祭)의 하나입니다. 상여는 상례를 진행하는데 있어
            시신을 실어 묘지까지 나르는데 중요한 기구였습니다. 상엿집은 상여를
            보관하는 곳으로 마을에서 공동으로 관리하는 마을공동체 문화의
            상징이었습니다.
            <p class="article-desc" style="font-size: 0.8em">
                <br />
                경산 상엿집 : 아카이브번호 00633043 / 중요민속문화재 제266호 경산
                상엿집 (경북 경산시 하양리 학리 산 144-35) 피사체는 중요민속문화재
                제266호, (사)나라얼연구소 소장. 《『상례, 슬픔을 함께 나누다』, 국립민속박물관·경산시립박물관·꼭두박물관,
                2016》에 수록. 상세 내용은 각 이미지에 기술됨.
            </p>
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">경산 상엿집</svelte:fragment>
    </Subhero>
</div>

<section class="article-container">
    <div
        class="article grid-2"
        style="grid-template-rows: min-content min-content">
        <div style="display: grid; gap: 2ch">
            <Image chapterCode="1" imgCode="002-1">
                ><svelte:fragment slot="desc" />
            </Image>
            <p class="article-text p-md-0">
                상여는 사람과 영혼 사이 마지막 의례로써 시신을 담은 관을 장지로
                옮기고, 이승과 저승을 연결하는 매개물로서 상징성이 있습니다.
                상여는 혼백을 운반하는 영여와 시신을 묘소까지 운반할 때 사용하는
                제구를 통칭하여 사용하지만, 삼척시 근덕면 하맹방 마을에선
                일반적으로 제구를 상여라 합니다.
            </p>
        </div>
        <div class="place-self-center">
            <Image chapterCode="1" imgCode="002-2">
                <svelte:fragment slot="desc"
                    >상여(喪輿), 양주상여와회 다지소리보존회 상여 영상</svelte:fragment>
            </Image>
        </div>
    </div>
    <div class="article">
        <video
            src="https://d3pyyak0c50n14.cloudfront.net/sangyeotzip/chapter01-video-01.mp4"
            class="article-video"
            style="padding-block: 2.5ch"
            controls
            muted
            autoplay></video>
    </div>
</section>

<section class="article-container">
    <div class="article">
        <div class="row row-cols-3 m-0">
            <img
                src="{imgPath('1', '003-1')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('1', '003-2')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('1', '003-3')}"
                alt=""
                class="col"
                style="padding: 1ch" />
        </div>
        <p class="article-image-desc">
            『세종실록(世宗實錄)』, 『사례편람(四禮便覽)』
        </p>
        <p class="article-text">
            중국에서는 상여를 대여(大輿) 또는 온량(轀輬), 영거(靈車)라고도
            하는데 대여는 말 그대로 큰 수레이고, 온량은 평안히 누워쉬는 수레,
            영거는 시신을 담은 관, 즉 영구를 싣는 수레를 뜻합니다.
            우리나라에서는 『세종실록(世宗實錄)』과
            『순장국장록(殉葬國葬錄)』에서 주로 국상(國喪) 때에 큰 상여인
            대여(大輿)라는 단어를 볼 수 있습니다. 이후 조선 후기 학자인
            이재(李縡: 1680~1746)가 쓴『사례편람(四禮便覽)』의 상례(喪禮)에
            대여와 더불어 상여(喪輿)라는 단어가 나오며, 여기서 상여는 대여보다는
            간단한 소여(小輿)를 의미했습니다.
        </p>
        <p class="article-text" style="font-size:0.9em">
            세종실록 : 조선전기 제4대 왕 세종의 재위 기간 동안의 국정 전반에
            관한 역사를 다룬 실록 <br />
            사례편람 : 조선 후기의 학자·정치가 이재(李縡)가 편술한 관혼상제의 사례(四禮)에
            관한 종합적인 참고서 <br />
            사례편람 상여도 : 사례편람에 실린 상여도로 상여의 구조를 살펴볼 수 있음
            <br />
            고종황제 국장 : 고종황제 국장행렬과 대여, 고종황제 대여행렬을 바라보는
            시민들, 고종황제의 국장 대여
        </p>
        <div class="row row-cols-1 row-cols-lg-3 m-0">
            <img
                src="{imgPath('1', '003-4')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('1', '003-5')}"
                alt=""
                class="col"
                style="padding: 1ch" />
            <img
                src="{imgPath('1', '003-6')}"
                alt=""
                class="col"
                style="padding: 1ch" />
        </div>
        <p class="article-image-desc m-0 p-0">상여도, 고종황제 국장</p>
    </div>
</section>

<section class="article-container">
    <div class="article">
        <Image chapterCode="1" imgCode="005-9">
            <svelte:fragment slot="desc"
                >청도 신촌리 유월장 꽃상여</svelte:fragment>
        </Image>
        <div class="article-text">
            <span class="article-title">
                "꽃집”, 상엿집의 다른 이름
                <hr />
            </span>
            <p class="article-desc">
                상여에는 마을의 솜씨 좋은 목각 장인이 부재와 널빤지에 각종
                그림을 새겨 넣었습니다. 일반적으로 꽃장식을 많이 하였기에 흔히들
                상여를 꽃상여라 하며, 이러한 이유에서 였는지 상여를 보관하고
                있는 상엿집을 꽃집, 곳집, 행상집이라 부릅니다.
            </p>
            <p class="article-desc" style="font-size:0.8em">
                상여장식 : 아카이브번호 00633070 / 피사체는 꼭두박물관 소장.
                《『상례, 슬픔을 함께 나누다』, <br />
                국립민속박물관·경산시립박물관·꼭두박물관, 2016, 60쪽》에 수록.
                <br />
                청도 신촌리 유월장 꽃상여 : 아카이브번호 00139771 / 1997년 청도 이서면
                신촌리 유월장 조사 사업
            </p>
        </div>
        <div class="row row-cols-2 row-cols-md-3 m-0">
            {#each Array(8) as item, index}
                <img
                    src="{imgPath('1', '005-' + (index + 1))}"
                    alt=""
                    class="col"
                    style="padding: 1ch;" />
            {/each}
        </div>
    </div>
</section>

<div class="" style="background-color: #212529; color: white">
    <Subhero chapterCode="1" imgCode="006">
        <svelte:fragment slot="header"
            >삼척 맹방리 상엿집은 <br /> 언제 만들어졌을까?</svelte:fragment>
        <svelte:fragment slot="desc">
            삼척 맹방리 상엿집에는 보 위에 3개의 종도리가 가로로 길게
            놓여있습니다. 보통 규모가 작은 여염집의 경우 상량문은 도리 바로
            밑에, 규모가 있는 여염집의 경우는 장여 밑에 적어놓는 것이
            일반적입니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc">종도리</svelte:fragment>
    </Subhero>
</div>

<section class="article-container">
    <div class="article">
        <p class="article-text">
            삼척 맹방리 상엿집의 경우 특이하게 도리측면에
            “대한광무삼년기해삼월이십칠일중수복원상량지후일동무효백병소멸(大韓光武參年己荄三月二十七日重修僕願上樑之後一洞無效百病消滅)”이라
            적힌 상량문이 있습니다. 일반적으로 상량문의 양쪽 끝에는 용호(龍虎),
            용구(龍龜), 봉룡(鳳龍)의 두 글자가 서로 마주 보도록 쓰고, 그 사이에
            상량한 연월일시와 복을 비는 상서로운 글을 써넣기 마련이지만, 맹방리
            상엿집의 상량문에는 바로 상량한 연월일시와 축원 문구가 종도리 측면에
            적혀져 있습니다.
        </p>
        <p class="article-text">
            <b
                >상량문을 통해 맹방리 상엿집은 1899년 이전부터 마을의 공동
                시설로 존재했으며, 1899년에 중수되었던 것을 알 수 있습니다. 무려
                최소 120년 전에 만들어진 아무 오래된 상엿집입니다.</b>
        </p>
        <div class="article grid-2">
            <Image chapterCode="1" imgCode="007-1" />
            <Image chapterCode="1" imgCode="007-2" />
        </div>
        <p class="article-image-desc">상량문</p>
    </div>
</section>

<div class="" style="background-color: #212529; color: white">
    <Subhero chapterCode="1" imgCode="008">
        <svelte:fragment slot="header"
            >아낙네들의 정보교환 장소로 <br /> 활용되었던 옛 터</svelte:fragment>
        <svelte:fragment slot="desc">
            하맹방마을에서 가장 연장자인 홍영택씨(1938년생)에 의하면, 원래
            하맹방마을의 상엿집 위치는 현재 하맹방2리 마을회관 앞쪽인 삼척시
            근덕면 하맹방2길 43-13(하맹방리 303-6) 인근에 1970년대까지 있었으며,
            당시 이곳에는 상엿집 외에도 두레박으로 물을 긷는 마을 공동우물과 묘
            5~6기도 함께 있었다고 합니다. 1960년대 후반에 현재의 위치로
            옮겨졌다고 합니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc"
            >마을 중앙의 옛 상엿집 터</svelte:fragment>
    </Subhero>
</div>

<section class="article-container">
    <div class="article">
        <div class="article grid-2">
            <Image chapterCode="1" imgCode="009-1" />
            <Image chapterCode="1" imgCode="009-2" />
        </div>
        <p class="article-image-desc p-0 m-0">하맹방리 상엿집</p>
        <p class="article-text">
            이 곳은 마을의 대소사를 비롯하여 시시콜콜한 가정사 이야기까지 나눴던
            아낙네들의 정보 교환의 장소였습니다. 그러나 1970년대 민가가
            들어서면서 미관상의 이유로 현재 위치인 맹방해수욕장 근처 근덕면
            하맹방리 221-17 솔밭으로 옮기게 되었다고 합니다.
        </p>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div style="display: grid; gap: 2ch">
            <Image chapterCode="1" imgCode="010-1">
                <svelte:fragment slot="desc">
                    인천광역시 강화군 길상면 선두2리 상엿집, 충청북도 보은군
                    속리산면 사내5리 상엿집
                </svelte:fragment>
            </Image>
            <p class="article-text">
                전통 상례 시설인 상엿집은 마을의 공동재산으로 이용하고 관리를
                하였으나, 이제는 남아있는 사례를 찾아보기가 힘들어졌습니다.
                남아있는 상엿집 또한 전통 기법의 축조가 아닌 근대적 축조기법과
                골슬레이트 등의 재료를 이용한 것이 대부분이며, 이 마저도 점차
                사라질 위기에 처해있습니다.
            </p>
        </div>
        <div class="place-self-center">
            <Image chapterCode="1" imgCode="010-2" />
        </div>
    </div>
</section>
