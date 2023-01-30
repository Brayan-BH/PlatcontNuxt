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
                                Fechas de facturación
                                <i class="material-icons">
                                    fact_check
                                </i>
                            </button>
                        </p>
                    </div>
                    <div class="body-card">
                        <div class="body-content">
                            <div :class="[(interaction.drop == 2) ? 'drop-show' : 'drop-hide']">
                                <p class="main-title">Smith Adam jhonson De la torre</p>
                                <p class="sub-title">Pequeña Empresa</p>
                                <p class="sub-title">Mediana Empresa</p>
                                <div class="importe">
                                    <span>S./</span>
                                    <span class="display-1">1000</span>
                                    <span>total</span>
                                </div>
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
                    <div class="container-table">
                        <table>
                            <tr>
                                <th>Factura</th>
                                <th>Cliente</th>
                                <th>Fecha</th>
                                <th>Importe</th>
                            </tr>
                            <tr>
                                <td>Pequeña Empresa</td>
                                <td>Smith Adam jhonson De la torre</td>
                                <td>30/09/2021</td>
                                <td>S/. 250</td>
                            </tr>
                            <tr>
                                <td>Pequeña Empresa</td>
                                <td>Smith Adam jhonson De la torre</td>
                                <td>30/10/2021</td>
                                <td>S/. 250</td>
                            </tr>
                            <tr>
                                <td>Pequeña Empresa</td>
                                <td>Smith Adam jhonson De la torre</td>
                                <td>30/11/2021</td>
                                <td>S/. 250</td>
                            </tr>
                            <tr>
                                <td>Mediana Empresa</td>
                                <td>Smith Adam jhonson De la torre</td>
                                <td>30/12/2021</td>
                                <td>S/. 250</td>
                            </tr>
                            <tr>
                                <td>Mediana Empresa</td>
                                <td>Smith Adam jhonson De la torre</td>
                                <td>30/01/2022</td>
                                <td>S/. 250</td>
                            </tr>
                        </table>
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
            <div :class="[(interaction.drop == 4) ? 'drop-show-section' : 'drop-hide-section']">
                <div class="container-table">
                    <table>
                        <tr>
                            <th>Detalles</th>
                            <th>Precio</th>
                            <th>Importe</th>
                            <th>total</th>
                            <th></th>
                        </tr>
                        <tr>
                            <td>Pequeña Empresa</td>
                            <td>Smith Adam jhonson De la torre</td>
                            <td>30/09/2021</td>
                            <td>S/. 250</td>
                            <td class="pay">Pagado</td>
                        </tr>
                        <tr>
                            <td>Pequeña Empresa</td>
                            <td>Smith Adam jhonson De la torre</td>
                            <td>30/10/2021</td>
                            <td>S/. 250</td>
                            <td class="pay">Pagado</td>
                        </tr>
                        <tr>
                            <td>Pequeña Empresa</td>
                            <td>Smith Adam jhonson De la torre</td>
                            <td>30/11/2021</td>
                            <td>S/. 250</td>
                            <td class="pay">Pagado</td>
                        </tr>
                        <tr>
                            <td>Pequeña Empresa</td>
                            <td>Smith Adam jhonson De la torre</td>
                            <td>30/12/2021</td>
                            <td>S/. 250</td>
                            <td class="not-pay">No pagado</td>
                        </tr>
                        <tr>
                            <td>Pequeña Empresa</td>
                            <td>Smith Adam jhonson De la torre</td>
                            <td>30/01/2022</td>
                            <td>S/. 250</td>
                            <td class="not-pay">No pagado</td>
                        </tr>
                    </table>
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