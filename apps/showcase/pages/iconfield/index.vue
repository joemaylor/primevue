<template>
    <DocComponent title="Vue IconField" header="IconField" description="IconField wraps an input and an icon." :componentDocs="docs" :ptTabComponent="ptComponent" :apiDocs="['IconField', 'InputIcon']" :themingDocs="themingDoc" />
</template>

<script>
import AccessibilityDoc from '@/doc/iconfield/AccessibilityDoc.vue';
import BasicDoc from '@/doc/iconfield/BasicDoc.vue';
import FloatLabelDoc from '@/doc/iconfield/FloatLabelDoc.vue';
import IftaLabelDoc from '@/doc/iconfield/IftaLabelDoc.vue';
import SizesDoc from '@/doc/iconfield/SizesDoc.vue';
import ImportDoc from '@/doc/iconfield/ImportDoc.vue';
import TemplateDoc from '@/doc/iconfield/TemplateDoc.vue';
import PTComponent from '@/doc/iconfield/pt/index.vue';
import ThemingDoc from '@/doc/iconfield/theming/index.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'import',
                    label: 'Import',
                    component: ImportDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'template',
                    label: 'Template',
                    component: TemplateDoc
                },
                {
                    id: 'floatlabel',
                    label: 'Float Label',
                    component: FloatLabelDoc
                },
                {
                    id: 'iftalabel',
                    label: 'Ifta Label',
                    component: IftaLabelDoc
                },
                {
                    id: 'sizes',
                    label: 'Sizes',
                    component: SizesDoc
                },
                {
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            ptComponent: PTComponent,
            themingDoc: ThemingDoc
        };
    }
};
</script>
