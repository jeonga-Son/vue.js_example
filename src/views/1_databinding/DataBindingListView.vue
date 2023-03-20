<template>
<div>
    <div>
        <select name="" id="">
            <option :value="city.code" :key="city.code" v-for="city in cities">{{city.title}}</option>
        </select>
    </div>
    <div>
        <table>
            <thead>
                <tr>
                    <th>제품번호</th>
                    <th>제품명</th>
                    <th>가격</th>
                    <th>주문수량</th>
                    <th>합계</th>
                </tr>
            </thead>
            <tbody>
                <tr :key="drink.drinkId" v-for="(drink) in drinkList">
                    <td>{{drink.drinkId}}</td>
                    <td>{{drink.drinkName}}</td>
                    <td>{{drink.price}}</td>
                    <td><input type="number" name="" id="" v-model="drink.quantity" /></td>
                    <td>{{drink.price * drink.quantity}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</div>
</template>
<script>

export default{ 
    name:'',
    components:{},
    data(){
        return{
            cities: [
                {title: '서울', code: '02'},
                {title: '부산', code: '051'},
                {title: '제주', code: '064'}
            ],
            drinkList: [
                {
                drinkId: '1',
                drinkName: '코카콜라',
                price: 700,
                quantity: 1
                },
                {
                drinkId: '2',
                drinkName: '제로 사이다',
                price: 900,
                quantity: 1
                },
                {
                drinkId: '3',
                drinkName: '델몬트 오렌지',
                price: 1200,
                quantity: 3
                },
                {
                drinkId: '4',
                drinkName: '토마토 주스',
                price: 600,
                quantity: 1
                },
                {
                drinkId: '5',
                drinkName: '꿀맛 ZICO',
                price: 100,
                quantity: 6
                }
            ]
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{}
}
</script>