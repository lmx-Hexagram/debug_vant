<template>
    <div>
            <van-swipe-cell>

                <van-cell :border="false" title="overlay" value="test" v-on:click="showDetail=true"/>
                <van-cell :border="false" title="popup" value="test" v-on:click="showDetail1=true"/>
                <van-cell :border="false" title="none" value="test" v-on:click="showDetail2=true"/>

                <template slot="right">
                    <van-button square type="primary" text="选择"/>
                </template>

            </van-swipe-cell>

            <van-overlay :show="showDetail" @click="showDetail = false" />
            <van-popup v-model="showDetail1">内容</van-popup>
    </div>
</template>

<script>
    export default {
        name: 'Affairs',
        data(){
            return{
                showDetail:false,
                showDetail1:false,
                showDetail2:false,
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
