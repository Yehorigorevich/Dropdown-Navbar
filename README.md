# Dropdown-Navbar
# HTML

<body>
<nav role="navigation">
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#" aria-haspopup="true">Portfolio</a>
            <ul class="dropdown" aria-label="submenu">
                <li><a href="#">Web</a></li>
                <li><a href="#" aria-haspopup="true">UI</a>
                    <ul class="dropdown" aria-label="submenu">
                        <li><a class="sub" href="#">User</a></li>
                        <li><a class="sub" href="#">Interface</a></li>
                    </ul>
                </li>
                <li><a href="#">UX</a></li>
            </ul>
        </li>
        <li><a href="#">Contact</a></li>
    </ul>
</nav>
<section class="section-1">
    <div class="container">
        <div class="box"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Earum praesentium ea sit. Magnam numquam reiciendis iure. Corrupti modi vero similique veniam magni, eius cum nemo beatae maiores assumenda. Sint nihil magni nulla iure, dolor tempora voluptatem eos assumenda soluta nisi molestiae repudiandae! Assumenda architecto error, aliquid, porro illum laboriosam maxime.</p></div>
        <div class="box"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Atque eligendi quaerat quidem, facere rerum accusamus sed aspernatur ea dolore laboriosam, doloremque nam sit! Tempore iure fuga expedita eaque ad, error, dolor vitae totam reprehenderit corporis nulla ab debitis odio incidunt laborum quasi minima voluptate nisi saepe quo ipsam nostrum suscipit?</p></div>
        <div class="box"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eius sequi quo repellendus ullam assumenda saepe porro ipsa eveniet reiciendis fugiat minima libero, perspiciatis at consequatur nemo quam! Beatae ea itaque atque, repudiandae voluptates dolore, dicta culpa nemo eaque nisi esse facere quidem modi exercitationem nulla dolores. Illum dolorem repellendus minima?</p></div>
    </div>
</section>
</body>

# CSS

body {width:100%; height: 100%; margin: 0px;}
*{
    box-sizing: border-box
}
a {
    text-decoration: none;
    text-align: center;
    }

nav {
    font-family: "Space Mono";
    background: black;
    }

ul {
    background: black;
    list-style: none;
    margin: 0;
    padding-left: 0;
    }

li {
    color: #fff;
    background: black;
    display: block;
    float: right;
    padding: 1rem;
    position: relative;
    text-decoration: none;
    transition-duration: 0.5s;
    }

li a {
    color: #fff;
    text-align : center;
    }

li:hover,
li:focus-within {
    background: white;
    color: black;
    cursor: pointer;
    }

li:focus-within a {
    outline: none;
    color: black;
    }

ul li ul {
    background: black;
    visibility: hidden;
    opacity: 0;
    min-width: 5rem;
    position: absolute;
    transition: all 0.5s ease;
    margin-top: 1rem;

    left: 0;
    display: none;
    }

ul li:hover > ul,
ul li:focus-within > ul,
ul li ul:hover,
ul li ul:focus {
    visibility: visible;
    opacity: 1;
    display: block;
    }

ul li ul li {
    clear: both;
    width: 100%;
    }
