<template>
    <div id="footer">
        <p>Make Your Burger &copy; 2022</p>
        <p>phone: (16) 99377-7570</p>
    </div>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped>
    #footer {
        height: 200px;
        background: #222;
        border-top: 4px solid #111;
        color: #fcba03;
        display: flex;
        align-items: center;
        justify-content: space-around;
        padding: 30px 50px;
        width: 100%;
        position: relative;
    }
</style>