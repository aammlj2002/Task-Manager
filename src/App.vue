<template>
    <div class="container">
        <div class="layout-grid">
            <div class="navbar">
                <Navbar />
            </div>
            <div class="left-sidebar">
                <LeftSideBar />
            </div>
            <div class="main">
                <router-view />
            </div>
            <div class="footer">
                <Footer />
            </div>
        </div>
    </div>
</template>

<script>
import Footer from './components/Footer'
import LeftSideBar from './components/LeftSideBar'
import Navbar from './components/Navbar'
export default {
    components: {
        Footer,
        LeftSideBar,
        Navbar
    },
}
</script>

<style>
.layout-grid {
    /* height: 100%; */
    display: grid;
    grid-template: 12vh 80vh 8vh / 1fr 4fr;
}
.navbar {
    background: #ffffff;
    border-bottom: 2px solid #01b7ff;
    grid-area: 1 / 1 / 2 / 3;

    display: flex;
    align-items: center;
    justify-content: left;
}
.left-sidebar {
    background: #f5f5f5;
    border-right: 2px solid #01b7ff;
    grid-area: 2 / 1 / 4 / 2;
    overflow-y: auto;
}
.main {
    background: #ffffff;
    grid-area: 2 / 2 / 3 / 3;
    overflow-y: auto;
    padding: 10px;
}
.footer {
    background: #01b7ff;
    grid-area: 3 / 2 / 4 / 3;

    display: flex;
    align-items: center;
    justify-content: center;
}
</style>
