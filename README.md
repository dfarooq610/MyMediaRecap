# MyMediaRecap

in 2023, i want to be able to share an instragram story highlighting what i watched, listened to, and read each month. This is a tool to try and generate those images programatically, since designing them manually in figma was quite a pain.

given a list of IMDB movie IDs and a list of LCCN Book Numbers, and a background color hex code generates an 1080x1920 image to share on instagram

### Input
```json
{
  "movies": ["tt19770238", "tt3915174"],
  "books": ["2020022471"],
  "background": "02534C",
}
```

### Output
<p align="center">
  <img src="https://user-images.githubusercontent.com/59672089/215275423-97e4b2e1-4357-4d30-856e-8de6a14939be.png" width="324" height="576">
</p>

### Features
- ideally fetches top tracks from spotify API for your user. 

- for movie thumbnails, uses https://www.omdbapi.com/

- for book thumbnail, uses https://openlibrary.org/dev/docs/api/covers

- need to think of a programatic way to generate the pic of the month. Want assets to autoscale within boundaries (what if i had 7 movies?)

- need to think of a way to analyze the book of the month

- might be nice to make a UI where you can directly share to instagram stories?
