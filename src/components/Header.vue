<template>
    <v-toolbar app>
        <v-toolbar-title>VueGram</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-title>{{userName}}</v-toolbar-title>
        <v-toolbar-items class="hidden-sm-and-down ml-4" >
            <v-btn flat><v-avatar
                size="48px"
                color="red"
            >
                <img :src="profileImg" alt="alt">
            </v-avatar></v-btn>
        </v-toolbar-items>
  </v-toolbar>
</template>
<script>
export default {
    name: "app-toolbar",
    props: {
        userName: String,
        profileImg: String
    }
}
</script>

