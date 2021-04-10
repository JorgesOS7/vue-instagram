<template>
    <main class="h-screen overflow-y-auto">
        <section class="px-4 py-2 border-b border-gray-900">
            <Stories />
        </section>
        <section class="divide-y divide-gray-900">
            <div class="flex flex-col pb-4" v-for="item in 4" :key="item">
                <div class="flex flex-row justify-between items-center space-x-1 p-2">
                    <div class="flex flex-row items-center space-x-4">
                        <img src="../assets/user.jpg" class="w-10 h-10 object-cover rounded-full" alt="">
                        <span class="text-sm font-medium">Michelle Smith</span>
                    </div>
                    <button>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z" />
                        </svg>
                    </button>
                </div>
                <div>
                    <div class="w-full h-96" style="background-image: url('https://images.unsplash.com/photo-1578836537282-3171d77f8632?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80');background-repeat: no-repat;background-size: cover;background-blend-mode: multiply;"></div>
                </div>
                <div class="flex flex-col px-4">

                    <div class="flex justify-between py-2">
                        <div class="flex flex-row items-center space-x-4">
                            <button>
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
                                </svg>
                            </button>
                            <button>
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
                                </svg>
                            </button>
                            <button>
                                <svg class="w-6 h-6 fill-current" version="1.1" id="Capa_1"
                                xmlns="http://www.w3.org/2000/svg"
                                xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 512.001 512.001" style="enable-background:new 0 0 512.001 512.001;" xml:space="preserve">
                                <g>
                                    <g>
                                    <path d="M507.608,4.395c-4.243-4.244-10.609-5.549-16.177-3.321L9.43,193.872c-5.515,2.206-9.208,7.458-9.42,13.395
                                    c-0.211,5.936,3.101,11.437,8.445,14.029l190.068,92.181l92.182,190.068c2.514,5.184,7.764,8.455,13.493,8.455
                                    c0.178,0,0.357-0.003,0.536-0.01c5.935-0.211,11.189-3.904,13.394-9.419l192.8-481.998
                                    C513.156,15.001,511.851,8.638,507.608,4.395z M52.094,209.118L434.72,56.069L206.691,284.096L52.094,209.118z M302.883,459.907
                                    l-74.979-154.599l228.03-228.027L302.883,459.907z"/>
                                    </g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                <g>
                                </g>
                                </svg>
                            </button>
                        </div>
                        <button>
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 5a2 2 0 012-2h10a2 2 0 012 2v16l-7-3.5L5 21V5z" />
                            </svg>
                        </button>
                    </div>
                    <div class="">
                        <p class="font-medium">Liked by Albert_1231 and others </p>
                    </div>
                    <div class="">
                        <p class="font-medium text-gray-500">View all 360 comments</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<script>
import Stories from '@/components/Stories';
export default {
    name: 'Feed',

    components: {
        Stories
    }
}
</script>
<style>
/* .scrollbar-story::-webkit-scrollbar {
  width: 0.25rem;
  height: 0.25rem;
}

.scrollbar-story::-webkit-scrollbar-track {
  background-color: #08090B;

}

.scrollbar-story::-webkit-scrollbar-thumb {
  background-color: #08090B;
}

.scrollbar-story::-webkit-scrollbar-thumb {
  border-radius: 0.25rem;
} */
</style>