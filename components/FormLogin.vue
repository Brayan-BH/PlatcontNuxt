<template>
    <main>
        <div class="container-login">
            <div class="form-container">
                <div class="head">
                    <h2>Iniciar Sesión</h2>
                    <img class="logo__img" src="/img/logo.png" alt="logo">
                </div>
                <form>
                    <div class="body">
                        <div class="inputbox">
                            <input type="mail" required>
                            <span>Coreo Electronico</span>
                        </div>
                        <div class="inputbox">
                            <input type="password" required>
                            <span>Contraseña</span>
                        </div>
                    </div>
                </form>
                <nuxt-link to="#">¿Has olvidado tu correo electrónico?</nuxt-link>
            </div>
            <div class="d-grid">
                <button class="btn-register" id="button-enviar">
                    <nuxt-link to="/signup">Crear Cuenta</nuxt-link>
                </button>
                <button class="btn-ingresar" id="button-enviar">
                    Ingresar
                </button>
            </div>
        </div>
    </main>
</template>