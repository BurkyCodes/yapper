<script setup lang="ts">
import { Head } from '@inertiajs/vue3';
import Layout from '@/layouts/Layout.vue';

defineOptions({ layout: Layout });
</script>

<template>
    <div class="mx-auto max-w-2xl">
        <Head title="Welcome" />
        <div class="card bg-base-100 shadow mt-8">
            <div class="card-body">
                <div>
                    <h1 class="text-3xl font-bold">Welcome to Yapper City</h1>
                    <p class="mt-4 text-base-content/60">This is your brand new Laravel application. Time to make it
                        sing (or chirp)!</p>
                </div>
            </div>
        </div>
    </div>
</template>
