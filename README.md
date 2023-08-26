# note-homepage-cards

Source code of the pokemon-like cards on my [notebook](https://note.tonycrane.cc/)'s homepage, modified from [simeydotme/pokemon-cards-css](https://github.com/simeydotme/pokemon-cards-css/).

## Usage

- Install dependencies
    ```shell
    $ npm install
    ```
- Run locally for development
    ```shell
    $ npm run dev # open at https://localhost:5173/
    ```
- Build to static files
    ```shell
    $ npm run build
    ```
- Copy to note's mkdocs project
    - Copy static files
        ```text
        dist/assets/index.???.css
        dist/assets/index.???.js
        public/*
        ```
    - Insert html to homepage
        ```html
        <link rel="stylesheet" href="css/cards/base.css" />
        <link rel="stylesheet" href="css/cards/cards.css" />
        <script type="module" crossorigin src="/assets/cards/index.???.js"></script>
        <link rel="stylesheet" href="/assets/cards/index.???.css">
        <div id="app"></div>
        ```

## Acknowledgement

- [simeydotme/pokemon-cards-css](https://github.com/simeydotme/pokemon-cards-css/)

## LICENSE

Licensed under [GPL-3.0](https://github.com/TonyCrane/note-homepage-cards/blob/main/LICENSE), same as the upstream's [license](https://github.com/TonyCrane/note-homepage-cards/blob/main/LICENSE.pokemon-cards-css).