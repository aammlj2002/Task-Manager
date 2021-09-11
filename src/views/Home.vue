<template>
    <h2 class="task-list-header">Go to school</h2>
    <div class="add-task">
        <span class="material-icons-outlined add-icon">add_circle_outline</span>
        <input type="text" placeholder="add new task" />
    </div>
    <div class="task-list">
        <div class="task">
            School
            <span class="material-icons-outlined task-icon">edit</span>
            <span class="material-icons-outlined task-icon">delete</span>
            <span class="material-icons-outlined task-icon">circle</span>
        </div>
        <div class="task">
            School
            <span class="material-icons-outlined task-icon">edit</span>
            <span class="material-icons-outlined task-icon">delete</span>
            <span class="material-icons-outlined task-icon">check_circle</span>
        </div>
    </div>
</template>

<script>
export default {
}
</script>
<style scoped>
.task-list-header {
    text-align: center;
    font-size: 110%;
}
.task {
    padding: 5px 7px;
    display: flex;
    align-items: center;
    justify-content: left;
}
.task-icon {
    margin-left: 10px;
    cursor: pointer;
    user-select: none;
}
.add-task {
    margin-bottom: 10px;
    display: flex;
    align-items: center;
}
.add-icon {
    margin-right: 10px;
    user-select: none;
    cursor: pointer;
}
input {
    border: none;
}
</style>