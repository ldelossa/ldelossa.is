<template>
        <div class="status-bar">
            <div class="left-status-bar">
                <div class="mode-indicator">
                    <span class="status-item">INSERT</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">master</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">|</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">
                        ~/webstuff/table_of_contents.html
                    </span>
                </div>
            </div>
            <div class="right-status-bar">
                <div class="default-indicator">
                    <span class="status-item">linux</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">|</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">utf8</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">|</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">html</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">37%</span>
                </div>
                <div class="default-indicator">
                    <span class="status-item">35:1</span>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: "StatusBar"
}
</script>

<style scoped>
.status-bar {
    font-size: 1.2vw;
    display: flex;
    height: 100%;
    justify-content: space-between;
    background-color: #363a3e;
    font-family: monaco,Consolas,Lucida Console,monospace;
    color: #AFB7C0
}
.left-status-bar {
    display: flex;
    justify-content: flex-start;
    align-items: flex-end;
    width: 50%
}
.right-status-bar {
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    width: 50%
}
.status-item {
    font-size: 1.2vw;
}
.default-indicator {
    padding: .8% .8% 0 .8%;
}
.mode-indicator {
    background-color: #759ABD;
    padding: .8% .8% 0 .8%;
}
</style>
