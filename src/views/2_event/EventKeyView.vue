<template>
<div>
    <!-- <input type="search" name="" id="" @keyup="checkEnter($event)" v-model="searchText"> -->
    <input type="search" name="" id="" @keyup.stop="doSearch" v-model="searchText">
    <button @click="doSearch">조회</button>
    <button type="submit" @click.prevent="doSearch"></button>
</div>
</template>
<script>
// .enter
// .tap
// .delete
// .esc
// .space
// .up
// .down
// .left
// .right
// .stop - event.stopPropagation()
// .prevent  -event.preventDefault()
export default{ 
    name:'',
    components:{},
    data(){
        return{
            sampleData:''
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{
        doSearch() {
            console.log(this.searchText)
        },
        checkEnter(event) {
            // event.stopPropagation();
            if(event.keyCode === 13) {
                this.doSearch()
            }
        }
    }
}
</script>