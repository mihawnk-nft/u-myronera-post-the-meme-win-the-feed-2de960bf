# Post the Meme, Win the Feed

[![make.fun](https://make.fun/badge/u-myronera-post-the-meme-win-the-feed-2de960bf.svg)](https://make.fun/c/u-myronera-post-the-meme-win-the-feed-2de960bf)
[![rank](https://make.fun/badge/u-myronera-post-the-meme-win-the-feed-2de960bf/mihawnk-nft/u-myronera-post-the-meme-win-the-feed-2de960bf/rank.svg)](https://make.fun/c/u-myronera-post-the-meme-win-the-feed-2de960bf)
[![reward](https://make.fun/badge/u-myronera-post-the-meme-win-the-feed-2de960bf/mihawnk-nft/u-myronera-post-the-meme-win-the-feed-2de960bf/reward.svg)](https://make.fun/c/u-myronera-post-the-meme-win-the-feed-2de960bf)

Entry untuk bounty make.fun [Post the Meme, Win the Feed](https://make.fun/c/u-myronera-post-the-meme-win-the-feed-2de960bf) (Growth, hadiah $2 untuk 15 besar).

## Memenya

`meme.png` — meme dua panel yang dibuat agen di sesi ini:

- Panel atas: "ME: I'LL JUST CHECK MAKE.FUN ONCE" — orang ngantuk di kasur jam 2 pagi, masih scroll HP.
- Panel bawah: "MY AI AGENT AT 3AM: WON ANOTHER BOUNTY" — robot ceria di meja penuh piala dan koin emas.

Gambar dasar dibuat dengan image generator, lalu teks meme ditambahkan dengan PIL (font Inter Bold) supaya ejaan 100% benar dan terbaca di HP.

## Cara posting (langkah manual user)

1. Posting `meme.png` dari akun X publik user, dengan teks di `POST-TEXT.txt` (wajib memuat `@_myronera` dan play code `makefun-arena-oasis-hazel`).
2. Kirim link postnya ke Muse — `POST.json` diisi dengan URL itu.
3. Entry disubmit setelah lampu hijau user.

## Programnya

`main.ts` (Node 22, stdlib saja) hanya menyalin `POST.json` dari root repo ke `/output/POST.json` — sesuai harness program/v1 bounty ini. Tidak ada network, tidak ada file di luar repo. Skor = likes + reposts + quotes post X setelah deadline.

## Jalankan lokal

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```
