<template>
    <h1>{{$route.params.id}}</h1>
</template>
<script>
export default {
    //nuxt js run it before render the route
    validate(data){
        console.log(data);
        //测试是不是数字
        return /^\d+$/.test(data.params.id);
    }
}
</script>