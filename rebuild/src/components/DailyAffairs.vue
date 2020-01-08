<template>
    <div>
            <van-swipe-cell>
                <template slot="left">
                    <van-button square type="primary" text="选择"/>
                </template>

                <van-cell :border="false" title="test" value="test"/>
                <van-cell :border="false" title="test1" value="test"/>
                <van-cell :border="false" title="test2" value="test"/>
                <van-cell :border="false" title="test3" value="test"/>
                <van-cell :border="false" title="test4" value="test"/>
                <van-cell :border="false" title="test5" value="test"/>

            </van-swipe-cell>
    </div>
</template>

<script>
    export default {
        name: 'DailyAffairs',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
