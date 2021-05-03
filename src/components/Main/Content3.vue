<template>
    <!-- コンテンツ03 -->
    <div class="py-4">
        <section id="menu">
            <div class="container">
                <h3 class="mb-3">Menu</h3>
                <p>カフェ Mr. M COFFEEのメニューです。掲載していない季節限定メニューはMr. M COFFEEの<a href="">ブログ</a>にて紹介しています。</p>
                <!-- タブ型ナビゲーション -->
                <div class="nav nav-tabs" id="tab-menus" role="tablist">
                    <!-- タブ01 -->
                    <a href="#panel-menu01" class="nav-item nav-link active" id="tab-menu01" data-toggle="tab" role="tab" aria-controls="panel-menu01" aria-selected="true">コーヒー</a>
                    <!-- タブ02 -->
                    <a href="#panel-menu02" class="nav-item nav-link" id="tab-menu02" data-toggle="tab" role="tab" aria-controls="panel-menu01" aria-selected="true">モーニング</a>
                    <!-- タブ03 -->
                    <a href="#panel-menu03" class="nav-item nav-link" id="tab-menu03" data-toggle="tab" role="tab" aria-controls="panel-menu01" aria-selected="true">ランチ</a>
                    <!-- タブ04 -->
                    <a href="#panel-menu04" class="nav-item nav-link" id="tab-menu04" data-toggle="tab" role="tab" aria-controls="panel-menu01" aria-selected="true">ケーキ</a>
                </div>
                <!-- /タブ型ナビゲーション -->

                <!-- タブパネル -->
                <div class="tab-content" id="panel-menus">
                    <Panel
                        id="menu01"
                        title="COFFEE"
                        v-bind:active="true"
                        v-bind:contents='[
                            { name: "M ブレンド", price: 390 },
                            { name: "アイスコーヒー", price: 430 },
                            { name: "ブラジルシングル", price: 430 },
                            { name: "エスプレッソ", price: 300 },
                            { name: "カプチーノ", price: 430 },
                        ]'
                        img-src="./img/coffee.jpg"
                        img-alt="コーヒー"
                    />
                    <Panel
                        id="menu02"
                        title="MORNNING"
                        v-bind:active="false"
                        v-bind:contents='[
                            { name: "トーストセット", price: 450 },
                            { name: "トーストゆで卵セット", price: 500 },
                            { name: "フレンチトーストセット", price: 600 },
                            { name: "野菜たっぷりスープセット", price: 650 },
                        ]'
                        img-src="./img/morning.jpg"
                        img-alt="モーニング"
                    />
                    <Panel
                        id="menu03"
                        title="LUNCH"
                        v-bind:active="false"
                        v-bind:contents='[
                            { name: "ワンプレートランチ", price: 1000 },
                            { name: "Mixサンド", price: 650 },
                            { name: "ハンバーグサンド", price: 750 },
                            { name: "野菜たっぷりスープ", price: 650 },
                        ]'
                        img-src="./img/lunch.jpg"
                        img-alt="ランチ"
                    />
                    <Panel
                        id="menu04"
                        title="CAKE"
                        v-bind:active="false"
                        v-bind:contents='[
                            { name: "シフォンケーキ", price: 400 },
                            { name: "チーズケーキ", price: 350 },
                            { name: "本日のケーキ", price: 400 },
                            { name: "季節のパウンドケーキ", price: 400 },
                        ]'
                        img-src="./img/cake.jpg"
                        img-alt="ケーキ"
                    />
                </div>
                <!-- /タブパネル -->
            </div>
        </section>
    </div>
    <!-- /コンテンツ03 -->
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Panel from './Content/Panel.vue';

@Component({
    components: {
        Panel
    },
})
export default class Content3 extends Vue {}
</script>
