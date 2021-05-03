<template>
    <!-- カード -->
    <div class="col-md-4">
        <div class="card mb-3">
            <img v-bind:src="imgSrc" alt="" class="img-fluid" />
            <!-- カード本文エリア -->
            <div class="card-body d-flex justify-content-between">
                <h4 class="card-title">{{ cardTitle }}</h4>
                <button class="btn btn-secondary" type="button" data-toggle="modal" v-bind:data-target="dataTarget">
                    詳しく見る
                </button>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Card extends Vue {
    @Prop({ default: ''})
    imgSrc!: string;

    @Prop({ default: '' })
    cardTitle!: string;

    @Prop({ default: '' })
    dataTarget!: string;

    mounted() {
        console.log(this.$props);
    }
    
    created() {
        console.log('This is Card component.');
    }
}
</script>