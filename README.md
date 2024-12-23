# HAPPY DOWNLOADER (HAPPY DL)

A simple tool to generate direct download links for media from Instagram, Facebook, and Twitter! Just provide the post URL, and this package will return a direct download URL.

## Installation

You can install `happy-dl` via npm:

```bash
npm install happy-dl
```

Or, if you're using Yarn:

```bash
yarn add happy-dl
```

## Usage

### Importing the Package

You can import the entire `happy-dl` module:

```javascript
const happyDL = require("happy-dl");
```

Or destructure specific functions:

```javascript
const {
  instagramDownloader,
  facebookDownloader,
  twitterDownloader,
} = require("happy-dl");
```

### Example Usage

#### Instagram Downloader

```javascript
happyDL
  .instagramDownloader("https://www.instagram.com/reel/C2xQMDBBY6v/")
  .then((result) => console.log("Fetched Instagram media details:", result))
  .catch((error) => console.error("Error fetching Instagram media details:", error));
```

#### Facebook Downloader

```javascript
happyDL
  .facebookDownloader("https://www.facebook.com/share/r/yfF9ZULaNJnQ72Ur/")
  .then((result) => console.log("Fetched Facebook media details:", result))
  .catch((error) => console.error("Error fetching Facebook media details:", error));
```

#### Twitter Downloader

```javascript
happyDL
  .twitterDownloader("https://x.com/ImHappyKumar/status/1758877530776547450")
  .then((result) => console.log("Fetched Twitter media details:", result))
  .catch((error) => console.error("Error fetching Twitter media details:", error));
```

## Supported Platforms

- Instagram
- Facebook
- Twitter
- More coming soon!

## Contributing

Contributions are welcome! If you find any issues or want to contribute new features, feel free to fork the repository and create a pull request.

### Steps to Contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
