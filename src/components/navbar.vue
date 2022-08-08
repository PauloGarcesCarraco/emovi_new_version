<template>
<div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><img src="../../src/assets/images/LogoEMOVI-head-retina.png" width=" 250"></a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="index.html">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="galeria.html">Galeria</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" style="color: white" href="#" id="navbarDropdown"
                            role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Noticias & STATS
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><a class="dropdown-item" href="americas.html">Americas</a></li>
                            <li><a class="dropdown-item"
                                    href="http://en.caam.org.cn/Index/lists/catid/54.html">China</a></li>
                            <li><a class="dropdown-item"
                                    href="https://www.acea.auto/fuel-pc/fuel-types-of-new-cars-battery-electric-7-5-hybrid-19-3-petrol-41-8-market-share-in-q2-2021/">EU+EFTA</a>
                            </li>
                            <li><a class="dropdown-item" href="ElMundo.html">El Mundo</a></li>
                            <li>
                                <hr class="dropdown-divider">
                            </li>
                            <li><a class="dropdown-item"
                                    href="chile.html">Chile</a></li>
                        </ul>
                    </li>
                </ul>
                <form class="d-flex">
                    <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-outline-success" type="submit">Search</button>
                </form>
            </div>
        </div>
    </nav>
</div>
</template>
<script>
export default {
  name: 'navbar-emovi',
  props: {
  }
}
</script>
<style scoped>
nav{
    margin-top: 0;
    text-align: center;
    padding-left: 10%;
}

</style>