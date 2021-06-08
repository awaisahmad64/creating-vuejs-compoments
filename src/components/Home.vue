<template>
    <div>
        <h1>This is my First Component</h1>
        <h2>{{data}}<br>{{msg}}</h2>
        <button v-on:mouseover="hello('parameter pass to call fun')">call function</button>
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data: String,
        msg: String
    },methods:{
        hello(data){
            alert(data);
        }
    }
}
</script>
