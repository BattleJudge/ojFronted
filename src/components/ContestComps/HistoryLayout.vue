<template>
    <div class="layout">
        <Layout> <!-- 头部（默认的还没改 -->
            <Header class="layout-head" :style="{position: 'fixed', width: '100%'}">
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <!--					<div class="layout-logo"></div>-->
                    <!--					<div class="layout-nav">-->
                    <!--						<MenuItem name="1">-->
                    <!--						<Icon type="ios-navigate"></Icon>-->
                    <!--						Item 1-->
                    <!--						</MenuItem>-->
                    <!--						<MenuItem name="2">-->
                    <!--						<Icon type="ios-keypad"></Icon>-->
                    <!--						Item 2-->
                    <!--						</MenuItem>-->
                    <!--						<MenuItem name="3">-->
                    <!--						<Icon type="ios-analytics"></Icon>-->
                    <!--						Item 3-->
                    <!--						</MenuItem>-->
                    <!--						<MenuItem name="4">-->
                    <!--						<Icon type="ios-paper"></Icon>-->
                    <!--						Item 4-->
                    <!--						</MenuItem>-->
                    <!--					</div>-->
                </Menu>
            </Header>
            <!-- 主体 -->
            <Content class="layout-content" :style="{margin: '78px 10px 0', background: '#fff', minHeight: '650px'}">
                <slot></slot> <!-- 插入分割面板 -->
            </Content>
        </Layout>
    </div>
</template>

<script>

    export default {
        name: 'HistoryLayout',
        components: {},

    }
</script>

<style scoped>
    .layout {
        border: 1px solid #d7dde4;
        background: #f5f7f9;
        position: relative;
        border-radius: 4px;
        overflow: hidden;

    }

    .layout-head {
        z-index: 15;
    }

    .layout-logo {
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
    }

    .layout-nav {
        width: 420px;
        margin: 0 auto;
        margin-right: 20px;
    }

    .layout-content {
    }
</style>
