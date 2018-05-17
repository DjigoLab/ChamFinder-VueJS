<template>
      <div class="container">
        {{msg}}{{name}}
        <form action="" method="post">
            <div class="form-field username">

                <label for="name">Username</label>
                <input type="name" name="name" v-model="name">
            </div>
            <div class="form-field email">

                <label for="email">Email</label>
                <input type="email" name="email" v-model="email">
            </div>
            <div class="form-field password">

                <label for="password">Password</label>
                <input type="password" name="password" v-model="password">
            </div>
            <div class="form-field confirmPassword">

                <label for="repeatPassword">Confirm Password</label>
                <input type="password" name="repeatPassword" v-model="repeatPassword">
            </div>
            <div class="form-field terms">
                <input type="checkbox" name="terms" v-model="accept">
                <label for="terms">Accept Terms</label>
            </div>

        <p v-if="accept == true">Your name is {{name}}, with the e-mail {{email}}, using a codificated
            password, which is {{password}}, and you have accepted  our terms.
        </p>
        <p v-else>
                Your name is {{name}}, with the e-mail {{email}}, using a codificated
                password, which is {{password}}, and you have NOT ACCEPTED our terms.
        </p>
        <p v-if="password === repeatPassword">
            Oh, by the way, your passwords are equal, good.
        </p>
        <p v-else>
            Hey, seems that you wrote your confirmation password wrong...
        </p>
            <button type="submit">Submit</button>
        </form>
      </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      msg: "Hello, ",
      name: "Stranger",
      email: "",
      password: "",
      repeatPassword: "",
      accept: false
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
  padding: 15px;
}
form {
        display: flex;
        flex-flow: column;
        padding: 10px;
    }

    .form-field {
        display: grid;
    }

    p{
        padding: 15px;
    }
</style>
