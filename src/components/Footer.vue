<template>
    <!-- フッター -->
    <footer class="py-4 bg-dark text-light">
        <div class="container text-center">
            <!-- ナビゲーション -->
            <ul class="nav justify-content-center mb-3">
                <li class="nav-item">
                    <a href="" class="nav-link">Top</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">News</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">About</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">Menu</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">Coupon</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">Information</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">Contact</a>
                </li>
            </ul>
            <!-- /ナビゲーション -->
            <button type="button" class="back-to-top">
                <span class="label">ページの先頭へ戻る</span>
            </button>
            <p>
                <small>Copyright ©2020 Mr. M COFFEE, All Rights Reserved.</small>
            </p>
        </div>
    </footer>
    <!-- /フッター -->
</template>

<script>
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Footer extends Vue {}
</script>
