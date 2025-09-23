<script>
    export default { 

       // add code here
        data(){
            return {
                select : 'Username',

            }
        }
    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="select">
        <option value="Username">Username login</option>
        <option value="Email">Email login</option>
    </select>
    
    <div>
        <label v-if="select == 'Username'">Username</label>
        <label v-if="select == 'Email'">Email</label> 
        <input v-if="select =='Username'" placeholder="Enter your username">
        <input v-if="select =='Email'" placeholder="Enter your email address">
    </div>
</template>

