<script lang="ts">
  import { page } from '$app/stores';
  import { derived } from 'svelte/store';

  const year = derived(
    page,
    ($page) => $page.url.pathname.split('/').slice(-1)[0],
  );
</script>

{#if $year === '2020'}
  <div class="row-in-row">
    <figure>
      <img src="/2020/1.png" alt="" />
      <figcaption>
        설국 , 00:02:00, 단채널영상, 2020
      </figcaption>
    </figure>
  </div>
  <div class="row-in-row">
    <figure>
      <img src="/2020/2.png" alt="" />
      <figcaption>
        running meditation, 00:02:00, 단채널영상, 2020      </figcaption>
    </figure>
  </div>
{/if}
{#if $year === '2021'}
  <div class="row">
    <figure>
      <img src="/2021/1.png" alt="" />
      <figcaption>myiodesopsia, 00:15:36, 단채널영상, 2021</figcaption>
    </figure>
  </div>
  <div class="row-in-row">
    <figure>
      <img src="/2021/2.png" alt="" />
      <figcaption>accumulation, 00:02:06, 단채널영상, 2021</figcaption>
    </figure>
  </div>
  <div class="row-in-row">
    <figure>
      <img src="/2021/3.png" alt="" />
      <figcaption>
        N.O.S(not otherwise specified), 00:02:19, 단채널영상, 2021
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2021/4.png" alt="" />
      <figcaption>서울대학교 74동 전시전경, 2021</figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2021/5.jpg" alt="" />
      <figcaption>myiodesopsia 2, 00:03:00, 단채널영상, 2021</figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2021/6.jpg" alt="" />
      <figcaption>
        알 수 없는 검음(Unknown Black), 순지에 수묵,390.9x160.2cm, 2021
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2021/7.jpg" alt="" />
      <figcaption>
        투명토록 허무해서(Transparent in Vain), 순지에 수묵,387.8x130.3cm, 2021
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2021/8.jpg" alt="" />
      <figcaption>
        덮쳐오는 일렁임에(because of the swaying), 순지에 수묵,387.8x130.3cm,
        2021
      </figcaption>
    </figure>
  </div>
{/if}
{#if $year === '2023'}
  <div class="row">
    <figure>
      <img src="/2023/1.jpg" alt="" />
      <figcaption>
        The passage of time according to the difference between tides, 장지에
        석회와 모래알갱이, 97x130.3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/2.jpg" alt="" />
      <figcaption>
        Vulnerability testing(3pcs), 장지에 석회와 모래알갱이, 각 30x30cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/3.jpg" alt="" />
      <figcaption>
        am 8:00 주문진 앞에서, 장지에 석회와 모래알갱이, 각 34.8x27.3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/4.jpg" alt="" />
      <figcaption>
        연약한 텍스쳐(texture)(2pcs), 장지에 석회와 모래알갱이, 각 54.5x54.67cm,
        2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/5.jpg" alt="" />
      <figcaption>파도 소리 연구, 순지에 수묵, 18x141x4cm, 2023</figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/6.jpg" alt="" />
      <figcaption>
        building sand castles, 장지에 석회와 모래알갱이, 70x75cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row-in-row">
    <figure>
      <img src="/2023/7.jpg" alt="" />
      <figcaption>
        간조(干潮) , 장지에 석회와 모래알갱이, 130.3x97cm, 2023
      </figcaption>
    </figure>
    <figure>
      <img src="/2023/8.jpg" alt="" />
      <figcaption>
        만조(滿潮) , 장지에 석회와 모래알갱이, 130.3x97cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/9.jpg" alt="" />
      <figcaption>
        밤바다(the night sea), 장지에 석회와 모래알갱이,162.2x130.3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/10.jpg" alt="" />
      <figcaption>
        under the waves, 장지에 석회와 모래알갱이, 162.2x130.3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/11.jpg" alt="" />
      <figcaption>
        after the waves, 장지에 석회와 모래알갱이, 162.2x130.3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/12.jpg" alt="" />
      <figcaption>
        a trace of a waver, 장지에 석회와 모래알갱이, 54x160x3cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/13.jpg" alt="" />
      <figcaption>
        the time of the waves, 장지에 석회와 모래알갱이, 20x204cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/14.jpg" alt="" />
      <figcaption>
        연약한 텍스쳐(texture)1, 장지에 석회와 모래알갱이, 54.5x54.67cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/15.png" alt="" />
      <figcaption>
        연약한 텍스쳐(texture) 2, 장지에 석회와 모래알갱이, 54.5x54.67cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/16.jpg" alt="" />
      <figcaption>
        a pebble stone1, 장지에 석회와 모래알갱이, 39.77x72.52cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/17.jpg" alt="" />
      <figcaption>
        a pebble stone2, 장지에 석회와 모래알갱이, 55.5x29.46cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/18.jpg" alt="" />
      <figcaption>
        a pebble stone3, 장지에 석회와 모래알갱이, 60.52x50.43cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/19.jpg" alt="" />
      <figcaption>
        a pebble stone4, 장지에 석회와 모래알갱이, 60.32x48.58cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/20.jpg" alt="" />
      <figcaption>
        a grain of black sand 1, 장지에 석회와 모래알갱이,156x115cm, 2023
      </figcaption>
    </figure>
  </div>
  <div class="row">
    <figure>
      <img src="/2023/21.jpg" alt="" />
      <figcaption>
        a grain of black sand 2, 장지에 석회와 모래알갱이, 117x173cm, 2023
      </figcaption>
    </figure>
  </div>
{/if}

<style>
  .row {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: end;
    margin-bottom: 50px;
    margin-left: 30px;
    margin-right: 30px;
  }
  .row-in-row {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: end;
    margin-bottom: 50px;
    margin-left: 30px;
    margin-right: 30px;
  }
  figcaption {
    font-style: normal;
    font-weight: 400;
    line-height: 17px;
    color: #6a6a6a;
    font-size: 12px;
    text-overflow: ellipsis;
    text-align: end;
  }
</style>
