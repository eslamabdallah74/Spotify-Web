<script setup>
const route = useRoute()

const client_id          = 'f1c2532691fd4d11bce39cfc7124110e';
const client_secret      = 'c5cd82fce51c489091e5ec587d7abe08';
const redirect_uri       = 'http://localhost:3000/';
const spotifyAuth        = "https://accounts.spotify.com/authorize";
const encode_uri         = encodeURI(redirect_uri);
const TOKEN              = "https://accounts.spotify.com/api/token";
const code               = route.query.code
const encodedID          = btoa(client_id + ":" + client_secret);

const login = () => {
    const authorizationUrl = `${spotifyAuth}?client_id=${client_id}&response_type=code&redirect_uri=${encode_uri}&show_dialog=true$scope=&scope=user-read-private user-read-email user-modify-playback-state user-read-playback-position user-library-read streaming user-read-playback-state user-read-recently-played playlist-read-private`
    // Go to
    window.location.href = authorizationUrl;

}
onMounted (() => {
    const sendRequest = $fetch(TOKEN,{
        method: "POST",
        params:{
            grant_type: "authorization_code",
            code: code,
            redirect_uri: encode_uri
        },
        headers: {
            "Content-Type"  : "application/x-www-form-urlencoded",
            "Authorization" : `Basic ${btoa}`
        }
    })

})

const refreshToken = () => {

}

</script>
<template>
    <div>
        <div>
            <div id="login">
                <h1>First, log in to spotify</h1>
                <button @click="login">Log in</button>
            </div>
        </div>
    </div>
</template>