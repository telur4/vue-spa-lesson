<template>
    <!-- メインビジュアル -->
    <div class="py-4">
        <div class="container">
            <!-- カルーセル外枠 -->
            <div id="main_visual" class="carousel slide" data-ride="carousel">

                <!-- インジケーター -->
                <ol class="carousel-indicators">
                    <li data-target="#main_visual" data-slide-to="0" class="active" />
                    <li data-target="#main_visual" data-slide-to="1" />
                    <li data-target="#main_visual" data-slide-to="2" />
                </ol>
                <!-- /インジケーター -->

                <!-- カルーセル内枠 -->
                <div class="carousel-inner">
                    <Slide
                        v-bind:active="true"
                        img-src="./img/slide_01.jpg"
                        img-alt="コーヒー写真"
                        title="Mr. M COFFEEのこだわり"
                        text="店主が世界中のコーヒー豆を厳選し、コーヒー豆の種類に合わせ、心を込めて焙煎、抽出しております。"
                    />
                    <Slide
                        v-bind:active="false"
                        img-src="./img/slide_02.jpg"
                        img-alt="ランチ写真"
                        title="Mr. M COFFEEのメニュー"
                        text="コーヒーはもちろん、モーニングやワンプレートランチ、季節のスイーツなどもご好評いただいております。"
                    />
                    <Slide
                        v-bind:active="false"
                        img-src="./img/slide_03.jpg"
                        img-alt="店内写真"
                        title="Mr. M COFFEEの空間"
                        text="座り心地の良いソファと丁度良い高さのテーブル。くつろぎの空間を満喫してください。"
                    />
                </div>
                <!-- /カルーセル内枠 -->

                <!-- コントローラー -->
                <a href="#main_visual" class="carousel-control-prev" role="button" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true" />
                    <span class="sr-only">前に戻る</span>
                </a>
                <a href="#main_visual" class="carousel-control-next" role="button" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true" />
                    <span class="sr-only">次に進む</span>
                </a>
                <!-- /コントローラー -->
            </div>
            <!-- /カルーセル外枠 -->
        </div>
    </div>
    <!-- /メインビジュアル -->
</template>

<script>
import { Component, Vue } from 'vue-property-decorator';
import Slide from './Content/Slide.vue';

@Component({
    components: {
        Slide
    },
})
export default class MainVisual extends Vue {}
</script>
