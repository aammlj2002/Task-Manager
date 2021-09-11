<template>
    <form class="add-task-list">
        <span class="material-icons-outlined">add_circle_outline</span>
        <input type="text" placeholder="add new task list" />
    </form>
    <div>
        <router-link to="/">Going to school</router-link>
        <router-link to="/">Going to school</router-link>
        <router-link to="/">Going to school</router-link>
        <router-link to="/">Going to school</router-link>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.add-task-list {
    max-width: 100%;
    padding: 5px 10px;
    display: flex;
    align-items: center;
    justify-content: left;
}
input {
    width: 200px;
    border: none;
    background: transparent;
}
a {
    text-decoration: none;
    display: block;
    padding: 7px 13px;
    transition: all 0.2s;
}
a:hover,
a:active {
    color: #01b7ff;
}
span {
    margin-right: 5px;
    cursor: pointer;
    user-select: none;
}
</style>