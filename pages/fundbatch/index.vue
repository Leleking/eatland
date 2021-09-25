<template>
    <div>
        <div class="h-screen rounded-md  bg-grey w-screen relative">
            <div class="nav h-30 bg-gray-400">
                <div class="absolute xl:left-1/4 left-0   right-0 top-10 px-5">
                    <div class=" w-full">
                        <div class="grid lg:grid-cols-12 lg:gap-20 md:gap-10 ">
                            <div class="lg:col-span-5 col-span-12">
                                <input class="h-14 w-full rounded-full" placeholder="Search" type="text">
                            </div>
                            <div class="lg:col-span-6">
                                <div class="flex justify-end">
                                    <div class="grid  grid-cols-2 gap-4">
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
                        
                    </div>
                    <!-- <div class="flex items-center h-28 justify-between">
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
                        
                    </div> -->
                </div>
            </div>
            <div class="side-bar w-72 absolute top-5 bottom-5 hidden xl:block  left-10 rounded-xl mb-0 shadow-2xl  bg-white">
                <div class="pt-5 relative" align="center">
                    <div class="flex flex-col justify-between">
                        <div class="pt-1"> 
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
                            <div class="flex justify-center pt-10">
                                <ul class=" nav-items">
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
                                    <li class="pt-20">
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
            <div class="main-content absolute xl:left-1/4  right-0 left-0 px-5">
                <div class="w-full">
                    <div class="page-header pt-10 pb-5 font-bold text-primary text-2xl">Dashboard</div>
                    <div class="page">
                        <div class="grid lg:grid-cols-12 lg:gap-20 md:gap-10 ">
                            <div class="lg:col-span-5 col-span-12">
                                <div class="card  p-10 bg-white shadow-lg rounded-2xl" style="height: 321px">
                                    <div class="flex flex-col justify-between h-full">
                                        <div class="flex justify-between">
                                        <div class="text-gray-500">Available balance</div>
                                        <div>
                                            <span class="text-gray-500">Credit:</span>
                                            <el-switch  v-model="card">
                                            </el-switch>
                                        </div>
                                    </div>
                                    <div>
                                        <span class="font-bold text-6xl">$2,200</span>
                                    </div>
                                    <div class="flex justify-between items-center">
                                        <div>**** 4532</div>
                                        <div>
                                            <img class="h-20" src="@/assets/mc.svg" alt="">
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            <div class="lg:col-span-6">
                                <div class="text-primary font-bold">Expenses Statistics</div>
                                <div id="chart pt-5" style="height: 321px">
                                    <apexchart width="400" type="donut" :options="chartOptions" :series="series"></apexchart>
                                </div>
                            </div>          
                        </div>
                        <div class="grid lg:grid-cols-12 lg:gap-20 md:gap-10 pt-10">
                            <div class="lg:col-span-5 col-span-12">
                                <div>
                                    <div>
                                        <div class="flex  justify-between">
                                            <div class="text-gray-500">Internet payment limit</div>
                                            <div><span class="text-primary">$1,200</span> / <span class="text-gray-500">3000</span> </div>
                                        </div>
                                        <el-progress class="pt-3" :percentage="50" color="#215287" :show-text="false"></el-progress>
                                    </div>
                                    <div class="pt-10">
                                        <div class="grid xl:grid-cols-2 grid-cols-1  gap-4">
                                            <div class="border p-5 rounded-3xl">
                                                <div class="flex items-center">
                                                    <div class="pr-5">
                                                        <el-progress :width='50' type="circle" :percentage="70" color="black"></el-progress>
                                                    </div>
                                                    <div>
                                                        <div>Income</div>
                                                        <div>$5,700</div>
                                                    </div>
                                                </div>
                                                
                                            </div>
                                            <div class=" p-5 rounded-3xl shadow-xl bg-white">
                                                <div class="flex items-center">
                                                    <div class="pr-5">
                                                        <el-progress :width='50' type="circle" :percentage="70" color="black"></el-progress>
                                                    </div>
                                                    <div>
                                                        <div>Income</div>
                                                        <div>$5,700</div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="lg:col-span-6">
                                <div>
                                <div class="flex justify-between items-center">
                                    <div class="text-primary font-bold">Send money to</div>
                                    <div><span class="text-primary text-3xl">+</span> </div>
                                </div>
                                <div class="pt-2">
                                    <hr>
                                </div>
                                <div class="pt-5">
                                    <div class="space-x-10" style="overflow: auto">
                                        <div class="inline-block w-20" align="center" v-for="i in 4" :key="i">
                                            <img src="@/assets/profile2.jpg" class="avatar" alt="">
                                            <div class="pt-2 sub-text">James Liena jsjd kskd</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            </div>          
                        </div>
                    </div>

                    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    
    export default {
        data() {
            return {
                card: false,
                series: [44, 55, 41],
                chartOptions: {
                    chart: {
                    type: 'donut',
                    },
                    responsive: [{
                    breakpoint: 480,
                    options: {
                        chart: {
                            width: 200
                        },
                        legend: {
                        position: 'bottom'
                        }
                    }
                    }]
                },
            }
        },
    }
</script>

<style lang="scss" scoped>
::placeholder {
    padding-left: 30px
}
.card {
    width: 100%;
}
.nav {
    background: url('../../assets/bg1.png');
    background-repeat: no-repeat;
    background-size: cover;
    height: 15vh;
}
.avatar {
    height: 70px;
    width: 70px;
    border-radius: 50%;
}
.sub-text {
    font-size: 12px;
    color: grey;
}
</style>