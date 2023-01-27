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
                    <!-- <div class="footer-card">
                        <button class="btn-actualizar" @click="">Actualizar</button>
                    </div> -->
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
                    <!-- <div class="footer-card">
                        <button class="btn-actualizar">Actualizar</button>
                    </div> -->
                </div>
            </div>
            <!-- Contraseña\ -->
            <!-- <div class="info-3">
                <div class="container-button-pass">
                    <p class="text-title before">
                        <button class="button-pass" type="button" role="button" @click="dropClick(3)">
                            Cambiar Contraseña
                            <i class="material-icons">
                                key
                            </i>
                        </button>
                    </p>
                </div>
            </div> -->
        </div>
        <!-- Section Dash -->
        <div class="container-dashboard">
            <div class="container-cards">
                <div class="cards-items">
                    <div class="items" @click="dropClick(1)">
                        <p class="number">1</p>
                        <i class="material-icons">
                            person
                        </i>
                        <p class="sub">Editar Información</p>
                    </div>
                    <div class="items" @click="dropClick(2)">
                        <p class="number">2</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Fechas de Facturación</p>
                    </div>
                    <div class="items" @click="dropClick(3)">
                        <p class="number">3</p>
                        <i class="material-icons">
                            key
                        </i>
                        <p class="sub">Cambiar Contraseña</p>
                    </div>
                    <div class="items column-3" @click="dropClick(4)">
                        <p class="number">4</p>
                        <i class="material-icons">
                            settings
                        </i>
                        <p class="sub">Facturas</p>
                    </div>
                </div>
                <!-- Actualizar informacion -->
                <div :class="[(interaction.drop == 1) ? 'drop-show-section' : 'drop-hide-section']">
                    <div class="section-show">
                        <div class="body-section">
                            <div class="section-items">
                                <label>Nombres y Apellidos</label>
                                <input class="input-name" type="text" placeholder="Apellidos y Nombres">
                            </div>
                            <div class="section-items">
                                <label>Dirección</label>
                                <input class="input-direc" name="direccion" type="text" placeholder="Dirección Actual">
                            </div>
                        </div>
                        <div class="footer-section">
                            <button class="btn-footer">
                                Actualizar
                                <i class="material-icons">
                                    change_circle
                                </i>
                            </button>
                        </div>
                    </div>
                </div>
                <!-- Actualizar Informacion 2 -->
                <div :class="[(interaction.drop == 2) ? 'drop-show-section' : 'drop-hide-section']">
                    <div class="section-show">
                        <div class="body-section">
                            <div class="section-items">
                                <label>Contraseña Actual(*)</label>
                                <input class="input-pass" type="text" placeholder="Contraseña Actual">
                            </div>
                            <div class="section-items">
                                <label>Contraseña Nueva(*)</label>
                                <input class="input-pass" name="password" type="text" placeholder="Contraseña Nueva">
                            </div>
                            <div class="section-items">
                                <label>Repetir Contraseña(*)</label>
                                <input class="input-pass" name="password" type="text" placeholder="Repetir Contraseña">
                            </div>
                        </div>
                        <div class="footer-section">
                            <button class="btn-footer">
                                Actualizar
                                <i class="material-icons">
                                    change_circle
                                </i>
                            </button>
                        </div>
                    </div>
                </div>
                <!-- Actualizar contraseña -->
                <div :class="[(interaction.drop == 3) ? 'drop-show-section' : 'drop-hide-section']">
                    <div class="section-show">
                        <div class="body-section">
                            <div class="section-items">
                                <label>Contraseña Actual(*)</label>
                                <input class="input-pass password1" type="password" placeholder="Contraseña Actual">
                                <i class="material-icons" @click="showPass1()">
                                    visibility
                                </i>
                            </div>
                            <div class="section-items">
                                <label>Contraseña Nueva(*)</label>
                                <input class="input-pass password2" name="password" type="password"
                                    placeholder="Contraseña Nueva">
                                <i class="material-icons" @click="showPass2()">
                                    visibility
                                </i>
                            </div>
                            <div class="section-items">
                                <label>Repetir Contraseña(*)</label>
                                <input class="input-pass password3" name="password" type="password"
                                    placeholder="Repetir Contraseña">
                                <i class="material-icons" @click="showPass3()">
                                    visibility
                                </i>
                            </div>
                        </div>
                        <div class="footer-section">
                            <button class="btn-footer">
                                Actualizar
                                <i class="material-icons">
                                    change_circle
                                </i>
                            </button>
                        </div>
                    </div>
                </div>
                <!-- Ver Facturas -->
                <div class="container-table">
                    <div :class="[(interaction.drop == 4) ? 'drop-show-section' : 'drop-hide-section']">

                        <table class="container">
                            <thead>
                                <tr>
                                    <th>
                                        <h1>Modulos</h1>
                                    </th>
                                    <th>
                                        <h1>Precio</h1>
                                    </th>
                                    <th>
                                        <h1>Total</h1>
                                    </th>
                                    <th>
                                        <h1>Lorem</h1>
                                    </th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>951</td>
                                    <td>636</td>
                                    <td>Pagado</td>
                                </tr>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>732</td>
                                    <td>104</td>
                                    <td>Pagado</td>
                                </tr>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>416</td>
                                    <td>532</td>
                                    <td>Pagado</td>
                                </tr>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>365</td>
                                    <td>296</td>
                                    <td> No Pagado</td>
                                </tr>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>200</td>
                                    <td>413</td>
                                    <td>No Pagado</td>
                                </tr>
                                <tr>
                                    <td>Pequeña Empresa</td>
                                    <td>462</td>
                                    <td>348</td>
                                    <td>No Pagado</td>
                                </tr>
                            </tbody>
                        </table>
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
        },
        showPass1() {
            const password1 = document.querySelector(".password1");
            const type1 = password1.getAttribute("type") === "password" ? "text" : "password";
            password1.setAttribute("type", type1);
        },
        showPass2() {
            const password2 = document.querySelector(".password2");
            const type2 = password2.getAttribute("type") === "password" ? "text" : "password";
            password2.setAttribute("type", type2);
        },
        showPass3() {

            const password3 = document.querySelector(".password3");
            const type3 = password3.getAttribute("type") === "password" ? "text" : "password";
            password3.setAttribute("type", type3);
        }
    }
}
</script>