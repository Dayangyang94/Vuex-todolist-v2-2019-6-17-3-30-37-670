
<template>
    <div>
        <h1>Welcome to {{username}}!</h1>
        <br/>
         <div><router-link :to="'/welcome/'+username">Welcome</router-link></div>
        <br/>
        <div><router-link :to="{name:'counter'}">Go to Counter</router-link></div> 
        <br/>
        <div><router-link :to="{name: 'toDoList'}">Go to toDoList</router-link></div>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    name: "welcome",
    props: ['username']
}
</script>