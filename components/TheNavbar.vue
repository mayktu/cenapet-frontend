<template>
  <nav class="navbar navbar-dark bg-dark navbar-expand-lg">
    <nuxt-link to="/" class="navbar-brand">
      <img src="@/assets/images/logo_claro.png" class="nav-image" />
    </nuxt-link>
    <button
      type="button"
      aria-label="Toggle navigation"
      aria-controls="nav-collapse"
      aria-expanded="false"
      data-toggle="collapse"
      data-target="#nav-collapse"
      class="navbar-toggler"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div id="nav-collapse" class="navbar-collapse collapse">
      <ul class="navbar-nav">
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >CENAPET</a>
          <div class="dropdown-menu" aria-labelledby="Menu cenapet">
            <nuxt-link class="dropdown-item" to="#">Sobre a diretoria</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Gestões</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Conselho</nuxt-link>
          </div>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >DOCUMENTOS</a>
          <div class="dropdown-menu" aria-labelledby="Menu documentos">
            <nuxt-link class="dropdown-item" to="#">Cartas</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Comissão Executiva</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Conselho</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">SESu/MEC</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Outros</nuxt-link>
          </div>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >PET</a>
          <div class="dropdown-menu" aria-labelledby="Menu PET">
            <nuxt-link class="dropdown-item" to="#">Grupos</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Orientações gerais</nuxt-link>
          </div>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >EVENTOS</a>
          <div class="dropdown-menu" aria-labelledby="Menu cenapet">
            <nuxt-link class="dropdown-item" to="#">Anais</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Histórico</nuxt-link>
            <nuxt-link class="dropdown-item" to="#">Organização</nuxt-link>
          </div>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="#">FORMULÁRIOS</nuxt-link>
        </li>
      </ul>
      <ul class="navbar-nav ml-auto">
        <div class="col-sm-6 col-lg-12">
          <div role="group" class="input-group">
            <input
              type="text"
              placeholder="Pesquisar"
              class="form-control"
              aria-label="Pesquisar no site"
            />
            <div class="input-group-append">
              <button type="submit" class="btn btn-secondary">
                <font-awesome-icon :icon="['fas', 'search']" />
              </button>
            </div>
          </div>
        </div>
      </ul>
    </div>
  </nav>
</template>

<style>
.navbar .navbar-dark .navbar-expand-lg {
  padding: 0.5rem 0.5rem;
}

.nav-image {
  max-height: 2.5rem;
}

.navbar-dark .navbar-nav .nav-item {
  padding: 0 0.5rem;
  margin: 0 0.7rem;
  letter-spacing: 1px;
  cursor: pointer;
}

.navbar-dark .navbar-nav .nav-link {
  color: var(--text-light1);
}

.navbar-dark .navbar-nav .dropdown-menu {
  min-width: 15rem;
  background-color: var(--theme-dark);
  padding-bottom: 0;
  border: none;
  border-radius: 0;
}

.navbar-dark .navbar-nav .dropdown-item {
  padding-top: 0.6rem;
  padding-bottom: 0.6rem;
  color: var(--text-light1);
}

.navbar-dark .navbar-nav .dropdown-item:hover,
.navbar-dark .navbar-nav .dropdown-item:focus {
  background-color: var(--highlight-dark);
  color: var(--text-light1);
}

.navbar-dark .navbar-nav .dropdown-header {
  color: var(--text-grey);
}

.navbar-dark .navbar-nav .dropdown-divider {
  border-color: var(--border-dark);
}

.navbar-nav .input-group input {
  border: none;
  box-shadow: none;
}

.navbar-nav .input-group .btn {
  background-color: transparent;
  border: none;
  box-shadow: none;
}

@media (max-width: 991px) {
  .navbar-dark .navbar-nav .dropdown-menu {
    border: 1px solid var(--border-dark);
    border-radius: 0.5rem;
    padding-bottom: 0.5rem;
  }

  .navbar-dark .navbar-nav .form-inline {
    margin-top: 0.3rem;
    flex-flow: unset;
  }

  .navbar-dark .navbar-nav .form-inline .form-control {
    margin-right: 0.5rem;
  }
}
</style>
