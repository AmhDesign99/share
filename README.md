# LAN Share — 5 Digit P2P

Browser-only file/folder sharing using a 5-digit session code and WebRTC/PeerJS.

## GitHub Pages
Upload `index.html` to your repository and enable GitHub Pages.

## Pairing
1. Sender clicks **Buat Sesi** and shares the 5-digit code.
2. Receiver enters the code and clicks **Gabung Sesi**.
3. When status becomes CONNECTED, choose files/folders and send them.

## Networking note
PeerJS Cloud is used only for signaling/brokering. WebRTC carries file data directly when a direct peer route is possible. The app sets an empty ICE server list to focus on local/direct connectivity and avoid TURN relays.

Opening GitHub Pages and signaling require a small amount of internet. File payloads are not uploaded to GitHub.
