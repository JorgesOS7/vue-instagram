<template>
            <div class="flex flex-row overflow-x-scroll scrollbar-story">
                <div class="relative text-center rounded-full">
                    <img src="../assets/user.jpg" class="rounded-full max-w-xs w-14 h-14 object-cover">
                    <div class="rounded-full right-0 top-10 border-2 border-black absolute bg-blue-500">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6" />
                        </svg>
                    </div>
                    <p class="text-xs truncate">Your story</p>
                </div>
                <div class="flex flex-row space-x-2 pl-4">

                    <div class="text-center" v-for="item in 10" :key="item">
                        <div class="p-1 text-center bg-gradient-to-r from-yellow-400 via-red-500 to-pink-500 rounded-full">
                            <img src="../assets/user2.jpg" class="w-14 h-14 rounded-full max-w-xs object-cover border-2 border-black"/>
                        </div>
                        <p class="text-xs truncate w-14">Albert_1231</p>
                    </div>

                </div>
            </div>
</template>