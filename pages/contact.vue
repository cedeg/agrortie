<template>
  <section class="section">
    <div class="container has-background-light">
      <div class="section">
        <h2
          class="has-text-primary is-size-3 is-size-4-mobile has-text-centered"
        >
          Contact
        </h2>
        <p class="is-size-5 is-size-6-mobile">
          Passez votre commande (à partir de 500kg en vrac ou par seaux ou sacs
          de 5kg) envoyez un message à
          <a href="mailto:info@agrortie.be" class="has-text-primary">
            info@agrortie.be
          </a>
        </p>
        <p class="is-size-5 is-size-6-mobile">
          Ou utilisez le formulaire ci-dessous
        </p>
        <b-field grouped>
          <b-field label="Nom" expanded>
            <b-input></b-input>
          </b-field>
          <b-field label="Prénom" expanded>
            <b-input></b-input>
          </b-field>
        </b-field>
        <b-field grouped>
          <b-field label="Mail" expanded>
            <b-input></b-input>
          </b-field>
          <b-field label="Société" expanded>
            <b-input></b-input>
          </b-field>
        </b-field>
        <b-input
          type="textarea"
          minlength="10"
          maxlength="100"
          placeholder="Message"
        >
        </b-input>
        <b-checkbox v-model="hasError">
          J'accepte que mes données soient sauvegardées par AGRORTIE scrl sans
          utilisation extérieure
        </b-checkbox>
        <br />
        <b-button type="is-primary is-pulled-right">Envoyer</b-button>
      </div>
    </div>
  </section>
</template>
