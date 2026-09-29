# TinkX TV

Videos and songs for the TinkX owner TV.

The TV only plays what is listed in `tv.json`. To add something:

1. Upload the file to `videos/` (MP4, H.264 + AAC, under 25 MB) or `music/` (MP3).
2. Optionally upload a picture to `thumbs/`.
3. Add an entry to `tv.json`:

```json
{ "id": "my-clip", "title": "My Clip", "artist": "Me", "type": "video", "file": "videos/My Clip.mp4", "thumb": "thumbs/my-clip.jpg" }
```

`type` is `video` or `music`. `id` must be unique (letters, numbers, dashes).
Everyone's TV picks up the change the next time the TV is spawned.
