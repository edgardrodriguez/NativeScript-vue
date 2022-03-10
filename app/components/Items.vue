<template>
    <Page>
        <ActionBar>
            <Label text="Inicio"></Label>
        </ActionBar>

        <ListView for="item in items" @itemTap="onItemTap">
            <v-template>
                <StackLayout orientation="horizontal">
                    <Label :text="item.name" textWrap="true"></Label>
                </StackLayout>
            </v-template>
        </ListView>
    </Page>
</template>

<script>
  import ItemDetails from "./ItemDetails";

  export default {
    data() {
      return {
        items: [
          {
            name: "Item 1",
            description: "Descripción del Item 1"
          },
          {
            name: "Item 2",
            description: "Descripción del Item 2"
          },
          {
            name: "Item 3",
            description: "Descripción del Item 3"
          },
          {
            name: "Item 4",
            description: "Descripción del Item 4"
          },
          {
            name: "Item 5",
            description: "Descripción del Item 5"
          },
          {
            name: "Item 6",
            description: "Descripción del Item 6"
          },
          {
            name: "Item 7",
            description: "Descripción del Item 7"
          },
          {
            name: "Item 8",
            description: "Descripción del Item 8"
          },
          {
            name: "Item 9",
            description: "Descripción del Item 9"
          },
          {
            name: "Item 10",
            description: "Descripción del Item 10"
          },
          {
            name: "Item 11",
            description: "Descripción del Item 11"
          },
          {
            name: "Item 12",
            description: "Descripción del Item 12"
          },
          {
            name: "Item 13",
            description: "Descripción del Item 13"
          },
          {
            name: "Item 14",
            description: "Descripción del Item 14"
          },
          {
            name: "Item 15",
            description: "Descripción del Item 15"
          },
          {
            name: "Item 16",
            description: "Descripción del Item 16"
          }
        ]
      };
    },
    methods: {
      onItemTap(args) {
        this.$navigateTo(ItemDetails, {
          frame: 'items',
          props: {item: args.item},
          animated: true,
          transition: {
            name: "slide",
            duration: 200,
            curve: "ease"
          }
        });
      }
    }
  };
</script>

<style scoped lang="scss">
    // Start custom common variables
    @import "@nativescript/theme/scss/variables/blue";
    // End custom common variables

    // Custom styles

</style>
