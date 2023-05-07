<<<<<<< HEAD
<script>
    import Navbar from "./Navbar.svelte";
</script>

<Navbar />
<div class="container">
    </slot />
</div>
=======
<nav>
        <h1>Start Bootstrap</h1>
    <ul>
        <li>
            <a href="/">Home</a>
        </li>
        <li>
            <a href="/about">About</a>
        </li>
        <li>
            <a href="/services">Services</a>
        </li>
        <li>
            <a href="/contact">Contact</a>
        </li>
    </ul>
</nav>

<slot />

<style>
    nav {
        display: flex;
        background-color: #212529;
        color: white;
    }
    ul {
        display: flex;
        margin: 0;
        margin-left: auto;
        list-style: none;
    }
    li {
        margin-right: 20px;
    }
    h1 {
        margin: 0;
        font-size: 1em;
        font-weight: normal;
    }
    a {
       text-decoration: none;
       color: white; 
    }
</style>

>>>>>>> parent of 459a3c2 (tutorial part 2 done)
