<script lang="ts">
  import { page } from '$app/stores';
  import { derived } from 'svelte/store';

  const id = derived(
    page,
    ($page) => $page.url.pathname.split('/').slice(-1)[0],
  );
</script>

{#if $id === '1'}
  <section>
    <span class="name"><img src="/arrow.png" alt="" height="15px"/> Mind+ing, 팩토리 2</span>
    <div class="container">
      <div class="title">
        <img src="/factory/0.jpg" alt="" />
      </div>
      <div class="description">
        <span>
          {'<mind+ing>는 이호경, 정수연의 개인적 경험에서 파생된 ‘마음’에서 시작하여 각자만의 유의미한 매체로 표현해나가는 여정을 보여주고자 한다. 이 전시는 두 작가 본인의 주의를 기울인다는 의미에서의 마인딩과 개인적 감정을 다루며 마음을 돌본다는 뜻의 이중적 의미를 담는다. 본 전시는 작가만의 경험을 기반으로 느꼈던 감정들을 끄집어내며 이를 각자의 조형언어로 새로이 시각화하고 minding의 연장선에 서고자 한다.'}</span
        >
        <span
          >이호경은 열심히 쌓아 만든 모래성이 파도에 의해 무너지는 모습을 관찰한
          후, 정처없이 밀려가고 떠밀려오는 상황 앞에 놓인 유동적 성질을 가진
          모래알들을 바라보게 된다. 파도 한 번에 무너져 내리는 연약한
          텍스쳐(texture)를 지닌 개체로 본인을 인식하며 모래알에 자신을
          투영한다. 그 후 불확실성이 담긴 파도의 소리를 채집하고 당시 느낀
          심상을 가시화한다. 모래 알갱이로 만들어진 바탕 위에 시각화된 소리의
          이미지들을 얹고 쓸려 나가는 모습을 담으며 이로써 당시 경험했던 자연에
          대한 감각을 환기한다.
        </span>
        <span>
          정수연은 다양한 기억의 층들을 접하며 기억의 연장선에 서 있게 되고, 더
          나아가 진정한 교감을 이루게 한 식물과의 기억을 시작으로 이상적인 정원
          만들기를 시도한다. 변함없이 분화된 형태, 지속성을 통해 유토피아를
          구현하고자 한다. 유토피아 정원은 완전하다고 인지되는 의도적인 형태,
          색감과 허구적으로 묘사된 상상의 식물 등 종의 다양성을 함의하며,
          근원적으로는 식물과 상상의 나래를 펼쳤던 어린 시절의 자아와 연결하는
          시작점으로서 작동하고자 한다.
        </span>
      </div>
      <div class="image-container">
        <img src="/factory/1.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/factory/2.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/factory/3.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/factory/4.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/factory/5.jpg" alt="" />
      </div>
    </div>
  </section>
{/if}
{#if $id === '2'}
  <section>
    <span class="name"
      ><img src="/arrow.png" alt="" height="15px"/> 나는 아주 사소한 것까지도 볼 수 있었다: I Could See the Smallest
      Things, 우석갤러리</span
    >
    <div class="container">
      <div class="title">
        <img src="/woosuk/0.jpg" alt="" />
      </div>
      <div class="description">
        <span>
          {'앰퍼샌드는 and(그리고)를 의미하는 기호로, 일상에서 흔하게 사용하는 부호다. 이름보다 형태로 익숙한 이 기호는 무언가 연결되고 지속될 것 같은 공통된 이미지를 연상시킨다. 전시 <앰퍼샌드>는 ‘&’ 처럼 ‘시각 작업이 보편적 인식을 바탕으로 관객에게 다가갈 수 있을까’라는 질문으로부터 시작했다.'}</span
        >
        <span>
          {`"모든 것이 달빛 아래에 드러나 있었고, 나는 아주 사소한 것까지도 볼 수 있었다." 미국 단편소설의 대가 레이먼드 카버(Raymond Carver, 1938~1988)의 <사랑을 말할 때 우리가 이야기 하는 것 (What We Talk about Love)> 중 단편
'나는 아주 사소한 것까지도 볼 수 있었다'에 등장하는 구절이다. '나는 아주 사소한 것까지도 볼 수 있었다 .(I Could See the Smallest Things.)' 속 여자는 한밤중 열린 대문 바깥으로 나갈 생각 않고 잠에 들 지 못한다. 의혹, 소문 등으로부터 거대해진 걱정을 안은 채 말이다. 이 여자의 모습은, 어쩌면 현 시대를 살아가는 우리의 그늘 과도 같을지 모른다.`}
        </span>
      </div>
      <div class="image-container">
        <img src="/woosuk/1.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/woosuk/2.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/woosuk/3.jpg" alt="" />
      </div>
    </div>
  </section>
{/if}
{#if $id === '3'}
  <section>
    <span class="name"
        ><img src="/arrow.png" alt="" height="15px"/> what-多got-多, 서울시청 시민청 갤러리</span
      >
    <div class="container">
      <div class="title">
        <img src="/citizen/0.jpg" alt="" />
      </div>
      <div class="description">
        <span>
          관람객이 전시장 문을 연 순간부터 작품의 비가시적인 영역에 도달하기
          까지 소요되는 시간에 대해 생각해본 적이 있다. 근본적으로는 도달
          가능성에 관한 의구심인데, 이미지 범람의 시대에 관람객에게 회화가
          단순히 또 하나의 이미지로 간주되어 제한적 기능을 하게 되는 것은 아닐까
          하는 불안에서 비롯된 기우다.‘왔다갔다’는 지그재그 모양을 표현한
          의태어로, 불안정한 모양의 시각적 효과를 통해 차량의 감속을 유도하기
          위한 도로 위 지그재그 차선 모양에서부터 출발했다. 완성된 작업을 전면에
          내세우는 일반적인 전시 구성을 탈피하고 작품의 표면과 이면을 넘나들 수
          있는 전시를 시도하며 작가와 관람객이 함께 환유할 수 있는 경계에 질문을
          던진다.
        </span>
        <span
          >{'‘시민청’이라는 공간의 특성에 맞추어 기획한 전시 《What-多 got-多》는 동양 매체를 기반으로 활동하는 여성 신인작가 김나현, 류은선, 이호경, 정수연, 청이인 총 5인이 한지라는 공통된 바탕재 위에 각기 다른 재료와 기법을 사용한 작품을 선보이는 자리이다. 동시에 작품 이면을 조명함으로써 회화, 그중에서도 현재 동양화로 분류될 수 있는 작품에 대한 대중적 접근성을 높인다. 재료와 기법에 대한 이해가 회화의 형식적 측면으로의 접근에 도움이 될 것이라 보고, 재료 설명과 작업과정을 담은 영상, QR코드를 통한 음성해설, 작품에 사용된 도구 등을 완성된 작품과 함께 배치한다. 이는 불특정 다수의 관람객이 전시를 감상할 때 캡션과 핸드아웃만으로는 형식적 측면에 대한 이해가 어렵다는 점을 극복하기 위한 시도다. 관람객이 작품 내부로 들어올 수 있도록 보다 친근하게 길을 열어주고, 자체적으로는 동양화의 발전 가능성을 탐색하고자한다.'}
        </span>
      </div>
      <div class="image-container">
        <img src="/citizen/1.jpg" alt="" />
      </div>
      <div class="image-container">
        <img src="/citizen/2.jpg" alt="" />
      </div>
    </div>
  </section>
{/if}

<style>
  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }
  section {
    margin-left: 40px;
    margin-right: 40px;
    margin-bottom: 80px;
  }
  .description span {
    display: block;
    margin-bottom: 20px;
    color: #6a6a6a;
    font-size: 22px;
  }
  .description {
    width: 1000px;
  }
  .title {
    display: flex;
    flex-direction: column;
    align-items: start;
    margin-bottom: 40px;
  }
  .title img {
    border: 1px solid #000;
  }
  .image-container {
    margin-top: 40px;
  }
  .container {
    margin-top: 10px;
  }
</style>
