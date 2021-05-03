<template>
    <tbody>
        <tr v-for="(content, key) in contents" v-bind:key="key">
            <th>{{ content.name }}</th>
            <td>{{ content.about }}</td>
        </tr>
    </tbody>
</template>

<script lang="ts">
import { Component, Prop, Vue} from 'vue-property-decorator';

@Component
export default class TableBody extends Vue {
    @Prop({ default: [] })
    contents!: Array<any>;

    mounted() {
        console.log(this.$props);
    }
    
    created() {
        console.log('This is TableBody component.');
    }
}
</script>