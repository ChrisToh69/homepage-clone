<template>
    <div class="flex justify-center">
        <h1 class="border-l-2 border-black text-xl mt-20 pl-4 text-center">
            <span class="font-bold">产品</span>
        </h1>
    </div>

    <div class="grid grid-cols-3 min-h-[800px] gap-2 h-full w-full ">
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
        {class:"row-span-2",
        backgroundImage: "/images/category-1-jpg.webp",
        icon: "/icons/category-icon-2-1.png",
        text: "One"},
    {
        class:"col-span-2",
        backgroundImage: "/images/category-2-jpg.webp",
        icon: "/icons/category-icon-3-1.png",
        text: "Two"
    },
    {
        backgroundImage: "/images/category-3-jpg.webp",
        icon: "/icons/category-icon-4-1.png",
        text: "Three"
    },
    {
        backgroundImage: "/images/category-4-jpg.webp",
        icon: "/icons/category-icon-5-1.png",
        text: "Four"
    },
    {   class:"col-span-2",
        backgroundImage: "/images/category-1-jpg.webp",
        icon: "/icons/category-icon-2-1.png",
        text: "One"},
    {   
        class:"row-span-2",
        backgroundImage: "/images/category-2-jpg.webp",
        icon: "/icons/category-icon-3-1.png",
        text: "Two"
    },
    {   
        backgroundImage: "/images/category-3-jpg.webp",
        icon: "/icons/category-icon-4-1.png",
        text: "Three"
    },
    {   
        backgroundImage: "/images/category-4-jpg.webp",
        icon: "/icons/category-icon-5-1.png",
        text: "Four"}
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