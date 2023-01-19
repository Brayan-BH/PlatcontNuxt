<template>
    <main>
        <div class="container-login">

            <div class="container-form">
                <div class="content-center">
                    <h2>Iniciar Sesión</h2>
                    <hr class="divider">
                </div>
                <!-- start form -->
                <div class="form-body">
                    <div class="form-content">
                        <form>
                            <!-- Email address input-->
                            <div class="form-floating">
                                <input class="form-control" name="email" type="email">
                                <label for="email">Correo Electrónico</label>
                            </div>
                             <!-- Password-->
                             <div class="form-floating">
                                <input class="form-control" name="email" type="password">
                                <label for="email">Contraseña</label>
                            </div>
                        </form>
                        <NuxtLink href="" to="#">¿Has olvidado tu correo electrónico?</NuxtLink>
                        <div class="d-grid">
                                <button class="btn-register" id="button-enviar">
                                    Crear cuenta
                                </button>
                                <button class="btn-ingresar" id="button-enviar">
                                    Ingresar
                                </button>
                            </div>
                    </div>
                </div>

            </div>
        </div>
    </main>
</template>