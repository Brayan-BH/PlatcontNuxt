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
                                    de tu proyecto <br> y te acompañamos en tu crecimiento</p><a><button
                                        class="button-clasic" type="button" role="button">Contactanos</button></a>
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
                    <div class="tabs">
                        <!-- Dropdawn -->
                        <h2>Mantente conectado y completa tareas con Platcont</h2>
                        <div class="container-tabs">
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(1)">
                                    <i class="material-icons">
                                        account_balance
                                    </i>
                                    Financiera
                                </button>
                                <div :class="[(interaction.tab == 1) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(2)">
                                    <i class="material-icons">
                                        account_balance_wallet
                                    </i>
                                    Contabilidad
                                </button>
                                <div :class="[(interaction.tab == 2) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(3)">
                                    <i class="material-icons">
                                        admin_panel_settings
                                    </i>
                                    Recursos Humanos
                                </button>
                                <div :class="[(interaction.tab == 3) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(4)">
                                    <i class="material-icons">
                                        inventory
                                    </i>
                                    Stock
                                </button>
                                <div :class="[(interaction.tab == 4) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(5)">
                                    <i class="material-icons">
                                        local_taxi
                                    </i>
                                    Taxi
                                </button>
                                <div :class="[(interaction.tab == 5) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(6)">
                                    <i class="material-icons">
                                        directions_car
                                    </i>
                                    Transportes
                                </button>
                                <div :class="[(interaction.tab == 6) ? 'show' : 'hide']">
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(7)">
                                    <i class="material-icons">
                                        payments
                                    </i>
                                    Costos
                                </button>
                                <div :class="[(interaction.tab == 7) ? 'show' : 'hide']">
                                    <p>
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    </p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                            <div class="dropdawn-container">
                                <button class="button-clasic-white" type="button" role="button" @click="tabClick(8)">
                                    <i class="material-icons">
                                        monetization_on
                                    </i>
                                    Activos Fijos
                                </button>
                                <div :class="[(interaction.tab == 8) ? 'show' : 'hide']">
                                    <p>
                                    <p>Lorem commodo ad aute ea do occaecat elit nulla voluptate laboris non anim
                                        commodo.Sunt sit ipsum deserunt deserunt irure ad. Dolor sint dolor commodo
                                        pariatur
                                        consequat enim laboris laborum tempor sit ipsum eiusmod cillum ea. In minim
                                        deserunt
                                        veniam amet incididunt est officia aliquip est est. Ea reprehenderit quis magna
                                        cupidatat et consequat. Ad cillum voluptate veniam cupidatat. Laborum pariatur
                                        non
                                        adipisicing labore sit veniam velit et officia tempor culpa pariatur.</p>
                                    </p>
                                    <img src="/img/platcont-view.png">
                                </div>
                            </div>
                        </div>
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