<template>
    <div
        class="bg-white shadow-[0_-4px_8px_0px_rgba(0,0,0,0.1)] md:hidden w-full h-16 rounded-t-lg fixed bottom-0 right-0 left-0 border-t-2">
        <nav class="w-full h-full flex items-center">
            <ul class="flex w-full px-2 justify-between gap-x-2 items-center">
                <li class="flex-auto">
                    <NuxtLink to="/" class="flex items-center justify-center gap-x-2 py-2 w-full text-gray-400">
                        <span>
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="currentColor">
                                <path
                                    d="M26.72 9.094 19.04 3.72c-2.093-1.466-5.307-1.386-7.32.174L5.04 9.107c-1.333 1.04-2.387 3.173-2.387 4.853v9.2c0 3.4 2.76 6.174 6.16 6.174h14.374c3.4 0 6.16-2.76 6.16-6.16v-9.04c0-1.8-1.16-4.014-2.627-5.04ZM17 24c0 .547-.453 1-1 1-.547 0-1-.453-1-1v-4c0-.546.453-1 1-1 .547 0 1 .454 1 1v4Z" />
                            </svg>
                        </span>
                        <span v-show="route.path === '/'">خانه</span>
                    </NuxtLink>
                </li>
                <li class="flex-auto">
                    <NuxtLink to="" class="disabled flex items-center justify-center  gap-x-2 py-2 w-full text-gray-400">
                        <span>
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8">
                                <g fill="currentColor">
                                    <path
                                        d="M10.257 2.833H7.565c-3.102 0-4.732 1.63-4.732 4.718v2.692c0 3.088 1.63 4.717 4.718 4.717h2.692c3.088 0 4.717-1.629 4.717-4.717V7.55c.014-3.088-1.615-4.718-4.703-4.718ZM26.45 2.833h-2.692c-3.089 0-4.718 1.63-4.718 4.718v2.692c0 3.088 1.63 4.717 4.718 4.717h2.691c3.088 0 4.718-1.629 4.718-4.717V7.55c0-3.088-1.63-4.718-4.718-4.718ZM26.45 19.026h-2.692c-3.089 0-4.718 1.629-4.718 4.717v2.692c0 3.088 1.63 4.718 4.718 4.718h2.691c3.088 0 4.718-1.63 4.718-4.718v-2.692c0-3.088-1.63-4.717-4.718-4.717ZM10.257 19.026H7.565c-3.102 0-4.732 1.629-4.732 4.717v2.692c0 3.103 1.63 4.732 4.718 4.732h2.692c3.088 0 4.717-1.63 4.717-4.718v-2.692c.014-3.102-1.615-4.731-4.703-4.731Z" />
                                </g>
                            </svg>
                        </span>
                        <span v-show="route.path === '/category'">دسته بندی</span>
                    </NuxtLink>
                </li>
                <li class="flex-auto">
                    <NuxtLink to="/cart" class="flex items-center justify-center gap-x-2 py-2 w-full text-gray-400">
                        <span>
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="currentColor">
                                <path
                                    d="M28.277 12.693c-.95-1.048-2.38-1.657-4.364-1.87V9.747a6.9 6.9 0 0 0-2.266-5.114c-1.46-1.332-3.358-1.955-5.327-1.771-3.386.326-6.233 3.598-6.233 7.14v.821c-1.984.213-3.415.822-4.364 1.87-1.374 1.53-1.331 3.57-1.176 4.987l.992 7.89c.298 2.763 1.417 5.597 7.508 5.597h7.905c6.092 0 7.211-2.834 7.509-5.582l.992-7.92c.155-1.402.184-3.442-1.176-4.972ZM16.518 4.831c1.417-.128 2.763.312 3.811 1.26a4.925 4.925 0 0 1 1.615 3.656v.991h-9.888v-.736c0-2.522 2.082-4.944 4.462-5.171Zm-4.59 13.798h-.014a1.42 1.42 0 0 1-1.416-1.416 1.424 1.424 0 0 1 2.848 0 1.42 1.42 0 0 1-1.418 1.416Zm9.917 0h-.014a1.42 1.42 0 0 1-1.417-1.416 1.424 1.424 0 0 1 2.848 0 1.42 1.42 0 0 1-1.417 1.416Z" />
                            </svg>
                        </span>
                        <span v-show="route.path === '/cart'">سبد خرید</span>
                    </NuxtLink>
                </li>
                <li class="flex-auto">
                    <NuxtLink to="" class="disabled flex items-center justify-center gap-x-2 py-2 w-full text-gray-400 ">
                        <span class="pt-1">
                            <svg xmlns="http://www.w3.org/2000/svg" width="29" height="25" fill="currentColor">
                                <path
                                    d="M20.834.333a7.702 7.702 0 0 0-6.156 3.09A7.701 7.701 0 0 0 8.522.332C4.278.333.833 3.8.833 8.067c0 1.644.267 3.178.712 4.578 2.177 6.91 8.933 11.066 12.266 12.2.467.155 1.245.155 1.711 0 3.334-1.134 10.09-5.267 12.267-12.2.467-1.423.711-2.934.711-4.578C28.522 3.8 25.078.333 20.834.333Z" />
                            </svg>
                        </span>
                        <span v-show="route.path === '/interests'">علاقه مندی ها</span>
                    </NuxtLink>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script setup>
const route = useRoute();
const activeButtomTab = ref(1);
</script>

<style scoped>
.router-link-active {
    @apply text-slate-800 font-bold;
}

.disabled {
    pointer-events: none;
    cursor: default;
}
</style>