<template>
    <div class="text-gray-500 font-serif">
        <div>
            <nav>
                <div>
                    <h1>
                        <a href="/">Food Ninja</a>
                    </h1>
                </div>
                <ul>
                    <li>
                        <a href="">
                            <span>
                                home
                            </span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span>
                                About
                            </span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span>
                                Contact
                            </span>
                        </a>
                    </li>
                </ul>
            </nav>
        </div><!-- end nav -->
        <main class="px-6 py-6">
            <div >
                <a href="#" class="text-primary">Log in</a>
                <a href="#" class="text-secondary-200">Sign up</a>
            </div>
            <header>
                <h2 class="text-gray-700 text-5xl">Recipes</h2>
                <h3 class="text-2xl">For Ninjas</h3>
            </header>
            <div>
                <h4 class="font-bold mt-12 pb-2 border-b border-gray-200 text-mammoth">Latest Recipes</h4>
                <div>
                    <div class="mt-8">

                        <!--  medium:after_download_modal.copy_text.photo: https://www.pexels.com/photo/cooked-food-704569/ -->
                        <img src="@/assets/food1.jpg" alt="">
                        <div>
                            <span>4 Bean Chilli Stew</span>
                            <span>Recipe by Mario</span>
                        </div>
                    </div>
                    
                </div>
            </div>
            <h4 class="font-bold mt-12 pb-2 border-b border-gray-200 ">Most Popular</h4>
            <div>
                <!--- cards go here-->
            </div>
            <div>
                <div class="bg-secondary-100 text-color-secondary">Load  more </div>
            </div>
        </main>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>