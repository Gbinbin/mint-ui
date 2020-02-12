<template>
    <div id="alert" ref="alert">
        <div class="alert_content">
            <div class="alert_title">{{ alert_title }}</div>
            <div class="alert_body">{{ customBody }}</div>
            <div class="alert_btn">
                <button v-if="confirmBtn" @touchstart="confirmBtn">确认</button>
                <button v-if="cancelBtn" @touchstart="cancelBtn">取消</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: '',
    data () {
        return {

        }
    },
components: {

}
}
</script>

<style scoped>


</style>
