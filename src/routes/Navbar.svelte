<script>
   import { page } from "$app/stores";
   
   const navs = [
    {
        title:"Home",
        href: "/",
    },
    {
        title:"About",
        href: "/about",
    },
    {
        title:"Services",
        href: "/services",
    },
    {
        title:"Contact",
        href: "/contact",
    },
   ]


   $: routId = $page.route.id;  
</script>

<nav>
    <div class="container">
        <h1>Start Bootstrap</h1>
        <ul>
            {#each navs as {title, href}}
              <li>
                <a {href} class:active={routeId == href} {titel}>{title}</a>
              </li>
            {/each}
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
        align-items: center;
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
       color: white#ddd;
    }
    .active {
        color: white;
    }
</style>