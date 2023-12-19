# welcome to sepioidea! [propnounced: sep-eo-id-eia, aka vulbytes vTuberThing]

this is meant to be a one stop shop for a v-tuber application with the following goals in mind: <br>

1. being 1 "do it all" application.
2. supporting 2d images and 3d poses
3. being more dynamic and scalable.
4. no dependancies on external softwares outside of obs
5. cross platform (Linux, MacOs, and Windows for those who don't have taste)
6. multi-user ease
7. easy to switch between multiple systems
8. break immersion as little as possible

<br>

## v1 to-do list:

[ ] - audio

<!-- prettier-ignore -->
    [ ] - audio input selection
    [ ] - threshold ui
    [ ] - "cooldown" 
    [ ] - 2d audio matrix

[ ] - 2d formats

<!-- prettier-ignore -->
    [ ] - add options for gifs (ie, play, hold on xFrame, etc etc
    [ ] - above but for videos
    [ ] - sub image anchoring 
    [ ] - automated tweening

[ ] - 3d formats

<!-- prettier-ignore -->
    [ ] - impliment three.js (easier this way)
    [ ] - easily import poses 
    [ ] - easy import animations and set them to do things based on audio context

[ ] - save/export config

<!-- prettier-ignore -->
    [ ] - user settings
    [ ] - pack images into save file for easy transport
    [ ] - pack 3d models and other information for easy transport

[ ] - credits file

[ ] - stretch features (no promise of implimentation

<!-- prettier-ignore -->
    [ ] - multiple audio inputs
    [ ] - chat retheming and stylization
        [ ] - creatable "chat" events that can trigger effects
    [ ] - audio effects
    [ ] - screen context which can dynamically effect the lighting of the model to be more immersive
    [ ] - 3d animation tweening support (figure out A -> B using interp method to make transitions less jank)
    [ ] - custom ui themes build in

## FAQ

### here's the obvious question, why make this?

well, there's a couple reasons. <br>

1. for my own self interest, i love playing with tech and i feel like this would be a fun project
2. coding portfolio. as of current i don't have a tonne of "big" projects under my belt so i feel like this would be a fun one.
3. monitary insentives, outside of the above, i plan to keep this project foss, however i do hope to receive community support via:

- a purchase on steam as a "tip", with the added luxury of auto updates
- various donations made on platforms (tba)
- "bounties" from creators requesting specific features (we will listening to the public, and will not be accepting any request, this is simply for the purpose of expoditing a reasonable feature)

4. community recognition, i just think it would be neat to have made a product that people enjoy and like using c:
5. build a community and more eyes/support on further projects! there's a lot more then just this i wanna do

### what about [vaedotuber mini](https://olmewe.itch.io/veadotube-mini)? why don't you just use that?

simply put, i find it too basic, and moving around between systems is sorta just a pain for me. i have huge respect to the dev of this and similar projects, i just don't feel like it's a fit for me, and if it's not a fit for me i imagine it wont be for many others aswell.

### what if i have an issue with (x)

sadly due to personal reasons and me working on this solo at the time of writing, i cannot garuntee that i'll be able to address every issue. unless this project becomes big enough i can either work on it full time, or hire someone to work on it full time, there is no garuntees i can make, so until then the software is provided **as is** with no warrenty or support garunteed. however feel free to create an issue [here](https://github.com/vulbyte/vtuberThing/issues), please do check your issue is unique before creating a new issue

### can you add (x)?

maybe! there's no garuntee so unless you can sponcer the development of a feature there's no garuntee. tho feel free to ask anyways!

### this/you are/is cringe

:3

### why did you use tauri with nextjs? don't you know (x) is faster?! omg you don't know what you're doing

yeh, i don't lmao. the main reason i'm using tauri x nextJs is because i feel like this will be the relitive easiest to make cross platform, keep preformant, and allow ease of modding. without (spilling the beans)[https://dictionary.cambridge.org/dictionary/english/spill-the-beans] i have some futire ideas that will need networking, and having the nextJS backbone will really help with that.
i also know other things are faster, but i want this to be an application i can casually dip in and out of with ease. and coding from scratch a c++ or rust gui and all that stuff doesn't feel like it would be a good time investment for this project when html+css+js(react) already does all that for me.

### why two windows? why can't i have it all in one window?

sepioidia was built with the mentality of "never breaking immmersion", one reason it has two windows, one being display, the other being settings is so that the display windows is **NEVER** interupted or affected in any way.

### what about change the size of it?

that can be done in the settings pannel. again with the above statement, we want to keep streams/recordings as flawless as possible, and if you accidentally rescaled the window that could mess up your recording, and it's our primary goal to prevent that from happening.

### why do some changes need a restart to apply?

simply put, the tauri applicati

## can i clone/fork/make a derivitive of this?

totally! <br>
however, feel free to reach out first though because as long as it's within the vision of the applications core, we might be able to integrate it into the core of the project! <br>
however if if you wish to anyways here are the requirements: <br>

1.  Rule Compliance:
    When forking or cloning the project, adhere to the rules of the latest version at that time. Use terms from the version you copied, unless it's a direct fork at version 1. In case of ambiguity (e.g., no date provided), default to the rules at the time of the first public clone or derivative. If there's no proof of cloning at a specific version, even if cloned at v3, adhere to the rules of the version at the time of posting (v14 in the given example).
2.  Hosting and Attribution:
    Ensure a conspicuous link to the project's hosting location is present in the README file (using the default Markdown format). The link should also be clearly visible within the application itself. Additionally, include the link wherever the project is advertised, such as on websites, to direct users back to the core project (https://www.github.com/vulbyte/vtuberThing).
3.  the application must not alter (at the time of fork) these files:
    <!-- prettier-ignore -->
        - credits.md

- credits

4. Non-Commerical and FOSS
   All forks/derivatives should be non-commercial. While additional support can be offered for sale, the core, extensions, or any related components must remain free and open-source.

5. any sub derivitives are required to agree to the same rules and licensing.
6. this project is not to be used as training data for ai's, gpt's, or anything of that nature.
7. if the user/organization/other doesn't adhere to these rules, they will be laiable to a fine at the descression of vulbyte.

#### this section is for the idiot developer (vulbyte)

First, run the development server:

```bash
pnpm tauri dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.on wrapper requires it. and i would rather keep that part of the app as close to stock to keep upgrades and what not easier to impliment.

## Thank you to these third parties for providing the tools to make this possible:

(in alphabetical order)<br>

- github - for hosting this project @[github](https://www.github.com/)
- mozilla - for their amazing developer documentation @[mozilla](https://developer.mozilla.org/en-US/)
- pnpm - for tool they provide @[pnpm](https://pnpm.io/)
- react - the react team @[react.dev/](https://react.dev/)
- tauri - the tauri app team @[tauri.app](https://tauri.app/)
- threeJS - the threeJS team @[threejs.org](https://threejs.org/)
- typescript - the typescript team @[typescriptlang.org/](https://www.typescriptlang.org/)
- nextJS - the nextJS team @[vercel](https://vercel.com/solutions/nextjs/)
- w3 - the w3 foundation for their great documentation @[w3schools](https://www.w3schools.com/)
