<template>
    <!-- スライド -->
    <div class="carousel-item" v-bind:class="isActive()">
        <img v-bind:src="imgSrc" v-bind:alt="imgAlt" class="img-fluid">
        <div class="carousel-caption d-none d-md-block">
            <h2>{{ title }}</h2>
            <p>{{ text }}</p>
        </div>
    </div>
    <!-- /スライド -->
</template>

<script lang="ts">
import { Component, Emit, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Slide extends Vue {
    @Prop({ default: false })
    active!: boolean;

    @Prop({ default: '' })
    imgSrc!: string;

    @Prop({ default: '' })
    imgAlt!: string;

    @Prop({ default: '' })
    title!: string;

    @Prop({ default: '' })
    text!: string;

    @Emit('is-active')
    isActive() {
        return this.$props.active ? "active" : "";
    }

    mounted() {
        console.log(this.$props);
    }

    created() {
        console.log('This is Slide component.');
    }
}
</script>