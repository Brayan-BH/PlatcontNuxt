<template>
    <div class="cuenta">
        <div class="container-information">

            <div class="info-1">
                <div class="container-card">
                    <div class="header-card">
                        <p class="header-title before">
                            <button class="title-btn" type="button" role="button" @click="dropClick(1)">
                                Su Información
                                <i class="material-icons">
                                    person
                                </i>
                            </button>
                        </p>
                    </div>
                    <div class="body-card">
                        <div class="body-content">
                            <div :class="[(interaction.drop == 1) ? 'drop-show' : 'drop-hide']">
                                <p class="main-title">Basurto Huamán Brayan</p>
                                <p>Av. Ocopilla 660
                                </p>
                                <p>huancayo, junin, 1800</p>
                                <p>Perú</p>
                            </div>
                        </div>
                    </div>
                    <div class="footer-card">
                        <button class="btn-actualizar">Actualizar</button>
                    </div>
                </div>
            </div>
            <div class="info-2">
                <div class="container-card">
                    <div class="header-card">
                        <p class="header-title before">
                            <button class="title-btn" type="button" role="button" @click="dropClick(2)">
                                Su Información
                                <i class="material-icons">
                                    person
                                </i>
                            </button>
                        </p>
                    </div>
                    <div class="body-card">
                        <div class="body-content">
                            <div :class="[(interaction.drop == 2) ? 'drop-show' : 'drop-hide']">
                                <p class="main-title">Basurto Huamán Brayan</p>
                                <p>Av. Ocopilla 660
                                </p>
                                <p>huancayo, junin, 1800</p>
                                <p>Perú</p>
                            </div>
                        </div>
                    </div>
                    <div class="footer-card">
                        <button class="btn-actualizar">Actualizar</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- Section Dash -->
        <div class="container-dashboard">
            <div class="container-cards">
                <div class="cards-items">
                    <div class="items">
                        <p class="number">1</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Items</p>
                    </div>
                    <div class="items">
                        <p class="number">2</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Items</p>
                    </div>
                    <div class="items">
                        <p class="number">3</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Items</p>
                    </div>
                    <div class="items column-3">
                        <p class="number">4</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Items</p>
                    </div>
                    <div class="items">
                        <p class="number">5 </p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Items</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "MiCuenta",
    mounted() {

    },
    data() {
        return {
            interaction: {
                drop: 0,
            }
        }
    },
    methods: {
        dropClick(index) {
            if (index == this.interaction.drop) this.interaction.drop = 0
            else this.interaction.drop = index
        }
    }
}
</script>