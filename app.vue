<template>
    <div class="h-screen">
        <UContainer class="grid place-items-center">
            <USelect v-model="component" :options="components" />
            <component :is="component" v-if="component" />
        </UContainer>
    </div>
</template>
<script setup>
const c1 = resolveComponent("Component1");
const c2 = resolveComponent("Component2");
const c3 = resolveComponent("Component3");
const components = shallowRef([c1, c2, c2]);
const component = shallowRef(components.value[0]);
</script>
