# ISECO SOS Mobile

Capacitor shell for the current ISECO patient SOS experience.

## Build
1. npm install
2. npx cap add android
3. npx cap add ios
4. npx cap sync
5. Android: npx cap open android
6. iOS: npx cap open ios

## Release hardening required before store submission
- Replace remote-web shell with bundled app UI / native integrations where store review requires it.
- Implement native microphone/audio recording and durable upload; current web app primarily performs speech-to-text/audio-level monitoring.
- Implement native foreground/background location with explicit consent and privacy disclosures.
- Add production authentication/API security and remove public fallback tokens.
- Enable proper RLS/policies for patient data and complete privacy/data-safety declarations.
- Connect real messaging/telephony providers before claiming SMS/WhatsApp/call delivery.
- Add incident status polling so pre-arrival prompts stop at ARRIVED_SCENE.
- Add app icons, splash assets, screenshots, privacy policy, support URL and store metadata.

Package/bundle ID: in.iseco.sos
