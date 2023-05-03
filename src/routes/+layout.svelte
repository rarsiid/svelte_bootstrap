<nav>
    <div class="container">

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
    </div>
</nav>

<div class="container"> 
    <slot />
</div>

<style>
    nav {
        padding: 0.5em;
        background-color: #343a40;
        color: white;
    }

    .container {
        display: flex;
    }

    ul {
        display: flex;
        margin: 0;
        margin-left: auto;
        list-style: none;
        font-size: 0.9em;
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

