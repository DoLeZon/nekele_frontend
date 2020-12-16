<template>
    <header class="header-global">
        <base-nav class="navbar-main" transparent type="" effect="light" expand>
            <router-link slot="brand" class="navbar-brand" to="/">
                <img src="img/brand/logo_nekele.png" width="200" alt="logo">
            </router-link>

            <!-- <div class="row" slot="content-header" slot-scope="{closeMenu}">
                <div class="col-6 collapse-brand">
                    <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/">
                        <img src="img/brand/blue.png">
                    </a>
                </div>
                <div class="col-6 collapse-close">
                    <close-button @click="closeMenu"></close-button>
                </div>
            </div> -->

            <ul class="navbar-nav navbar-nav-hover align-items-lg-center">
                <base-dropdown class="nav-item" menu-classes="dropdown-menu-xl">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-ui-04 d-lg-none"></i>
                        <span class="nav-link-inner--text">Comment ça fonctionne</span>
                    </a>
                    <div class="dropdown-menu-inner">
                        <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/"
                           class="media d-flex align-items-center">
                            <div class="icon icon-shape bg-gradient-primary rounded-circle text-white">
                                <i class="ni ni-spaceship"></i>
                            </div>
                            <div class="media-body ml-3">
                                <h6 class="heading text-primary mb-md-1">Travailler en tant que Freelance</h6>
                                <p class="description d-none d-md-inline-block mb-0">Créer un compte et commencer à gagner de l'argent depuis chez vous en travaillant selon se vos propres horaires.</p>
                            </div>
                        </a>
                        <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/"
                           class="media d-flex align-items-center">
                            <div class="icon icon-shape bg-gradient-warning rounded-circle text-white">
                                <i class="ni ni-ui-04"></i>
                            </div>
                            <div class="media-body ml-3">
                                <h5 class="heading text-warning mb-md-1">Embaucher un Freelance</h5>
                                <p class="description d-none d-md-inline-block mb-0">Créer un compte et trouver les talents nécéssaires à la réalisation de votre projet.</p>
                            </div>
                        </a>
                    </div>
                </base-dropdown>
                <li class="nav-item d-none d-lg-block ml-lg-4">
                    <router-link slot="brand" to="/">
                        <span class="nav-link-inner--text">Nos offres</span>
                    </router-link>
                </li>
            </ul>
            <ul class="navbar-nav align-items-lg-center ml-lg-auto">
                
                <li class="nav-item d-none d-lg-block ml-lg-4">
                    <router-link slot="brand" class="btn btn-success btn-icon" to="/login">
                        <span class="btn-inner--icon">
                            <i class="fa fa-sign-in mr-2"></i>
                        </span>
                        <span class="nav-link-inner--text">Connexion</span>
                    </router-link>
                </li>

                <li class="nav-item d-none d-lg-block ml-lg-4">
                    <router-link slot="brand" class="btn btn-neutral btn-icon" to="/register">
                        <span class="btn-inner--icon">
                            <i class="fa fa-user mr-2"></i>
                        </span>
                        <span class="nav-link-inner--text">Inscription</span>
                    </router-link>
                </li>
            </ul>
        </base-nav>
    </header>
</template>
<script>
import BaseNav from "@/components/BaseNav";
import BaseDropdown from "@/components/BaseDropdown";
import CloseButton from "@/components/CloseButton";

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown
  }
};
</script>
<style>
</style>
