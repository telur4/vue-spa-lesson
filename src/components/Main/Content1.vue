<template>
    <!-- コンテンツ01 -->
    <div class="py-4">
        <section id="news">
            <div class="container">
                <div class="row">
                    <!-- 左側カラム（画面幅md以上） -->
                    <div class="col-md-2">
                        <h3>News</h3>
                    </div>

                    <!-- 右側カラム（画面幅md以上） -->
                    <div class="col-md-10">
                        <dl class="row">
                            <dt class="col-md-3">2020年○月○日</dt>
                            <dd class="col-md-9">ランチクーポン配布中です</dd>
                            <dt class="col-md-3">2020年○月○日</dt>
                            <dd class="col-md-9">季節限定メニューを追加しました</dd>
                            <dt class="col-md-3">2020年○月○日</dt>
                            <dd class="col-md-9">新しい雑貨さん入荷しました</dd>
                        </dl>
                    </div>
                </div>
            </div>
        </section>
    </div>
    <!-- /コンテンツ01 -->
</template>

<script>
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Content1 extends Vue {}
</script>
