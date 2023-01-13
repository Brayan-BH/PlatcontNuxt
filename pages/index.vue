<template>
    <main>
        <!-- Plactont info -->
        <main>
            <div class="main-head">
                <div class="head-banner">
                    <p class="banner__text">
                        La aplicación Office se está convirtiendo en la nueva aplicación de Microsoft 365, su lugar para
                        buscar, crear
                        y compartir su contenido e ideas.
                    </p>
                    <p class="banner__link">
                        <span class="link__text">Obtener más información</span>
                        <span class="link__icon material-icons">navigate_next</span>
                    </p>
                </div>
                <div class="head-img">
                    <div class="img__gradient"></div>
                </div>
                <div class="head-detail">
                    <div class="main-container">
                        <div class="container-content">
                            <div class="text">
                                <h1>Platcont</h1>
                                <p>PLATCONT es más que un software. De la mano con un servicio <br> permanente de
                                    soporte, aseguramos el
                                    éxito
                                    de tu proyecto <br> y te acompañamos en tu crecimiento</p>
                                <a>
                                    <button class="button-clasic" type="button" role="button">
                                        Contactanos
                                    </button>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </main>
        <!-- Que es Platcont -->
        <div class="container-section-tabs">
            <div class="main-tabs">
                <div class="content-consumer">
                    <div>
                        <h2 class="tab-header">¿Qué es Platcont?</h2>
                        <p class="tab-subheader">PLATCONT es un sistema de gestión empresarial, que permite integrar
                            todos
                            los procesos internos
                            de tu organización, haciéndolas más eficientes. Al implementar PLATCONT, lograrás en corto
                            tiempo tener el total control de tu negocio, contando con información exacta, precisa y a
                            tiempo; lo que facilitará una mejor toma de decisiones.</p>
                    </div>
                    <!-- Caracteristicas -->
                    <div class="container-caracteristicas">
                        <div class="container-row">
                            <div class="space">
                                <div class="efect-hover">
                                    <i class="material-icons">
                                        groups
                                    </i>
                                    <h2 class="">Soporte Personalizado</h2>
                                </div>
                                <p>Atención permanente para ayudarlos desde el primer día.</p>
                            </div>
                            <div class="space">
                                <div class="efect-hover">
                                    <i class="material-icons efect-hover">
                                        settings
                                    </i>
                                    <h2 class="">Flexible</h2>
                                </div>
                                <p>Desarrollamos mejoras o nuevos módulos integrándolas con el sistema.</p>
                            </div>
                            <div class="space">
                                <div class="efect-hover">
                                    <i class="material-icons">
                                        devices
                                    </i>
                                    <h2 class="">Rápida Implementación</h2>
                                </div>
                                <p>En pocas semanas contarás con Platcont funcionando en tu empresa.</p>
                            </div>
                            <div class="space column-2">
                                <div class="efect-hover">
                                    <i class="material-icons">
                                        send
                                    </i>
                                    <h2 class="">Fácil de Usar</h2>
                                </div>
                                <p>Gracias a su interfaz amigable, no requiere de experiencia en uso de otros sistemas
                                    empresariales.</p>
                            </div>
                        </div>
                    </div>
                    <!-- tabs -->

                    <ModulosView/>

                    <modulos/>
                    <!-- Precios -->
                    <div class="layout-main">
                        <div class="layout-header">
                            <h2>
                                Buscar un Plan
                            </h2>
                            <p>
                                Tanto si quieres conectarte con familiares y amigos, como aprender de forma remota o
                                colaborar con tu equipo, hay un plan de Microsoft 365 que satisface tus necesidades.
                            </p>
                        </div>
                        <PreciosView/>
                    </div>

                </div>
            </div>
        </div>
    </main>

</template>

<script>

export default {
    name: "Navbar",
    mounted() {

    },
    data() {
        return {
            interaction: {
                tab: 0
            }
        }
    },
    methods: {
        tabClick(index) {
            if (index == this.interaction.tab) this.interaction.tab = 0
            else this.interaction.tab = index
        }
    }
}

</script>