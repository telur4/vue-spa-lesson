<template>
    <!-- コンテンツ05 -->
    <div class="py-4">
        <section id="information">
            <div class="container">
                <h3 class="mb-3">Information</h3>
                <p>カフェ Mr. M COFFEE（ミスターエムコーヒー）は、○○県の○○市の山の中にあります。大自然に囲まれて、こだわりのコーヒーを飲みながら、美味しい空気と美しい景色をご堪能ください。</p>
                <div class="row">
                    <!-- 左側セクション -->
                    <div class="col-md-6">
                        <section id="shop">
                            <h4 class="mb-3">Shop</h4>
                            <!-- 店舗情報の表 -->
                            <table class="table table-hover">
                                        <TableBody
                                            v-bind:contents='[
                                                { name: "店名", about: "Mr. M COFFEE" },
                                                { name: "住所", about: "〒000-0000 ○○県○○市○○町1-2-3" },
                                                { name: "電話番号", about: "000-000-0000" },
                                                { name: "営業時間", about: "8:00〜18:00" },
                                                { name: "モーニング", about: "8:00〜11:00" },
                                                { name: "ランチタイム", about: "11:30〜14:00" },
                                                { name: "ラストオーダー", about: "17:30" },
                                                { name: "定休日", about: "水曜日、不定休" },
                                                { name: "クレジットカード", about: "利用不可" },
                                                { name: "禁煙席", about: "喫煙席あり" },
                                                { name: "駐車場", about: "駐車場あり" },
                                            ]'
                                        />
                            </table>
                            <!-- /店舗情報の表 -->
                        </section>
                    </div>
                    <!-- /左側セクション -->

                    <!-- 右側セクション -->
                    <div class="col-md-6">
                        <section id="access">
                            <h4 class="mb-3">Access</h4>
                            <!-- アクセスマップ -->
                            <div class="embed-responsive embed-responsive-4by3">
                                <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d3240.3328068554265!2d139.735574!3d35.693427!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188c5e412329bb%3A0x7db38e6732953dc!2z44CSMTYyLTA4NDYg5p2x5Lqs6YO95paw5a6_5Yy65biC6LC35bem5YaF55S677yS77yR4oiS77yR77yT!5e0!3m2!1sja!2sjp!4v1518974506558" frameBorder={0} width="800" height="600" style="border: 0" allowFullScreen />
                            </div>
                            <!-- /アクセスマップ -->
                            <p>○○駅から徒歩12分（950m）、駐車場あり</p>
                        </section>
                    </div>
                    <!-- /右側セクション -->
                </div>
            </div>
        </section>
    </div>
    <!-- /コンテンツ05 -->
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import TableBody from './Content/TableBody.vue';


@Component({
    components: {
        TableBody
    }
})
export default class Content5 extends Vue {}
</script>
