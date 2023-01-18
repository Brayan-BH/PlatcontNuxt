<template>
    <div class="container-form">
        <div class="content-center">
            <h2>Contacta a Platcont</h2>
            <hr class="divider">
            <p>
                No dudes en comunicarte con nosotros, haznos llegar tus dudas y con gusto te ayudamos.
            </p>
        </div>
        <!-- start form -->
        <div class="form-body">
            <div class="form-content">
                <form>
                    <!-- Name input-->
                    <div class="form-floating">
                        <input class="form-control" name="name" type="text">
                        <label for="name">Nombre</label>
                    </div>
                    <!-- Email address input-->
                    <div class="form-floating">
                        <input class="form-control" name="email" type="email">
                        <label for="email">Correo</label>
                    </div>
                    <!-- Phone number input-->
                    <div class="form-floating">
                        <input class="form-control" name="telefono" type="tel">
                        <label for="email">Teléfono</label>
                    </div>
                    <!-- Message input-->
                    <div class="form-floating">
                        <textarea class="form-control textarea" name="asunto" type="text">
                        </textarea>
                        <label for="message">Comentario</label>
                    </div>
                    <div class="d-grid">
                        <button class="button-green" id="button-enviar">Enviar</button>
                    </div>
                </form>
            </div>
        </div>
        <!-- end form -->
        <div class="contact-message">
            <nuxt-link to="https://api.whatsapp.com/send?phone=51924700200" target=" _blank">
                <img src="/img/icons/whatsapp.png" alt="whatsapp" width="50">
            </nuxt-link>
            <p class="text-muted">
                Escribeme al whatsapp es más rapido
            </p>
            <div>+51 924700200</div>
        </div>
    </div>
</template>