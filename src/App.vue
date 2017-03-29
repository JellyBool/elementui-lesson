<template>
    <div id="app">
        <el-row :gutter="10">
            <el-col :xs="8" :sm="6" :md="4" :lg="3"><div class="grid-content bg-purple">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci illum in inventore mollitia pariatur perspiciatis recusandae sequi unde. Accusamus culpa facilis incidunt modi officia omnis quas quia, quod saepe tempora.</div></el-col>
            <el-col :xs="4" :sm="6" :md="8" :lg="9"><div class="grid-content bg-purple-light">
                <img src="./assets/logo.png">
                <h1>{{ msg }}</h1>
                <el-button :disabled="true" type="primary" @click.native="startHacking">Let's do it</el-button>
            </div></el-col>
            <el-col :xs="4" :sm="6" :md="8" :lg="9"><div class="grid-content bg-purple">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad nobis numquam rem voluptas voluptates? A accusantium aliquid beatae, commodi eos eveniet excepturi illum iusto magnam, nam nulla omnis recusandae sapiente.</div></el-col>
            <el-col :xs="8" :sm="6" :md="4" :lg="3"><div class="grid-content bg-purple-light">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad excepturi hic neque possimus velit! Blanditiis commodi, earum est exercitationem magni necessitatibus quidem quisquam quo saepe ut! Consequuntur dicta laboriosam ratione?</div></el-col>
        </el-row>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                msg: 'Use Vue 2.0 Today!'
            }
        },

        methods: {
            startHacking () {
                this.$notify({
                    title: 'It Works',
                    message: 'We have laid the groundwork for you. Now it\'s your time to build something epic!',
                    duration: 6000
                })
            }
        }
    }
</script>

<style>
    body {
        font-family: Helvetica, sans-serif;
    }
</style>
