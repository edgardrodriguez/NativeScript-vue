<template lang="html">
    <Page>
        <ActionBar>
            <Label text="Buscar"></Label>
        </ActionBar>

        <GridLayout class="page__content">
            <Label class="page__content-icon fas" text.decode="&#xf002;"></Label>
            <Label class="page__content-placeholder" :text="message"></Label>
        </GridLayout>
    </Page>
</template>

<script>
  export default {
    data() {
      return {
        message: "<!-- El contenido de la página de búsqueda va aquí -->"
      };
    }
  }
</script>

<style lang="scss" scoped>
    // Start custom common variables
    @import "@nativescript/theme/scss/variables/blue";
    // End custom common variables

    // Custom styles

</style>
