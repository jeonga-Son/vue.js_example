<template>
<div>
    <div>
        <input type="checkbox" name="" id="html" value="html" v-model="favoritLang"/>
        <label for="html">HTML</label>
    </div>
    <div>
        <input type="checkbox" name="" id="html" value="css" v-model="favoritLang"/>
        <label for="css">CSS</label>
    </div>
    <div>
        <input type="checkbox" name="" id="js" value="JS" v-model="favoritLang"/>
        <label for="js">JavaScript</label>
    </div>
    <div>선택한 지역 : {{favoritLang}}</div>
</div>
</template>
<script>
 
export default{ 
    name:'',
    components:{},
    data(){
        return{
            favoritLang: ['JS'] // default값을 JS 로 주었다.
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{}
}
</script>