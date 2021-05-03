<template>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb">
            <li class="breadcrumb-item">
                <a href="">Top</a>
            </li>
            <li class="breadcrumb-item active" aria-current="page">Contact</li>
        </ol>
    </nav>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Breadcrumb extends Vue {}
</script>