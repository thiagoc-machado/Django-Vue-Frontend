<template>
    <div class="container">
        <nav class="navbar navbar-expand-lg bg-body-tertiary">
            <div class="container-fluid">
                <button
                    class="navbar-toggler"
                    type="button"
                    data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent"
                    aria-controls="navbarSupportedContent"
                    aria-expanded="false"
                    aria-label="Toggle navigation"
                >
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div
                    class="collapse navbar-collapse"
                    id="navbarSupportedContent"
                >
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <router-link
                                class="nav-link active"
                                aria-current="page"
                                to="/"
                                >Home</router-link
                            >
                        </li>
                        <li class="nav-item">
                            <router-link class="nav-link" to="/about"
                                >Acerca de nosotros</router-link
                            >
                        </li>
                    </ul>
                    <form class="d-flex" role="search" action="">
                        <input
                            class="form-control me-2"
                            type="search"
                            placeholder="Buscar"
                            aria-label="Search"
                        />
                        <button class="btn btn-outline-success" type="submit">
                            Buscar
                        </button>
                    </form>
                </div>
            </div>
        </nav>
    </div>
    <router-view />

    <footer class="text-center py-4 my-4 border-top">
        <p>&copy; 2024 Thiago Machado</p>
    </footer>
</template>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}

nav {
    padding: 30px;
}

nav a {
    font-weight: bold;
    color: #2c3e50;
}

nav a.router-link-exact-active {
    color: #42b983;
}
</style>
