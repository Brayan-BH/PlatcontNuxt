<template>
    <div class="layout-container">
        <div class="container-card">
            <div class="container-card__items">
                <div class="item-card">
                    <div class="card">
                        <img class="card__img"
                            src="https://cdn-dynmedia-1.microsoft.com/is/image/microsoftcorp/personal-family?resMode=sharp2&amp;op_usm=1.5,0.65,15,0&amp;wid=1099&amp;hei=880&amp;qlt=75">
                        <div class="card__body orange">
                            <p class="body__title before">
                                <button class="title__btn" type="button" role="button" @click="collapseClick(1)">
                                    Pequeña Empresa
                                </button>
                            </p>
                            <div :class="[(interaction.collapse == 1) ? 'collapse-show' : 'collapse-hide']">
                                <div class="items__center">
                                    <p>Mantente al día con un plan para ti y para tu familia.</p>
                                </div>
                            </div>
                            <div class="items__link__group">
                                <a class="btn orange"
                                    href="https://www.microsoft.com/es/microsoft-365/explore-microsoft-365-for-home">
                                    Más información
                                </a>
                                <a class="btn__link"
                                    href="https://www.microsoft.com/es/microsoft-365/buy/compare-all-microsoft-365-products?tab=1">
                                    Ve los planes personales y familiares
                                </a>
                                <!--button/cta disclaimer-->
                            </div>
                        </div>
                    </div>
                </div>

                <div class="item-card">
                    <div class="card">
                        <img class="card__img"
                            src="https://cdn-dynmedia-1.microsoft.com/is/image/microsoftcorp/personal-family?resMode=sharp2&amp;op_usm=1.5,0.65,15,0&amp;wid=1099&amp;hei=880&amp;qlt=75">
                        <div class="card__body blue">
                            <p class="body__title">
                                <button class="title__btn" type="button" role="button" @click="collapseClick(2)">
                                    Mediana Empresa
                                </button>
                            </p>
                            <div :class="[(interaction.collapse == 2) ? 'collapse-show' : 'collapse-hide']">
                                <div class="items__center">
                                    <p>Permite que tus empleados con herramientas colaboren de forma segura y
                                        trabaja desde cualquier lugar.</p>
                                </div>
                            </div>
                            <div class="items__link__group">
                                <a class="btn blue"
                                    href="https://www.microsoft.com/es/microsoft-365/explore-microsoft-365-for-home">
                                    Más información
                                </a>
                                <a class="btn__link"
                                    href="https://www.microsoft.com/es/microsoft-365/buy/compare-all-microsoft-365-products?tab=1">
                                    Ve los planes personales y familiares
                                </a>
                                <!--button/cta disclaimer-->
                            </div>
                        </div>
                    </div>
                </div>

                <div class="item-card">
                    <div class="card">
                        <img class="card__img"
                            src="https://cdn-dynmedia-1.microsoft.com/is/image/microsoftcorp/personal-family?resMode=sharp2&amp;op_usm=1.5,0.65,15,0&amp;wid=1099&amp;hei=880&amp;qlt=75">
                        <div class="card__body green">
                            <p class="body__title">
                                <button class="title__btn" type="button" role="button" @click="collapseClick(3)">
                                    Grande Empresa
                                </button>
                            </p>
                            <div :class="[(interaction.collapse == 3) ? 'collapse-show' : 'collapse-hide']">
                                <div class="items__center">
                                    <p>Permite que tus empleados con herramientas colaboren de forma segura y
                                        trabaja desde cualquier lugar.</p>
                                </div>
                            </div>
                            <div class="items__link__group">
                                <a class="btn green"
                                    href="https://www.microsoft.com/es/microsoft-365/explore-microsoft-365-for-home">
                                    Más información
                                </a>
                                <a class="btn__link"
                                    href="https://www.microsoft.com/es/microsoft-365/buy/compare-all-microsoft-365-products?tab=1">
                                    Ve los planes personales y familiares
                                </a>
                                <!--button/cta disclaimer-->
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>



</template>

<script>
export default {
    name: "PreciosView",
    mounted() {

    },
    data(){
        return {
            interaction: {
                collapse: 0
            }
        }
    },
    methods: {
        collapseClick(index) {
            if (index == this.interaction.collapse) this.interaction.collapse = 0
            else this.interaction.collapse = index
        }
    }
}
</script>