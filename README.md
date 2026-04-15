# Spotify Video Blocklist

A minimal DNS blocklist focused on blocking Spotify video content only.

## Purpose

This list blocks:
- Video podcasts
- Video clips
- Canvas animations (looping visuals in songs)

While keeping:
- Audio playback working
- App functionality intact

## Usage (Pi-hole)

Add this URL to your Pi-hole:

https://raw.githubusercontent.com/PatrickKalka-SeriousByte/spotify-video-blocklist/refs/heads/main/spotify-video-blocklist.txt

Then:
- Group Management → Adlists
- Add the URL
- Update Gravity

## Expected Behavior

| Feature            | Result |
|--------------------|--------|
| Music playback     | works |
| Video podcasts     | blocked |
| Canvas animations  | blocked |
| Covers/UI          | works |

## Limitations

- No official domain list exists from Spotify
- Domains may change at any time
- Some video content may be delivered via shared CDNs

## Source & Methodology

Domains are identified via:
- DNS / Pi-hole query logs
- Network traffic analysis
- Community validation

## Contributing

If you find:
- new video domains
- false positives

Please open an issue.

## License

MIT License
