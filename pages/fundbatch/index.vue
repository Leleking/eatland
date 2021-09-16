<template>
    <div>
        <div class="h-screen rounded-md relative bg-grey">
            <div class="nav h-30 bg-gray-400">
                <div class="pl-96 pr-40 pt-5">
                    <div class="flex items-center h-28 justify-between w-full">
                        <div class="w-2/5">
                            <input class="h-14 w-full rounded-full" placeholder="Search" type="text">
                        </div>
                        <div class="grid grid-flow-col grid-cols-2 gap-4">
                            <div class="nav-icon h-14 w-14 flex justify-center items-center rounded-full bg-white">
                                <span class="mdi mdi-cog-outline text-gray-500 text-lg"></span>
                            </div>
                            <div class="nav-icon h-14 w-14 flex justify-center  items-center rounded-full bg-white">
                                <span class="mdi mdi-bell-outline text-gray-500 text-lg"></span>
                            </div>
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="side-bar w-2/12 absolute top-5  left-5 rounded-xl mb-5 shadow-2xl  bg-white" style="height: 90vh">
                <div class="pt-10" align="center">
                    <div class="h-full flex flex-col justify-between flex-grow">
                        <div class="pt-5"> 
                            <div class="font-bold text-2xl"><span class="text-primary">Fund</span>batch</div>
                        </div>
                        <div>  1</div>
                        <div>  1</div>
                    </div>
                    
                </div>

                
            </div>
            <div class="main-content pl-96 pr-40">
                <div class="border w-full">
                    content
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
::placeholder {
    padding-left: 30px
}
</style>