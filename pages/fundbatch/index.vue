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
            <div class="side-bar w-2/12 fixed top-5 bottom-5  left-5 rounded-xl mb-5 shadow-2xl  bg-white">
                <div class="pt-10 relative" align="center">
                    <div style="height: 85vh" class="flex flex-col justify-between">
                        <div class="pt-5"> 
                            <div class="app-logo">
                                <div class="font-bold text-2xl"><span class="text-primary">Fund</span>batch</div>
                            </div>
                            <div class="profile-img pt-10">
                                <img src="@/assets/profile1.jpg" style="height: 90px; width: 90px; " class="rounded-full" alt="">
                            </div>
                            <div class="user-name pt-5">
                                <h3 class="text-sm font-light text-gray-500">Welcome back,</h3>
                                <div class="text-primary pt-1 font-bold">Simeone Nortey</div>
                            </div>
                            <div class="monthly-budget pt-10">
                                <div class="font-bold text-3xl">$4,300</div>
                                <div class="text-gray-500">Monthly budget</div>
                            </div>
                            <div class="pt-10">
                                <ul class="nav-items px-20">
                                    <li>
                                        <a class="flex py-5">
                                        <span class="mdi mdi-view-dashboard pr-4"></span>
                                        <p class="float-left">Dashboard </p>
                                        </a>
                                    </li>
                                    <li>
                                        <a class="flex py-5 text-gray-500">
                                        <span class="mdi mdi-chart-multiple pr-4"></span>
                                        <p class="float-left">Investments </p>
                                        </a>
                                    </li>
                                    <li>
                                        <a class="flex py-5 text-gray-500">
                                        <span class="mdi mdi-swap-horizontal pr-4"></span>
                                        <p class="float-left">Transactions </p>
                                        </a>
                                    </li>
                                    <li>
                                        <a class="flex py-5 text-gray-500">
                                        <span class="mdi mdi-wallet-outline pr-4"></span>
                                        <p class="float-left ">Wallets </p>
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                        <div>
                            <div class="">
                                <ul class="px-20">
                                    <li>
                                        <a class="flex py-5">
                                        <span class="mdi mdi-logout pr-4"></span>
                                        <p class="float-left">Sign-out </p>
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                </div>

                
            </div>
            <div class="main-content pl-96 pr-40">
                <div class="w-full">
                    <div class="page-header pt-10 pb-5 font-bold text-primary text-2xl">Dashboard</div>

                    <div class="grid grid-cols-2 gap-10">
                        <div>
                            <div class="">
                                <div class="card p-10 bg-white shadow-lg rounded-lg" style="height: 321px">
                                    card
                                </div>
                            </div>
                        </div>
                        <div>
                            content1
                        </div>
                    </div>
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
.card {
    width: 100%;
}
</style>