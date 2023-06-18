<template>
    <div class="">
        <UContainer>
            <div class="min-h-screen grid place-items-center">
                <div>
                    <p class="text-2xl font-semibold leading-6 block mb-6">
                        Notifications
                    </p>
                    <ul class="flex flex-row space-x-4">
                        <li>
                            <UButton
                                label="Show success toast"
                                @click="toast.add({ title: 'Hello world!' })" />
                        </li>
                        <li>
                            <UButton color="red" label="Show error toast"
                            @click="toast.add({ title: 'Hello world!',
                            color:"red" })" />
                        </li>
                    </ul>
                </div>
            </div>
        </UContainer>
        <UNotifications />
    </div>
</template>
<script setup>
const toast = useToast();
</script>
