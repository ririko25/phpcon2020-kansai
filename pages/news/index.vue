<template>
  <main>
    <div class="c-background">
      <Share />
      <p-news></p-news>
      <L-footer></L-footer>
    </div>
  </main>
</template>

<script>
import PNews from '~/components/News.vue'
import Share from "~/components/top/-Share.vue";
import LFooter from "~/components/Footer.vue";

export default {
  components: {
    PNews,
    LFooter,
    Share
  },
  head: {
      title: 'PHPカンファレンス関西2020 は 5月9日(土)に開催!',
      meta: [
        { property: 'og:title', content: 'PHPカンファレンス関西2020 は 5月9日(土)に開催!' },
        { property: 'og:image', content: 'https://2020.kphpug.jp/images/ogp.jpg' },
        { property: 'og:url', content: 'https://2020.kphpug.jp/' },
        { property: 'og:description', content: '集え、PHPer！！PHPerのGWはこの日が本番あのPHPの祭典がついに帰ってきた！今回のテーマは「Share!!」当日はPHPに関するトークセッションのほか、懇親会やその他イベントを実施予定「PHPカンファレンス関西」で知識•技術•感動をみんなで分かち合おう！' },
        { name: 'twitter:card', content: 'summary_large_image' },
        { name: 'description', content: '集え、PHPer！！PHPerのGWはこの日が本番あのPHPの祭典がついに帰ってきた！今回のテーマは「Share!!」当日はPHPに関するトークセッションのほか、懇親会やその他イベントを実施予定「PHPカンファレンス関西」で知識•技術•感動をみんなで分かち合おう！' }

      ]
    }
}
</script>

<style lang="scss" scoped>

@import "~/assets/scss/common.scss";

.c-background {

  &:before {
    content:"";
    width: 100vw;
    height: 100vh;
    background-image: url('~assets/images/hero/hero_sp_zou.png');
    background-repeat: no-repeat;
    background-size: 100%;
    display: block;
    position: fixed;
  }

    @include desktop(){
    &:before {
      background:none;
    }
}
}
</style>
