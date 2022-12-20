<script>
    import { onMount } from "svelte";

    // Import Swiper styles
    import "swiper/css";
    import "swiper/css/pagination";
    import "swiper/css/navigation";
    import "swiper/css/effect-cards";
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
</script>

<Hero chapterCode="6" bgCode="068">
    <svelte:fragment slot="header">6부</svelte:fragment>
    <svelte:fragment slot="title">삼척 맹방리의 상례문화</svelte:fragment>
</Hero>

<section class="article-container fullscreen bg-dark text-white">
    <div class="article article-text g-0" style="gap:0">
        <h2 class="article-header">6-1. 강원도 사람들의 기억 속 상례문화</h2>
        <br>
        <hr />
        <br>
        <video
            src="https://d3pyyak0c50n14.cloudfront.net/sangyeotzip/chapter06-video.mp4"
            class="article-video"
            style="padding-block: 2.5ch"
            controls
            muted
            autoplay></video>
    </div>
</section>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2 order-md-1">
            <Image chapterCode="6" imgCode="064">
                <svelte:fragment slot="desc">
                    <a href="https://youtu.be/PNXf_ibPc7o?t=5730">
                        1996년 임권택 감독의 영화 “축제” 속 상여소리 장면
                    </a>
                </svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <h3 class="article-title">6-2. 영화 속의 상례</h3>
            <hr />
            <p class="article-desc">
                1996년 임권택 감독의 영화 “축제, 삶과 죽음 그리고 남은 이들의
                향연”은 상례를 죽은 이를 보내는 산 사람들의 축제로 표현한
                영화입니다. 한국 영화의 거장 임권택 감독의 작품으로 안성기,
                오정해 등이 출연한 작품입니다. 유튜브에서 무료로 보실 수 있으니
                시간 나실 때 감상해 보시기 바랍니다.
            </p>

            <p class="article-desc">
                <a href="https://www.kmdb.or.kr/db/kor/detail/movie/k/04830">
                    영화 내용 자세히 보기
                </a>
            </p>
            <p class="article-desc">
                줄거리: 40대 명망있는 작가 이준섭은 5년이 넘게 치매를 앓아온
                시골노모가 돌아가셨다는 연락을 받고 분주히 고향을 찾는다. 특히
                치매에 걸린 시어머니를 모셔온 형수의 감정은 홀가분과 애석함이
                교차한다. 한편, 준섭의 모친상을 통해 그의 문학세계를 재조명하는
                기사를 쓰러온 기자 장혜림은 관찰자로 장례식의 이모저모를
                취재하기 바쁘다. 장례가 시작되고, 가족 간의 갈등도 서서히
                풀리고, 할머니를 모시지 않은 작은 아버지 준섭을 원망하던 용순은
                준섭이 쓴 동화를 읽고 눈물을 흘린다. 장례가 끝나자 노모가 남겨준
                큰 사랑과 삶의 지혜를 가족들은 각자 가슴 속에 간직하게 된다.
                (출처 : 한국영상자료원, 한국영화데이터베이스)
            </p>
        </div>
    </div>
</section>

<div class="chapter03-sub" style="background-color: #212529; color: white">
    <Subhero chapterCode="6" imgCode="065">
        <svelte:fragment slot="header"
            >6-3. 삼척 맹방리의 상장례 문화</svelte:fragment>

        <svelte:fragment slot="desc">
            국립민속박물관 상엿집 조사팀에서는 매방리 상엿집 뿐만 아니라
            맹방리의 상장례 문화에 대해서도 조사하였습니다. 맹방리에서는 상여와
            상엿집에 대한 기억을 가진 어르신들이 점차 사라지고 있었는데,
            마을에서 1974년부터 이장을 오래 역임하신 홍영택씨(1938년생)의 구술과
            사진자료들로 맹방리의 상장례 문화를 조금이나마 조명할 수 있게
            되었습니다.
        </svelte:fragment>
        <svelte:fragment slot="imgDesc"
            >맹방리 상장례에 대해서 구술 중인 홍영택씨</svelte:fragment>
    </Subhero>
</div>

<section class="article-container">
    <div class="article grid-2">
        <div class="order-2 order-md-1 place-self-center">
            <Image chapterCode="6" imgCode="066">
                <svelte:fragment slot="desc">
                    맹방리 마을의 논밭
                </svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <p class="article-desc p-md-0 order-1 order-md-2">
                강원도 삼척시 맹방리는 아름다운 맹방해변 옆에 위치한 마을입니다.
                현재 총 50여 가구가 거주하고 있으며 주요 성씨는 평택 임씨, 순흥
                안씨라고 하는데 현재는 외지인들이 많이 들어와서 사는 각성받이
                마을입니다.
            </p>
            <p class="article-desc p-md-0 order-1 order-md-2">
                맹방리는 바다에 접하고 있으나 어업에 종사하는 사람은 없고
                논농사와 밭농사 주요 생업인 전형적인 농촌입니다. 주요 작물은 쌀,
                보리, 좁쌀 등이라고 합니다. 맹방리 사람들은 예부터 고기잡이를
                하지 않고 농사를 짓는 것을 자랑스럽게 생각하였다고
                합니다.(농민은 어민을 다소 낮게 보는 경향이 다소 있음.)
            </p>
        </div>
    </div>
</section>

<section class="article-container pt-0">
    <div class="article grid-2">
        <div class="order-2">
            <Image chapterCode="6" imgCode="067">
                <svelte:fragment slot="desc">맹방해수욕장</svelte:fragment>
            </Image>
        </div>
        <p class="article-text p-md-0">
            맹방리는 아름다운 바다를 접하고 있어서 1970년대부터 민박업도 많이
            했다고 합니다.(최근 BTS의 사진 촬영지로 유명세를 치르기도
            하였습니다.)
        </p>
    </div>
</section>

<section class="article-container pt-0">
    <div class="article grid-2">
        <div class="order-2 order-md-1 place-self-center">
            <Image chapterCode="6" imgCode="068">
                <svelte:fragment slot="desc">맹방리 성황당</svelte:fragment>
            </Image>
        </div>
        <div class="article-text p-md-0 order-1 order-md-2">
            <p class="article-text p-md-0 order-1 order-md-2">
                마을제사는 현재도 계속 지내고 있으며 정월 초사흘에 빠지지 않고
                마을 입구의 성황당에서 지내고 있습니다.
            </p>
        </div>
    </div>
</section>

<section class="article-container pt-0">
    <div class="article">
        <div class="chapter-6-grid">
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="069">
                    <svelte:fragment slot="desc">맹방리 성황당</svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(1) 장례기간</h3>
                    <hr />
                    <p class="article-desc">
                        현재는 3일장이 대부분이지만 옛날 맹방리에서는 경제적으로
                        여유가 있는 집은 15일, 일반적으로는 5일~9일이었다고
                        합니다. 장례기간이 길었던 이유는 장례를 치르기 위한
                        준비를 상주 혹은 마을사람들이 모두 해야 했었고, 교통과
                        통신의 미비로 조문을 하는데도 시간이 더 걸렸기
                        때문이라고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="070">
                    <svelte:fragment slot="desc">
                        1978년 부고장. 조재기의 부친 조철원의 사망을 알리는
                        문서.
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">
                        (2) 부고(訃告), 상(喪)을 알리다.
                    </h3>
                    <hr />
                    <p class="article-desc">
                        상을 당하면 먼저 부고를 하는데 가까운 곳에는 사람이 가서
                        직접 알리고, 멀리 있는 분들에게는 편지나 전보로 알리기도
                        했습니다. 1960년대 마을에는 우체국에서 사용하는 마을
                        공용 전화기가 1대 있었다고 합니다. 전화가 보편화된
                        이후로는 멀리 있는 사람들에게도 부고를 알리기 편해졌다고
                        합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="071">
                    <svelte:fragment slot="desc">
                        1978년 부고장. 조재기의 부친 조철원의 사망을 알리는
                        문서.
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(3) 음식과 술</h3>
                    <hr />
                    <p class="article-desc">
                        상례 음식은 당시 가난한 농촌 사정상 된장 미역국, 무나물,
                        채소나물이 일반적이었다고 한다. 형편이 조금 나은 집들은
                        돼지나 소를 잡아서 손님 대접을 했다고 합니다. 상례에
                        가장 중요한 것은 막걸리였다고 합니다. 당시만 해도 집에서
                        직접 막걸리를 만들어서 조문객을 대접했다고 합니다.
                        근덕에 양조장이 들어선 후에는 말통으로 20통 정도
                        주문해서 상을 치뤘다고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="072">
                    <svelte:fragment slot="desc">
                        조문을 받는 상주
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(4) 조문(弔問)과 만장(挽章)</h3>
                    <hr />
                    <p class="article-desc">
                        조문을 온 사람들은 종이나 면포에 고인을 추모하는 글인
                        만장(挽章)을 지참하였고, 조문품으로는 양초, 종이, 명주,
                        막걸리, 계란 등 장례에 필요한 물품을 주로 건냈다고
                        합니다. 상주는 조문객이 오면 곡을 합니다. 조문객은
                        빈소에 절을 올리고 상주와 맞절을 합니다. 상주가 내오는
                        술과 음식을 나누며 밤을 새웁니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="073">
                    <svelte:fragment slot="desc">
                        깃대에 걸린 만장. 상여보다 먼저 간다.
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <p class="article-desc">
                        만장(挽章)은 죽은 이를 추모하는 글입니다. 여유가 있는
                        사람들은 천에 만장을 쓰고, 그렇지 못한 사람들은 한지에
                        만장을 썼다고 합니다. 상가에서 받은 만장이 너무 많은
                        경우에는 상가집에 새끼 줄을 메어서 만장을 길게 이어서
                        붙였다고 합니다. 상여가 나갈 때는 만장을 깃대에 걸어서
                        상여보다 먼저 가게 하고, 묘지에 도착한 후에는 불에
                        태웠습니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="074">
                    <svelte:fragment slot="desc">
                        깃대에 걸린 만장. 상여보다 먼저 간다.
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">
                        (5) 상복(喪服), 수의(壽衣), 관(棺) 준비
                    </h3>
                    <hr />
                    <p class="article-desc">
                        상복은 형편이 좋은 사람들은 광목으로 만든 상복을 입었고,
                        형편이 어려운 사람들은 그냥 평상복을 입었다고 합니다.
                        후대에는 양복을 입었습니다. 수의(壽衣)는 집에 보관하던
                        삼베로 직접 집에서 만들어서 고인에게 입혔다고 합니다.
                        관은 마을의 목수를 통해서 짰다고 합니다. 고인이 사망하면
                        목수가 와서 치수를 재서 관을 짜는데 길이는 6자 정도이고
                        넓이는 1.5~2자 정도가 일반적이었다고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="075">
                    <svelte:fragment slot="desc">
                        고사계가 설치한 차양과 가리개
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(6) 마을의 장례조직, 고사계</h3>
                    <hr />
                    <p class="article-desc">
                        마을에 초상이 나면 고사계가 먼저 초상이 난 집에 삼베로
                        차양(챙)을 만들고 마당에는 멍석을 깔아서 조문객을 맞이할
                        준비를 합니다. 고사계에서는 장례용품, 장례용 천막,
                        돗자리, 깔판, 상, 목기 등 마을에서 공동으로 사용하는
                        장례 용품들을 가지고 옵니다. 상은 소반같은 형태의
                        1~2인용 상이었고, 목기는 대접같은 형태가 많이
                        사용되었다고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="076">
                    <svelte:fragment slot="desc">
                        고인을 염(殮)하고 관에 모신다.
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">
                        (7) 염(殮), 고인을 깨끗하게 하고 수의를 입히다.
                    </h3>
                    <hr />
                    <p class="article-desc">
                        염(殮)이란 시신을 깨끗하게 닦아드리고 수의로 갈아입힌 후
                        베나 이불 따위로 싸는 장례 과정입니다. 오늘날에는
                        장의사가 전문적으로 염을 하지만 과거에는 마을 사람들이나
                        친척 중 염을 할 줄 아는 사람이 대신하였다고 합니다. 먼저
                        시신을 향물이나 쑥물을 섞어 깨끗이 닦고, 손발톱을 깍아서
                        조발주머니에 넣습니다. 상주가 정성스럽게 준비한 수의로
                        갈아 입힙니다.
                    </p>
                    <h3 class="article-title">
                        (8) 입관(入棺), 고인을 관에 모시다.
                    </h3>
                    <hr />
                    <p class="article-desc">
                        염(殮)이 끝나면 바로 고인을 관에 모십니다. 관에 칠성판을
                        먼저 넣고 그 위에 고인을 모십니다. 가까운 친지 외에는
                        입관을 보는 것이 험하다고 하여 대부분 사람들은 피한다고
                        합니다. 관은 서늘한 곳에 모시는데, 여름철에는 특히
                        시신이 부패되는 경우가 있어서, 관 밑에 시신에서 나오는
                        체액이 흐르는 경우도 있었다고 합니다. 대청 마루 아래에
                        땅을 파서 최대한 서늘하게 시신을 보관하거나 마당에
                        임시로 관을 매장해서 보관하기도 하였다고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="077">
                    <svelte:fragment slot="desc">
                        상여에 관을 올리는 상여꾼들
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(9) 상여계와 상여꾼</h3>
                    <hr />
                    <p class="article-desc">
                        상여계는 상여를 운반하고 준비하는 마을의 조직입니다.
                        상여꾼은 마을 주민들이 돌아가면서 했는데 이장의 권한으로
                        선발했다고 합니다. 대체로 경제적으로 여유가 있는
                        사람들은 20명 정도의 상여꾼을 썼고 여유가 없는 사람은
                        10명 정도만 썼다고 합니다. 상여꾼들에게는 식사와 담배가
                        제공되었으며, 상여가 원만하게 갈 수 있도록 상주가 계속
                        음식과 술을 제공하였다고 합니다. 상여를 메는 줄을
                        접줄이라 하는데 좌우로 2개 있어 양쪽으로 나뉘어서 상여를
                        멥니다. 광목 천으로 만든 상여줄도 버리지 않고 상여꾼들이
                        나누어 가졌다고 합니다. 상여줄로는 대개 속옷 등을
                        만들었다고 합니다.
                    </p>
                    <p class="article-desc">
                        상여꾼 중에서 술을 잘 마시고 장난을 잘 치는 사람들을
                        왈패라고 합니다. 대개 상여를 멘 줄 앞쪽에 있는 왈패꾼을
                        앞코잽이라고 하고 뒤쪽에 있는 왈패꾼은 뒷코잽이라고
                        부릅니다. 왈패꾼은 상여꾼 중 경험이 많은 사람들이 맡아서
                        합니다. 상여 운반 중에 농을 부리고 장난을 치는 행위는
                        힘든 상여 운반일에 활력을 주기도 하고, 상주들의 슬픔을
                        달래는 효과도 있다고 합니다. 왈패꾼들은 상주들에게 술과
                        음식을 요구하기도 하고 적당하게 투정을 부리기도 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="078">
                    <svelte:fragment slot="desc">상여행렬</svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(10) 상여소리</h3>
                    <hr />
                    <p class="article-desc">
                        마을에는 상여소리를 하는 소리꾼이 있었는데 현재는
                        작고하셔서 전승이 끊긴 상태라고 합니다. 상여소리에서
                        가장 중요한 것은 요량(방울)이라는 손방울입니다. 요량을
                        든 사람이 상여에 올라타고 상여소리를 선도합니다.
                        상여소리의 내용은 “사람의 인생이 허무하고, 저승에 가셔서
                        극락왕생하라는 바람” 등이라고 합니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="079">
                    <svelte:fragment slot="desc">
                        꽃으로 장식된 상여
                    </svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(11) 상여장식</h3>
                    <hr />
                    <p class="article-desc">
                        경제적으로 여유있는 사람은 빨간색 꽃으로 상여를
                        장식하였습니다. 맹방리에서는 두꺼운 종이로 만든 닭모양
                        장식인 장닭이라는 상여 장식이 있었습니다. 나무로 만든
                        상여 장식은 봉황이었는데, 맹방리에서 닭 모양으로
                        만들었다고 합니다.
                    </p>
                    <h3 class="article-title">(12) 상여가 나가다.</h3>
                    <hr />
                    <p class="article-desc">
                        상여가 나갈 때는 고인의 집 마당을 왔다 갔다 하며 먼저
                        돕니다. 상주들은 고인을 아쉬워하면서 상여가 가지 못하게
                        막아서며 슬프게 곡을 합니다. 상주들은 고인의 극락왕생을
                        빌며 노잣돈을 상여가 가는 길에 놓습니다. 상여행렬은
                        만장, 요여, 상여순으로 갑니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="081">
                    <svelte:fragment slot="desc">발인제</svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(13) 발인제(發靷祭)</h3>
                    <hr />
                    <p class="article-desc">
                        상여가 고인의 집에서 나가면 넓은 장소에 상여를 모시고
                        발인제를 지냅니다. 발인제는 멍석이나 돗자리를 깔고
                        음식을 상여 앞에 진설한 후에 상주를 비롯한 사람들이
                        고인에게 술을 올리고 절을 하는 제사입니다. 발인제가
                        진행되는 중에도 상여꾼들은 상여 소리를 하면서 분위기를
                        고조시킵니다.
                    </p>
                </div>
            </div>
            <div class="chapter-6-grid-item">
                <Image chapterCode="6" imgCode="082">
                    <svelte:fragment slot="desc">노제</svelte:fragment>
                </Image>
                <div class="article-text p-md-0">
                    <h3 class="article-title">(14) 노제(路祭)</h3>
                    <hr />
                    <p class="article-desc">
                        상여가 장지로 가는 길에는 여러 차례 노제를 올립니다.
                        노제를 지내는 회수는 정해진 것이 없으나 대개 잘 사는
                        사람들은 3~4번 정도 노제를 올렸다고 합니다. 노제를 지낼
                        때마다 고인의 저승길에 필요한 노잣돈을 올리는데 여기에
                        사용된 돈들은 대개 상여꾼들을 대접하는데 쓰입니다. 노제
                        때에는 친지나 마을사람들이 미리 준비한 추도사를 읽기도
                        합니다.
                    </p>
                    <h3 class="article-title">
                        (15) 매장(埋葬), 고인을 산에 모시다.
                    </h3>
                    <hr />
                    <p class="article-desc">
                        상여가 산에 도착하면 상여를 내려놓고 다시 제사를
                        올립니다. 상주들은 구슬프게 곡을 하고 고인에게 절을
                        올립니다. 제사가 끝나면 상여꾼들은 고인을 매장하고
                        봉분을 만들고 잔디를 덮습니다. 이것으로 모든 장례 절차는
                        끝이 납니다.
                    </p>
                </div>
            </div>
        </div>
    </div>
</section>
