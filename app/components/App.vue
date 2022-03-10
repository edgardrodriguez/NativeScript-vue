<template lang="html">
    <TabView androidTabsPosition="bottom">
        <TabViewItem title="Inicio">
            <Frame id="items">
                <Items/>
            </Frame>
        </TabViewItem>

        <TabViewItem title="Navegar">
            <Frame id="browse">
                <Browse/>
            </Frame>
        </TabViewItem>

        <TabViewItem title="Buscar">
            <Frame id="search">
                <Search/>
            </Frame>
        </TabViewItem>
    </TabView>
</template>

<script>
  import Items from "./Items.vue";
  import Browse from "./Browse.vue";
  import Search from "./Search.vue";

  export default {
    components: {
      Items,
      Browse,
      Search
    }
  };
</script>

<style lang="scss">
    // Start custom common variables
    @import "@nativescript/theme/scss/variables/blue";
    // End custom common variables

    // Custom styles

</style>
