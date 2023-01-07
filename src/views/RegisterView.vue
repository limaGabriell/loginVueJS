<template>
    <div className="container">
            <div className="container-login">
                <div className="wrap-login">
                    <form className="login-form">
                        <span className="login-form-title">Criar Conta</span>

                        <span className="login-form-title">
                            <img src="../assets/bigasBranco.png" alt="Logo do Bigas"/>
                        </span>

                        <div className="wrap-input">
                            <input type="text" name="name" id="name">
                            <span className="focus-input" data-placeholder="Nome"></span>
                        </div>

                        <div className="wrap-input">
                            <input type="email" name="email" id="email">
                            <span className="focus-input" data-placeholder="Email"></span>
                        </div>

                        <div className="wrap-input">
                            <input type="password" name="password" id="password">
                            <span className="focus-input" data-placeholder="Password"></span>
                        </div>

                        <div className="container-login-form-btn">
                            <button className="login-form-btn">Cadastrar</button>
                        </div>

                        <div className="text-account">
                            <span className="txt1">Ja tenho conta</span>

                            <a href="/" className="txt2">Entrar</a>
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

<style>
    
</style>