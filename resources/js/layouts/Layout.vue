<script setup lang="ts">
import { Link } from '@inertiajs/vue3';
import { home } from '@/routes';
</script>

<template>
    <div class="flex min-h-screen flex-col bg-base-200 font-sans">
        <nav class="navbar bg-base-100">
            <div class="navbar-start">
                <Link :href="home()" class="btn btn-ghost text-xl">
                    <img src="/yapper.png" alt="Y" width="50" />
                    Yapper
                </Link>
            </div>
            <div class="navbar-end gap-2">
                <a href="#" class="btn btn-ghost btn-sm">Sign In</a>
                <a href="#" class="btn btn-primary btn-sm">Sign Up</a>
            </div>
        </nav>

        <main class="container mx-auto flex-1 px-4 py-8">
            <slot />
        </main>

        <footer class="footer footer-center bg-base-300 p-5 text-xs text-base-content">
            <div>
                <p>© {{ new Date().getFullYear() }} Yapper city - Built with Laravel</p>
            </div>
        </footer>
    </div>
</template>
