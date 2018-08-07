<template>
<v-card elevation-3>
    <v-toolbar color>
        <v-toolbar-title>
            <v-avatar
                color="red"
            >
                <img :src="profileImg" alt="alt">
            </v-avatar>
            <span>{{userName}}</span>
            
        </v-toolbar-title>
        <v-spacer></v-spacer>
    </v-toolbar>
    <v-card-media
        
        height="400px"
        :src="image"
    >
        
    </v-card-media>
    <v-card-text>
        <span class="black--text">{{userName}}:</span>
        <span class="grey--text">{{postDescr}}</span>
    </v-card-text>
</v-card>
</template>

<script>
export default {
    name: 'Post',
    data () {
        return {}
    },
    props: {
        profileImg: String,
        userName: String,
        postDescr: String,
        likes: Number,
        image: String
    }
}
</script>
