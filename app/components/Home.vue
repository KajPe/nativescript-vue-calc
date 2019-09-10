<template>
    <Page class="page">
        <ActionBar class="action-bar">
            <Label class="action-bar-title" text="Home"></Label>
        </ActionBar>

        <StackLayout>
            <Button text="Calculator" @tap="goToCalc" class="btn" />
        </StackLayout>
    </Page>
</template>

<script>
    import Calc from './Calculator'

    export default {
        data () {
            return {
            };
        },
        methods: {
            goToCalc() {
                this.$navigateTo(Calc);
            }
        }
    };
</script>

<style scoped>
.btn {
    background-color: #6699ff;
    color: #ffffff;
    font-size:24px;
    width: 300;
    height: 80;
    margin-top: 30;
    padding: 0;
    border: 0;
    border-radius: 40;
}
</style>
