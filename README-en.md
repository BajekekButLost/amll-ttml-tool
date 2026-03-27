<div align="center">

<img src="./public/logo.svg" align="center" width="256">

# Apple Music-like Lyrics TTML Tool

A modern word-by-word lyrics editor built for the [Apple Music-like Lyrics ecosystem](https://github.com/amll-dev/applemusic-like-lyrics)!

<img width="1312" alt="image" src="https://github.com/user-attachments/assets/4db81b29-df0c-4f6e-819a-3b956b28247c">
<img width="1312" alt="image" src="https://github.com/user-attachments/assets/929eefee-ebda-43db-ad04-c0f099077053">
<img width="1312" alt="image" src="https://github.com/user-attachments/assets/7c80902e-45a9-42ae-b980-f5500069acb8">

</div>

## Usage

> [!WARNING]
> This tool is not recommended for mobile phones or small-screen devices, as editing can be quite cumbersome.

You can try the online version here:  
[`https://amll-ttml-tool.stevexmh.net/`](https://amll-ttml-tool.stevexmh.net/)

You are also welcome to check out the [test deployment](https://amll-ttml-tool-test.vercel.app/) to experience the latest features (and the latest bugs).

A Tauri desktop version is also available through GitHub Actions builds. See [GitHub Action build for the Tauri desktop version](https://github.com/amll-dev/amll-ttml-tool/actions/workflows/build-desktop.yaml) for more details.

## Features

- Basic lyric input, editing, and timing tools
- Open and save lyrics in TTML format
- Configure lyric line behaviors, such as background vocals or duet lines
- Edit lyric metadata, including title, artist, NetEase Cloud Music ID, and more
- Split, merge, and move words
- Import lyrics from formats such as LRC, ESLyric, YRC, QRC, and Lyricify Syllable, with export support for some formats
- Import lyrics from plain text with special markers
- Customizable keyboard shortcuts

## Development

Building this project can be somewhat complex. If the written instructions feel too verbose, you can refer directly to the steps in [`build-desktop.yaml`](.github/workflows/build-desktop.yaml).

This project uses **PNPM only**, so make sure you have PNPM installed before getting started.

Clone the repository, then run the following commands in the project directory:

```bash
pnpm i           # Install dependencies
pnpm dev         # Start the development server
pnpm build       # Build the web version
pnpm tauri dev   # Start the Tauri desktop development environment
pnpm tauri build # Build the Tauri desktop version
```

## Contributions

We welcome all active code/translation contributions! We also welcome submissions of features and suggestions!

If you would like to provide translations for new languages, please refer to [`./src/i18n/index.ts`](./src/i18n/index.ts) and [`./locales/zh-CN/translation.json`](./locales/zh-CN/translation.json)!
