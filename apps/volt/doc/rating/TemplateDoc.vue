<template>
    <DocSectionText v-bind="$attrs">
        <p>Custom icons are used to override the default icons with <i>onicon</i>, <i>officon</i> and <i>cancelicon</i> slots.</p>
    </DocSectionText>
    <div class="card flex justify-center">
        <Rating v-model="value">
            <template #onicon>
                <img src="https://primefaces.org/cdn/primevue/images/rating/custom-onicon.png" height="24" width="24" />
            </template>
            <template #officon>
                <img src="https://primefaces.org/cdn/primevue/images/rating/custom-officon.png" height="24" width="24" />
            </template>
        </Rating>
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import Rating from '@/volt/Rating.vue';
import { ref } from 'vue';

const value = ref(null);

const code = ref(`
<template>
    <div class="card flex justify-center">
        <Rating v-model="value">
            <template #onicon>
                <img src="https://primefaces.org/cdn/primevue/images/rating/custom-onicon.png" height="24" width="24" />
            </template>
            <template #officon>
                <img src="https://primefaces.org/cdn/primevue/images/rating/custom-officon.png" height="24" width="24" />
            </template>
        </Rating>
    </div>
</template>

<script setup lang="ts">
import Rating from '@/volt/Rating.vue';
import { ref } from 'vue';

const value = ref(null);
<\/script>
`);
</script>
