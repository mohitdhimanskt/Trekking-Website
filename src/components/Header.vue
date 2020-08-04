<template>
    <div>
            <div class="header">
            <router-link to="/"><img src="/static/FOH.PNG"></router-link>
            <h5>Far Out Himalaya</h5>
                <div class="header-btn">
            <router-link to="/about"><span class="header">About us</span></router-link>
            <!-- <button class="header" type="button"><span class="header">Login</span></button>
            <button class="header" type="button"><span class="header">Sign up</span></button> -->
                </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Header',
    props: {
        title: String
    },
    data: function() {
        return {
            name: 'Mohit'
        }
    }
}
</script>
<style scoped>
h5 {
flex: 1;
color: #F5004C;
margin: 10px 1289px 0px 10px;
}
.header-btn{
    width: 180%;
    display: inherit;
    align-items: inherit;
    justify-content: inherit;
}
.header{
    color: rgba(0, 0, 0, 0.87);
    padding: 8px 16px;
    font-size: 0.875rem;
    min-width: 64px;
    box-sizing: border-box;
    min-height: 36px;
    transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
    font-family: "Roboto", "Helvetica", "Arial", sans-serif;
    font-weight: 500;
    line-height: 1.5;
    border-radius: 4px;
    letter-spacing: 0.02857em;
    text-transform: uppercase;
}


</style>