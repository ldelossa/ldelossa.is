<template>
    <div class="terminal-window">
        <div class="text-window">
            <pre>
 1 type TableOfContents struct {
 2     About about
 3     Projects projects
 4     Contact URL
 5 }
 6 
 7 type about struct {
 8     experience URL
 9     constributions URL
10 }
11  
12 type projects struct {
13    GraphX URL
14    OpenEdge URL
15    CSEC URL
16    CloudScale URL
17 }
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
            </pre>
        </div>
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
    </div>
</template>

<script>
export default {
    name: "TerminalWindow"
}
</script>

<style scoped>
.terminal-window {
    height: 100%;
}
.text-window {
    font-family: monaco,Consolas,Lucida Console,monospace;
    height: calc(100% - 2vw);
    background-color: #e4e4e4;
    text-align: left;
}
.status-bar {
    font-size: 1.2vw;
    display: flex;
    height: 2vw;
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

