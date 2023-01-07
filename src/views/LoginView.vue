<template>
        <div className="container">
            <div className="container-login">
                <div className="wrap-login">
                    <form className="login-form">
                        <span className="login-form-title">Bem Vindo!</span>

                        <span className="login-form-title">
                            <img src="../assets/bigasBranco.png" alt="Logo do Bigas"/>
                        </span>

                        <div className="wrap-input">
                            <input type="email" name="email" id="email">
                            <span className="focus-input" data-placeholder="Email"></span>
                         </div>

                        <div className="wrap-input">
                            <input type="password" name="password" id="password">
                            <span className="focus-input" data-placeholder="Password"></span>
                        </div>

                        <div className="container-login-form-btn">
                            <button className="login-form-btn">Entrar</button>
                        </div>

                        <div className="text-account">
                            <span className="txt1">Não possui conta?</span>

                            <a href="/register" className="txt2">Criar Conta</a>
                        </div>
                    </form>
                </div>
            </div>
        </div>
</template>


<script>
import FormComponentsVue from '@/components/FormComponents.vue';

    export default {
        name: 'LoginView',
        components: {
            FormComponentsVue 
        }
    }

</script>


<style scoped>

</style>