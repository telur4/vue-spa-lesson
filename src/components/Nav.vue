<template>
    <!-- ナビゲーションバー -->
    <nav class="navbar navbar-expand-md navbar-dark bg-dark sticky-top">
        <!-- サブコンポーネント -->
        <div class="container">
            <!-- ブランド -->
            <a href="" class="navbar-brand">Mr. M COFFEE</a>
            <!-- 切り替えボタン -->
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar-content" aria-controls="navbar-content" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <!-- ナビゲーション -->
            <div class="collapse navbar-collapse" id="navbar-content">
                <!-- ナビゲーションメニュー -->
                <!-- 左側メニュー：トップページの各コンテンツへのリンク -->
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item active">
                        <a href="" class="nav-link">
                            Top <span class="sr-only">(current)</span>
                        </a>
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
                    <!-- ドロップダウン -->
                    <li class="nav-item dropdown">
                        <a href="" class="nav-link dropdown-toggle" id="navbarropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Information</a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a href="" class="dropdown-item">Shop</a>
                            <a href="" class="dropdown-item">Access</a>
                        </div>
                    </li>
                </ul>
                <!-- 右側メニュー：Contactページへのリンク -->
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <!-- <a href="" class="nav-link btn btn-info">Contact</a> -->
                        <router-link to="/contact" class="nav-link btn btn-info">Contact</router-link>
                    </li>
                </ul>
                <!-- /ナビゲーションメニュー -->
            </div>
            <!-- /ナビゲーション -->
        </div>
        <!-- /サブコンポーネント -->
    </nav>
    <!-- /ナビゲーションバー -->
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Nav extends Vue {}
</script>