<template>
    <!-- ヘッダー -->
    <header class="py-4">
        <div class="container text-center">
            <h1>
                <a href="">
                    <img src="@/assets/img/logo.png" alt="カフェ MR. M COFFEE" />
                </a>
            </h1>
        </div>
    </header>
    <!-- /ヘッダー -->
</template>


<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Header extends Vue {}
</script>
