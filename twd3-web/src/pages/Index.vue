<template>
  <q-page>
    <div class="fit row wrap justify-center items-center content-center" style=" background:#3B3B3B;">
      <div class="col-auto">
      <img
      width="100%"
        alt="TwD3 logo"
        src="~assets/TwD3Logo.png"
      >
      </div>
    </div>
    <div class="row">
      <div class="q-px-lg q-pb-md col-md-4">
        <h3>TwD3とは</h3>
        <p>TwD3はTweetDeckの多重起動を検知するGoogleChrome拡張機能です。</p>
        <p>多重起動の検知だけでなく、TweetDeckの利用が便利になる機能が付属しています。</p>
      </div>
      <div class="q-px-lg q-pb-md col-md-4">
        <h3>できること</h3>
        <ul>
          <li>検知時自動ウィンドウ遷移</li>
          <ul>
            <li>自動で余計なウィンドウを閉じ、既に開かれているTweetDeckウィンドウへ遷移します。</li>
          </ul>
          <li>クイックアクセス</li>
          <ul>
            <li>アイコンを左クリックすることでTweetDeckへ素早くアクセスすることができます。</li>
          </ul>
          <li>TweetDeckブロックモード</li>
          <ul>
            <li>集中しなければならないときなど、TweetDeckを開きたくない場面でご利用ください。</li>
          </ul>
        </ul>
      </div>
      <div class="q-px-lg q-pb-md col-md-4">
        <h3>利用料金</h3>
        <p>TwD3は完全無料で提供しています。</p>
      </div>
    </div>

    <div class="row">
      <div class="q-px-lg q-pb-md col-md-6">
        <q-timeline color="secondary">
          <q-timeline-entry heading tag="h4">
            V1.2.x
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.2.3"
            subtitle="2020年11月18日"
          >
            <div>
              TwD3-Webリンクの追加
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.2.2"
            subtitle="2020年10月16日"
          >
            <div>
              他言語(En)対応のアップデート
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.2.1"
            subtitle="2020年9月19日"
          >
            <div>
              一つの小さな新機能と、一つのバグフィックス。
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.2"
            subtitle="2020年8月23日"
            icon="star"
            color="orange"
          >
            <div>
              TweetDeckブロックモードの追加。クイックアクセス関連のバグ修正。
            </div>
          </q-timeline-entry>

          <q-timeline-entry heading tag="h4">
            v1.1.x
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.1"
            subtitle="2020年4月14日"
          >
            <div>
              クイックアクセス機能が追加。
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Version 1.0"
            subtitle="2020年2月13日"
            icon="cake"
            color="orange"
          >
            <div>
              初期リリース。
            </div>
          </q-timeline-entry>
        </q-timeline>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>
