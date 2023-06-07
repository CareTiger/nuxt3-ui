<template>
    <div>
        <UContainer>
            <fieldset>
                <legend
                    class="text-base font-semibold leading-6 text-gray-900 block">
                    Notifications
                </legend>
                <p class="mt-1 text-sm leading-6 text-gray-600">
                    How would you like to be notified?
                </p>
                <div class="mt-6 space-y-6">
                    <div class="relative flex gap-x-3">
                        <UCheckbox
                            label="Email"
                            help="Get notified by email." />
                    </div>
                    <div class="relative flex gap-x-3">
                        <UCheckbox label="SMS" help="Get notified by SMS." />
                    </div>
                    <div class="relative flex gap-x-3">
                        <UCheckbox
                            disabled
                            :checked="true"
                            label="In app"
                            help="Get notified in app." />
                    </div>
                    <div class="relative flex gap-x-3">
                        <UCheckbox
                            disabled
                            checked="true"
                            label="In app"
                            help="Get notified in app." />
                    </div>
                </div>
            </fieldset>
        </UContainer>
    </div>
</template>
