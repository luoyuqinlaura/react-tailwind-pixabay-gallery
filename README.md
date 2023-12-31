# Image Gallery

   <img src="./src/assets/search-for-cats.png">

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

## Image Tags Component

since the tags are included in an array.
<img src="./src/assets/api.png">

1. we get image as the prop in imageCard, since tags belongs to each image, so we can loop through the tag in the place that we want to display tags.
2. used split() which can convert string into array

## Image Search Component

1. format
2. logic: since this is a form, we need get the user input, so we get a state 'text' whever the input is onChange. However, this is not an App level state, so when user click search button, we need using prop to transfer the 'text' to the APP level 'term'
3. term as dependency, whenever term change, the useEffect will run again.
