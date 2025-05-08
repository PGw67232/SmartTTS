# SmartTTS Node-RED flow

Działanie:

Jeśli nic nie jest odtwarzane, TTS wypowie wiadomość i ustawi poprzedni poziom głośności.

Jeśli głośnik odtwarza coś z URL, Spotify lub YouTube Music, TTS wypowie wiadomość, przywróci poprzedni poziom głośności i wznowi odtwarzanie.


Wymagania:
- Home Assistant

Jeśli używasz głośników Google Home:
- Oficjalna integracja Google Cast z Home Assistant

Jeśli używasz głośników Alexa:
- Niestandardowa integracja Alexa Media Player z Home Assistant (https://github.com/custom-components/alexa_media_player)

Jeśli używasz Spotify:
- Oficjalna integracja Spotify z Home Assistant
- Niestandardowa integracja Spotcast z Home Assistant (https://github.com/fondberg/spotcast)

Jeśli używasz YouTube Music:
- Niestandardowa integracja ytube music player z Home Assistant (https://github.com/KoljaWindeler/ytube_music_player)

Jak zacząć:
1. Kliknij dwukrotnie na node Smart TTS w zakładce subflows
2. Skonfiguruj swoje ustawienia
3. Gotowe!

Zmienne wejściowe:

msg.speaker (wymagane) – ID głośnika obsługującego Google Cast

msg.message (wymagane) – wiadomość TTS

msg.volume (opcjonalne) – głośność wiadomości TTS. Jeśli nie podano, głośność nie jest zmieniana

msg.tts_service (opcjonalne) – usługa TTS używana do wypowiedzenia wiadomości. Jeśli nie podano, używana jest domyślna

msg.tts_language (opcjonalne) – język wiadomości Google TTS
