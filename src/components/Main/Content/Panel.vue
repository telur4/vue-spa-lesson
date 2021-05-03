<template>
    <!-- パネル -->
    <div class="tab-pane fade show border border-top-0" v-bind:class="isActive()" v-bind:id="'panel-' + id" role="tabpanel" v-bind:aria-labelledby="'tab-' + id">
        <div class="row p-3">
            <div class="col-md-7 order-md-2">
                <h4>{{ title }}</h4>
                <table class="table table-striped">
                    <tbody>
                        <tr v-for="(content, key) in contents" v-bind:key="key">
                            <th>{{ content.name }}</th>
                            <td>{{ String(content.price) + "円（税別）" }}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <div class="col-md-5">
                <img v-bind:src="imgSrc" v-bind:alt="imgAlt" class="img-fluid" />
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Emit, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Panel extends Vue {
    @Prop({ default: '' })
    id!: string;

    @Prop({ default: '' })
    title!: string;

    @Prop({ default: false })
    active!: boolean;

    @Prop({ default: [] })
    contents!: Array<any>

    @Prop({ default: '' })
    imgSrc!: string;

    @Prop({ default: '' })
    imgAlt!: string;

    @Emit('is-active')
    isActive() {
        return this.$props.active ? "active" : "";
    }

    mounted() {
        console.log(this.$props);
    }
    
    created() {
        console.log('This is Panel component.');
    }
}
</script>