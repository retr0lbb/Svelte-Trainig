<script>
    import "../styles/global.css"
</script>

<header class="nav">
    <div class="logo">
        <a href="/">Poké-Api</a>
    </div>
    <ul class="list">
        <li><a href="/details">Details</a></li>
        <li><a href="/render">render</a></li>
    </ul>
</header>
<main class="content">
    <!--page conternt-->
    <slot></slot>
</main>


<style>
    .content{
        width: 100%;
        height: 90vh;
        background-color: rgb(11, 0, 22);
    }
    a{
        text-decoration: none;
        color: inherit;
    }
    .nav{
        width: 100%;
        height: 10vh;
        background-color: rgb(21, 21, 21);
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 40px 10px 40px;
    }
    .list{
        list-style: none;
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        gap: 10px;
        color: white;
        font-size: 22px;
        height: 100%;
    }
    .list li{
        display: grid;
        place-items: center;
        cursor: pointer;
        width: 100%;
        padding: 0px 20px;
        height: 100%;
        transition: all .1s ease-in-out;
    }
    li:hover{
        transform: scale(1.05);
        color: rgb(209, 215, 92);
    }
    .logo{
        color: rgb(226, 226, 226);
        font-size: 2rem;
        font-family: sans-serif;
        font-weight: bold;
        cursor: pointer;
        transition: all .1s ease-in-out;
    }
    .logo:hover{
        transform: scale(1.05);
        color: rgb(209, 215, 92);
    }
</style>