<template>
    <main>
        <div class="container-register">
            <div class="form-register">
                <div class="head-register">
                    <h2>Registrate ahora</h2>
                    <img class="logo__img" src="/img/logo.png" alt="logo">
                </div>
                <form >
                    <div class="body-register">
                        <div class="item">
                            <input type="text" required>
                            <span>Nombres y apellidos</span>
                        </div>
                        <div class="item">
                            <input type="email" required>
                            <span>Coreo ELecronico</span>
                        </div>
                        <div class="item">
                            <input type="tel" required>
                            <span>Teléfono</span>
                        </div>
                        <div class="item">
                            <input type="password" required>
                            <span>Contraseña</span>
                        </div>
                        <div class="item">
                            <input type="tel" required>
                            <span>Confirmar Contraseña</span>
                        </div>
                    </div>
                </form>
                <nuxt-link href="" to="#">Terminos y Condiciones</nuxt-link>
                <div class="d-grid">
                    <button class="btn-ingresar" id="button-enviar">
                        Ingresar
                    </button>
                </div>
            </div>
        </div>
    </main>
</template>