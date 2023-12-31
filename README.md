# Image Gallery

## Create card template

1. set up tailwind and react

```
cd '/Users/biubiubiu/Documents/Udemy/youtubeReactTaiwind'

npx create-react-app data-finance-yt

npm install -D tailwindcss
npx tailwindcss init

npm start
```

2. in the tailwind.config file, add content to the content
   in the index.css file, only

```
@tailwind base;
@tailwind components;
@tailwind utilities;

```

## Create API Key

Fetching data and make the card template into component looping through all the images.

1. Pixabey API
   get myself api key, save it in the .env file
2. useEffect: how we make request

## Image Card Component

1. fetching the data and put it into the state(setImages), now all the hits array are put into Images
2. we create ImageCard components, and in App.js, we loop through the images array, put each image into ImageCard components.
3. notice that: since we are creating a list, we need attribute 'key', which must be unique.
4. next step, passing image as prop, from app.js to imagecard.js

## Image Prop Component

1.passing prop image, which is every image from the images list of App.js, passing to imageCard, and we can get the info from each image, to set views, authors, likes...
