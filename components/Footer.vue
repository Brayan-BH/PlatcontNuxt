<template>
    <div class="container-foot">
        <div class="content-container">
            <div class="row">
                <!-- Footer Menu -->
                <div class="footer-menu">
                    <p>Platcont</p>
                    <ul class="platcont-items">
                        <li class="list">
                            <nuxt-link to="/" class="text-light">Inicio</nuxt-link>
                        </li>
                        <li class="list">
                            <nuxt-link to="/whyplatcont" class="text-light">¿Por qué Platcont?</nuxt-link>
                        </li>
                        <li class="list">
                            <nuxt-link to="/precios" class="text-light">Precios</nuxt-link>
                        </li>
                        <li class="list">
                            <nuxt-link to="/contactanos" class="text-light">Contáctanos</nuxt-link>
                        </li>
                    </ul>
                </div>
                <!--  -->
                <!-- Footer Redes -->
                <div class="footer-sociales">
                    <p>Redes Sociales</p>
                    <div class="red-social">
                        <nuxt-link to="https://twitter.com/?lang=es" target=" _blank">
                            <img src="/img/icons/twitter.png" alt="facebook" width="30">
                        </nuxt-link>
                    </div>
                    <div class="red-social">
                        <nuxt-link to="https://www.youtube.com" target=" _blank">
                            <img src="/img/icons/youtube.png" alt="facebook" width="30">
                        </nuxt-link>
                    </div>
                    <div class="red-social">
                        <nuxt-link to="https://www.facebook.com" target=" _blank">
                            <img src="/img/icons/facebook_messenger.png" alt="facebook" width="30">
                        </nuxt-link>
                    </div>
                    <div class="red-social column-2">
                        <nuxt-link to="https://api.whatsapp.com/send?phone=51924700200" target=" _blank">
                            <img src="/img/icons/whatsapp.png" alt="facebook" width="30">
                        </nuxt-link>
                    </div>
                </div>
                <!--  -->
                <!-- Footer Contacto -->
                <div class="footer-contactos">
                    <p>Contáctanos</p>
                    <ul class="platcont-items">
                        <li class="list border-bottom">
                            <nuxt-link to="://924-700-200" class="text-light">Celular:
                                924-700-200
                            </nuxt-link>
                        </li>
                        <li class="list border-bottom">
                            <nuxt-link to="platcont@hotmail.com" class="text-light">Correo
                                Electrónico: platcont@hotmail.com
                            </nuxt-link>
                        </li>
                    </ul>
                </div>
                <!--  -->
            </div>
        </div>
    </div>
</template>