<template>
    <!-- モーダル -->
    <div class="modal fade" v-bind:id="id" tabIndex="-1" role="dialog" aria-labelledby="id + '-label'" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" v-bind:id="id + '-label'">{{ title }}</h5>
                    <button class="close" type="button" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">×</span>
                    </button>
                </div>
                <div class="modal-body">
                    <p class="text-center">
                        <img v-bind:src="imgSrc" alt="#" class="img-fluid">
                    </p>
                    <p>{{ text }}</p>
                </div>
                <div class="modal-footer">
                    <button class="btn btn-secondary" type="button" data-dismiss="modal">Close</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class modal extends Vue {
    @Prop({ default: ''})
    id!: string;

    @Prop({ default: '' })
    title!: string;

    @Prop({ default: '' })
    imgSrc!: string;

    @Prop({ default: '' })
    text!: string;

    mounted() {
        console.log(this.$props);
    }
    
    created() {
        console.log('This is Modal component.');
    }
}
</script>