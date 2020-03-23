<template>
    <div class="Watch">
        用户名：<input type="text" @input="handle($event)">{{msg}}
    </div>
</template>

<script>
    export default {
        name: "Watch",
        data:function(){
            return {
                username:'',
                msg:''
            }
        },
        methods:{
            handle:function(event){
                this.username = event.target.value;
                this.check();
            },
            check:function(){
                setTimeout(function(){
                    if(this.username === "admin"){
                        this.msg = "用户名重复，请重新输入！"
                    }else{
                        this.msg = "该用户名可用！"
                    }
                },2000);
            }
        }
    }
</script>

<style scoped>
    input{
        width:200px;
        height:30px;
        padding:0 10px;
    }
</style>