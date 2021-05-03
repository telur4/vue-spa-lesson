<template>
    <!-- コンテンツ04 -->
    <div class="py-4 bg-light">
        <section id="coupon">
            <div class="container">
                <h3 class="text-center mb-3">Coupon</h3>
                <!-- カード -->
                <div class="card text-center text-dark w-75 mx-auto">
                    <div class="card-header bg-success text-while">
                        Mr. M COFFEEランチクーポン
                    </div>
                    <div class="card-body">
                        <h5 class="card-title">食後のコーヒープラス100円にてご提供</h5>
                        <p class="card-text text-justify">ワンプレートランチ（限定数20食）ご注文のお客様に、プラス100円で食後のコーヒーをご提供。お会計の際に、このクーポン画面をスタッフに見せてください。</p>
                    </div>
                    <div class="card-footer bg-success text-white">
                        クーポンコード：HAPPYLUNCH
                    </div>
                </div>
                <!-- /カード -->
            </div>
        </section>
    </div>
    <!-- /コンテンツ04 -->
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Content4 extends Vue {}
</script>
