<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <Nuxt-link class="navbar-brand" href="#">Testサイト</Nuxt-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <Nuxt-link class="nav-link" activeClass="active" aria-current="page" href="/">Home</Nuxt-link>
        </li>
        <li class="nav-item">
          <Nuxt-link class="nav-link" activeClass="active" href="/secondpage">secondpage</Nuxt-link>
        </li>
        <li class="nav-item">
          <Nuxt-link class="nav-link" activeClass="active" href="/fishdata">fishdata</Nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
    </div>
</template>