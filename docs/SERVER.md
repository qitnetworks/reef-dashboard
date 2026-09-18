# Server / VM edition 0.3.0

Free proprietary software · EN / PL / ES / FR / DE · Local data · Your aquarium name

**For ordinary Windows users, choose the separate Windows ZIP instead.** It includes everything: extract it and double-click **Start Aquarium.exe**. This server package is for an existing Linux x64 server/VM with Docker Engine and Compose. It is not a bootable VM image. [Docker installation](https://docs.docker.com/engine/install/).

## English

1. Extract this complete ZIP into a permanent folder on the server. Run `sh install.sh`. For Docker Desktop on Windows, use `install.cmd`.
2. The installer detects the home network and displays a clickable link and QR code. Open the link on your computer or scan the code on a tablet connected to the same home Wi-Fi. No need to look up an IP or type a password. This private link works once, for 10 minutes.
3. The setup assistant opens automatically: choose your aquarium name and language, click **Find my devices**, select the discovered devices and give them names. You can also start with the journal or try the demo. Device commands remain in ReefBeat; the dashboard only reads information.
4. Connect another tablet from **Settings → Connect a tablet**. Generate a fresh code if one expires. From the server terminal, `sh connect.sh` also creates a new code; Docker Desktop users can open `Connect.cmd`.
5. Keep the server running. On iPad, open the link in Safari and use Share → Add to Home Screen. Use Dashboard/full screen on the tablet. Network isolation or guest Wi-Fi can prevent discovery and tablet access; use the same home network. Advanced settings allow manual MAC/IP entry.

## Polski

1. Rozpakuj cały ZIP do stałego katalogu na serwerze i uruchom `sh install.sh`. Przy Docker Desktop w Windows użyj `install.cmd`. Zwykłym użytkownikom Windows polecamy osobny pakiet Windows, który nie wymaga Dockera.
2. Instalator sam ustala sieć i pokazuje klikalny link oraz QR. Otwórz link na komputerze albo zeskanuj kod tabletem w tej samej sieci domowej. Nie szukasz IP ani nie wpisujesz hasła. Prywatny link jest jednorazowy i ważny 10 minut.
3. Kreator uruchamia się automatycznie: wpisz nazwę akwarium, wybierz język, kliknij **Znajdź moje urządzenia**, zaznacz znalezione urządzenia i nadaj im nazwy. Możesz zacząć od dziennika albo demo. Sterowanie pozostaje w ReefBeat; aplikacja tylko odczytuje dane.
4. Kolejny tablet połącz przez **Ustawienia → Połącz tablet**. Wygasły kod zastąp nowym. Na serwerze nowy kod daje `sh connect.sh`; przy Docker Desktop służy do tego `Connect.cmd`.
5. Serwer musi być włączony. Na iPadzie otwórz link w Safari, następnie Udostępnij → Do ekranu początkowego. Uruchom Dashboard/pełny ekran. Gościnne Wi-Fi lub izolacja sieci mogą blokować połączenie — urządzenia powinny być w tej samej sieci domowej. Ręczne MAC/IP są w opcjach zaawansowanych.

## Español

1. Extrae todo el ZIP en una carpeta permanente del servidor y ejecuta `sh install.sh`. Con Docker Desktop en Windows, usa `install.cmd`. Para usuarios normales de Windows, el paquete Windows independiente no requiere Docker.
2. El instalador detecta la red y muestra un enlace y un código QR. Abre el enlace o escanea el QR con una tableta en la misma red doméstica. No necesitas buscar una IP ni escribir una contraseña. El enlace privado es de un solo uso y dura 10 minutos.
3. El asistente se abre automáticamente: nombre del acuario, idioma, **Buscar mis dispositivos**, selección y nombres. También puedes empezar con el diario o la demo. El control sigue en ReefBeat; esta aplicación solo lee datos.
4. Conecta otra tableta desde **Ajustes → Conectar una tableta**. Para otro código desde el servidor, ejecuta `sh connect.sh` o abre `Connect.cmd` con Docker Desktop.
5. Mantén el servidor encendido. En iPad: Safari → Compartir → Añadir a pantalla de inicio. Usa el panel/pantalla completa. Las redes de invitados o aisladas pueden bloquear la conexión. Las opciones avanzadas permiten introducir MAC/IP manualmente.

## Français

1. Extrayez tout le ZIP dans un dossier permanent du serveur et lancez `sh install.sh`. Avec Docker Desktop sous Windows, utilisez `install.cmd`. Le paquet Windows indépendant est plus simple et ne nécessite pas Docker.
2. Le programme détecte le réseau et affiche un lien et un QR code. Ouvrez le lien ou scannez le code avec une tablette sur le même réseau domestique. Aucune IP ni aucun mot de passe à saisir. Ce lien privé est utilisable une seule fois pendant 10 minutes.
3. L’assistant s’ouvre automatiquement : nom, langue, **Trouver mes appareils**, sélection et noms des appareils. Vous pouvez aussi commencer avec le journal ou la démo. Les commandes restent dans ReefBeat ; cette application lit uniquement les données.
4. Connectez une autre tablette depuis **Réglages → Connecter une tablette**. Pour un nouveau code depuis le serveur : `sh connect.sh`, ou `Connect.cmd` avec Docker Desktop.
5. Gardez le serveur allumé. Sur iPad : Safari → Partager → Sur l’écran d’accueil. Activez le tableau de bord/plein écran. Un réseau invité ou isolé peut bloquer la connexion. La saisie manuelle MAC/IP reste disponible dans les options avancées.

## Deutsch

1. Die vollständige ZIP in einen dauerhaften Ordner auf dem Server entpacken und `sh install.sh` ausführen. Mit Docker Desktop unter Windows: `install.cmd`. Für normale Windows-Nutzer ist das separate Windows-Paket einfacher und benötigt kein Docker.
2. Das Installationsprogramm erkennt das Heimnetz und zeigt einen Link und QR-Code. Den Link öffnen oder den Code mit einem Tablet im selben Heimnetz scannen. Keine IP-Suche und keine Passworteingabe nötig. Der private Link gilt einmalig für 10 Minuten.
3. Der Assistent startet automatisch: Aquarienname, Sprache, **Meine Geräte finden**, Geräte auswählen und benennen. Auch ein Start mit dem Protokoll oder der Demo ist möglich. Die Steuerung bleibt in ReefBeat; die App liest nur Daten.
4. Weitere Tablets über **Einstellungen → Tablet verbinden** verbinden. Einen neuen Code auf dem Server erzeugt `sh connect.sh`, mit Docker Desktop auch `Connect.cmd`.
5. Der Server muss eingeschaltet bleiben. Auf dem iPad: Safari → Teilen → Zum Home-Bildschirm. Dashboard/Vollbild einschalten. Gastnetze und Netzwerkisolierung können die Verbindung verhindern. Manuelle MAC/IP-Eingabe gibt es unter den erweiterten Optionen.

## Maintenance / administration

- Keep `.env` private. It contains the generated fallback administrator credentials (`reef` / `APP_PASSWORD`). The QR/link also grants administrator access. One shared installation, no per-user roles.
- Download a JSON backup in **Data & backups** before updates. Keep `.env` and the existing data volume, then run the new installer in the same folder. A release with a different Compose project name needs a JSON backup import into the new installation.
- Start: `docker compose up -d`. Stop: `docker compose stop`. **Never use `docker compose down -v` on real data.** The persistent volume stores the database. JSON backups include both modes, but not passwords; CSV contains measurements, not the entire journal. Restore makes a safety SQLite copy before replacing data. UI backup limit: 60 MB.
- If port 8787 is already used, edit `REEF_PORT` in `.env` before starting. The installer advertises the chosen port automatically. The host must allow this port on the home network. Do not forward it to the Internet; remote use needs a VPN or HTTPS reverse proxy.
- Device discovery checks one private IPv4 /24 explicitly selected in the assistant. Some networks require advanced configuration. Local device APIs are unofficial; model/firmware support can vary. ReefWave exposes a schedule, not measured flow. Missing readings are not replaced with demo data.
- Server image: Linux amd64/x86-64, not ARM64. A Proxmox VM needs Linux and Docker first; no Proxmox credentials are required by the application. Tablets are clients, not servers. No cloud account or source build required.
- Included: journal, CSV, JSON backups, recurring in-app reminders, warning thresholds, configurable slideshow. No cloud backup, push notifications or PDF/AI parsing. Source stays private; see LICENSE.txt and THIRD-PARTY-NOTICES.txt.
