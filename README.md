
Desi HD Maker - Ready-to-build React + Capacitor project
-------------------------------------------------------

APP: Desi HD Maker (AI-enhance mode)

What's included:
- Minimal Vite + React web app (src/)
- ffmpeg.wasm integration for on-device enhancement
- PWA manifest + icon SVG
- Instructions to wrap with Capacitor and build APK

Steps to build APK (on your PC with Node.js + Android Studio installed):

1. Unzip project and open terminal in the project folder:
   cd desi-hd-maker
   npm install

2. (Optional) Test in browser:
   npm run dev
   Open http://localhost:5173

3. Build web assets:
   npm run build

4. Initialize Capacitor and add Android:
   npm install @capacitor/cli @capacitor/core
   npx cap init "Desi HD Maker" com.yourname.desi_hd_maker
   npx cap add android
   npx cap copy

5. Open Android project in Android Studio:
   npx cap open android
   Then run on device or create signed APK via Build -> Generate Signed Bundle / APK

Notes:
- ffmpeg.wasm is heavy. For better performance and true AI upscaling, consider a server-based Real-ESRGAN pipeline (not included).
- If you want, I can provide a pre-built debug APK. To provide that I would need a place to upload it to or a method to transfer.

