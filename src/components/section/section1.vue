<template>
    <div class="flex justify-center">
        <h1 class="border-l-2 border-black text-xl mt-20 pl-4 text-center mb-5">
            <span class="font-bold">产品</span>
        </h1>
    </div>

    <div class="grid grid-cols-3 min-h-[1200px] gap-2 h-full w-full ">
        <div :class= product.class v-for="product in products" :key="product.icon">
            <product 
            :cardDisplay="product" 
            />
        </div>
    </div>
</template>

<script>
import product from '../ui/product.vue';
export default {
data(){
    return{
    products: [ 
        {class:"row-span-2", // image 1
        backgroundImage: "/images/category-1-jpg.webp",
        icon: "/icons/Asset-62.png",
        text: "甘文烟/元宝粒/檀香粉"},
    {
        class:"col-span-2", // image 2
        backgroundImage: "/images/category-2-jpg.webp",
        icon: "/icons/category-icon-2-1.png",
        text: "盘香/塔粒"
    },
    {   // image 3
        backgroundImage: "/images/category-3-jpg.webp",
        icon: "/icons/category-icon-3-1.png",
        text: "蜡烛"
    },
    {   // image 4
        backgroundImage: "/images/category-4-jpg.webp",
        icon: "/icons/category-icon-4-1.png",
        text: "纸张"
    },
    {   // image 5
        class:"col-span-2",
        backgroundImage: "/images/category-5-jpg.webp",
        icon: "/icons/category-icon-5-1.png",
        text: "包装香"},
    {   // image 6
        class:"row-span-2",
        backgroundImage: "/images/category-8-jpg.webp",
        icon: "/icons/category-icon-6-1.png",
        text: "水晶酥油烛"
    },
    {   // image 7
        backgroundImage: "/images/category-6-jpg.webp",
        icon: "/icons/category-icon-7-1.png",
        text: "烧金桶"
    },
    {   // image 8
        backgroundImage: "/images/category-7-jpg.webp",
        icon: "/icons/category-icon-8-1.png",
        text: "冥币"}
    ]
    }
    
},
components:{
    product
}

}

</script>

<style>

</style>