# ¡Hola! 👋, Soy Bruno Llovera. 
<!--
**Bhargavi-hash/Bhargavi-hash** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
-->

<img align="right" width=300px alt="Unicorn" src="https://c.tenor.com/GN73MKBawZYAAAAi/busy-cute.gif" />

## <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px">&nbsp;***Sobre mí***
Soy estudiante en la Universidad Tecnológica de Cancún, estudio un TSU en Tecnologías de la Información, Área de Desarrollo de Software Multiplataforma. Actualmente me siento satisfecho de mi carrera ya que quisiera desempeñarme profesionalmente en un futuro en un Desarrollador Software. Mi sueño es trabajar y vivir de eso, de lo que mas me interesa.
* **Estoy interesado en el desarrollo web, desarrollo movil y desarrollo de software**
- 🌱 Actualmente estoy aprendiendo ...
  - Java
  - JavaScript
  - React js

__Check out my GitHub repository:__

<div>
   <p align="center">
    <b><em>Canción favorita:</em></b> <br/>
    <iframe style="border-radius:12px" src="https://open.spotify.com/embed/track/21B4gaTWnTkuSh77iWEXdS?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </p>
</div>


<h2>👀 My github Stats</h2>

<div>

  
  <p align="center">
  <b><em>GitHub Stats:</em></b> <br/>
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=Bhargavi-hash" alt="GitHub Stats" /> <br/><br/>
  
</div>

![My github status](https://github-readme-stats.vercel.app/api?username=Bhargavi-hash&show_icons=true&include_all_commits=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Bhargavi-hash&layout=compact)










# spotify-github-profile

Create Spotify now playing card on your github profile

Running on Vercel serverless function, store data in Firebase (store only access_token, refresh_token, token_expired_timestamp)

## Annoucements

**2024-06-21**

Vercel change the package the free tier is not enough for our usage. I moved service to self-host at Digital Ocean.

Please replace your old endpoint `https://spotify-github-profile.vercel.app` to `https://spotify-github-profile.kittinanx.com`

## Table of Contents  
[Connect And Grant Permission](#connect-and-grant-permission)  
[Example](#example)  
[Running for development locally](#running-for-development-locally)  
[Setting up Vercel](#setting-up-vercel)  
[Setting up Firebase](#setting-up-firebase)  
[Setting up Spotify dev](#setting-up-spotify-dev)  
[Running locally](#running-locally)  
[How to Contribute](#how-to-contribute)  
[Known Bugs](#known-bugs)  
[Features in Progress](#features-in-progress)  
[Credit](#credit)  

## Connect And Grant Permission

- Click `Connect with Spotify` button below to grant permission

[<img src="/img/btn-spotify.png">](https://spotify-github-profile.kittinanx.com/api/login)

## Example

- Default theme

![spotify-github-profile](/img/default.svg)

- Compact theme

![spotify-github-profile](/img/compact.svg)

- Natemoo-re theme

![spotify-github-profile](/img/natemoo-re.svg)

- Novatorem theme

![spotify-github-profile](/img/novatorem.svg)

- Karaoke theme

![spotify-github-profile](/img/karaoke.svg)



## Running for development locally

To develop locally, you need:

- A fork of this project as your repository
- A Vercel project connected with the forked repository
- A Firebase project with Cloud Firestore setup
- A Spotify developer account

### Setting up Vercel

- [Create a new Vercel project by importing](https://vercel.com/import) the forked project on GitHub

### Setting up Firebase

- Create [a new Firebase project](https://console.firebase.google.com/u/0/)
- Create a new Cloud Firestore in the project
- Download configuration JSON file from _Project settings_ > _Service accounts_ > _Generate new private key_
- Convert private key content as BASE64
  - You can use Encode/Decode extension in VSCode to do so
  - This key will be used in step explained below

### Setting up Spotify dev

- Login to [developer.spotify.com](https://developer.spotify.com/dashboard/applications)
- Create a new project
- Edit settings to add _Redirect URIs_
  - add `http://localhost:3000/api/callback`

### Running locally

- Install [Vercel command line](https://vercel.com/download) with `npm i -g vercel`
- Create `.env` file at the root of the project 
- Paste your keys in `SPOTIFY_CLIENT_ID`, `SPOTIFY_SECRET_ID`, and insert the name of your downloaded JSON file in `FIREBASE`


```sh
BASE_URL='http://localhost:3000/api'
SPOTIFY_CLIENT_ID='____'
SPOTIFY_SECRET_ID='____'
FIREBASE='__BASE64_FIREBASE_JSON_FILE__'
```

- Run `vercel dev`

```sh
$ vercel dev
Vercel CLI 20.1.2 dev (beta) — https://vercel.com/feedback
> Ready! Available at http://localhost:3000
```

- Now try to access http://localhost:3000/api/login

## How to Contribute

- Develop locally and submit a pull request!
- Submit newly encountered bugs to the [Issues](https://github.com/kittinan/spotify-github-profile/issues) page
- Submit feature suggestions to the [Issues](https://github.com/kittinan/spotify-github-profile/issues) page, with the label [Feature Suggestion]

## Known Bugs

[404/500 Error when playing local files](https://github.com/kittinan/spotify-github-profile/issues/19)

## Other Platforms
- [Apple Music GitHub Profile](https://github.com/rayriffy/apple-music-github-profile)

## Credit

Inspired by https://github.com/natemoo-re
