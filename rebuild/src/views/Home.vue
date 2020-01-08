<template>
    <div>
        <van-tabs v-model="active" animated swipeable>
            <van-tab title="标签页1">
                    <DailyAffairs/>
            </van-tab>
            <van-tab title="标签页2">
                    <Affairs/>
            </van-tab>
            <van-tab title="标签页3">
                    <Affairs/>
            </van-tab>
        </van-tabs>
        <!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    </div>
</template>

<script>
    // @ is an alias to /src
    import DailyAffairs from '@/components/DailyAffairs.vue';
    import Affairs from "@/components/Affairs";

    export default {
        name: 'home',
        components: {
            DailyAffairs,
            Affairs
        },
        data() {
            return {
                active: "标签页1"
            };
        }
    }
</script>
