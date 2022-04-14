<template>
    <img 
    src="@/assets/logo.svg"
    class="icon" >
</template>

<script>

export default {
    name: 'Icon',
    props:['icon'],
    data() {
        return{
            skillIcons:[
                {
                    id:1,
                    img:'@/assets/logo.svg',
                    alt: "Vue icon"
                },
                {
                    id:2,
                    img:'@/assets/imgs/skillTree_icon_html.png',
                    alt: "HTML icon"
                }
            ]       
        }
    }
}
</script>