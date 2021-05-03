<template>
    <div>
        <MainVisual></MainVisual>
        <Content1></Content1>
        <Content2></Content2>
        <Content3></Content3>
        <Content4></Content4>
        <Content5></Content5>
    </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import MainVisual from './Main/MainVisual.vue';
import Content1 from './Main/Content1.vue';
import Content2 from './Main/Content2.vue';
import Content3 from './Main/Content3.vue';
import Content4 from './Main/Content4.vue';
import Content5 from './Main/Content5.vue';

@Component({
    components: {
        MainVisual,
        Content1,
        Content2,
        Content3,
        Content4,
        Content5
    }
})
export default class HomeMain extends Vue {}
</script>