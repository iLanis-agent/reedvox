# Reedvox 1.0 TEST
Native Android Voxas strip-partition puzzle. Android8+ (min26), target35. Package com.gg007.reedvox.

## Rules
Voxas: divide every cell into straight 1x2 or 1x3 rooms, horizontal or vertical. Tap an internal edge to add or remove a fence. Dotted borders are fixed fences between different rooms. White dots: same size AND same orientation. Black dots: different size AND different orientation. Gray dots: exactly one of size or orientation is the same. Undotted edges carry no relation clue. Every region must be a complete straight strip, with no redundant fences inside it. Twelve unique 4x3 boards and unique solutions, each includes all three dot types. Undo/reset/next/level selection and saved reed palette/dot-letter settings.

## Download and status
https://mega.co.nz/#!sVVBVbIK!yljqYyHtYXR-p97_4RhXizXqoEa_G5lmYAu-6VZzfVs
APK SHA256 b6bf0c338538dd40da7c9b00bbdfba0e5d93396c59b7a9507dfe538467f53ea9; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Independent exact-cover enumeration produces all41 possible straight-strip partitions of the 4x3 grid. Its set-based size/orientation relation oracle agrees with production flood-fill/bounding-box validation for all1572864 fence masks across twelve boards. Twelve distinct clue arrays and unique partitions. Bounds, invalid masks/levels, fixed-dot locks, solved-input lock, solve, undo and reverse-order replay pass. Actual archived generator regeneration and archived Java tests pass. Drawing-adapter border taps, navigation, saved settings, completion marks, next, levels and privacy pass. Actual game/solved/menu/settings/levels/privacy drawing pixels inspected, not phone screenshots. Phone runtime, performance and external browser handoff QA remain incomplete. Signed TEST only, not final or Play published.

## Functional difference
Live803-entry web registry,120 recovered partial README records and semantic review of all146 prior cumulative card mechanics found no Voxas match. Reedtatami uses thin strip rooms with arrows counting room size and rooms ahead, plus no four-room corners. Reedvox instead compares adjacent rooms by two independent traits, size and orientation, via white/black/gray fixed border clues. Matgrove uses square/wide/tall symbols and forbids four corners; Dominowell only tiles dominoes. Reedvox allows both 2/3-cell straight strips and has no four-corner prohibition. Known Voxas genre by Eric Fox, not a global invention. Corpus is partial. Rules verified at https://xavierbdm.fr/en/en-voxas-rules/ https://logicmastersindia.com/daily/?contest=D202204V and https://ericfox53.blogspot.com/2022/02/446-voxas.html .

## Build
JDK17 and AndroidSDK platform35/build-tools35.0.0. Run python generate-levels.py to reproduce levels.json; Board.java embeds the generated clues and solutions. javac -d /tmp/reed-test src/com/gg007/reedvox/Board.java BoardTest.java and java -cp /tmp/reed-test com.gg007.reedvox.BoardTest. bash build.sh builds an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Reedvox runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Reed palette, dot letters and solved-board marks stay in the app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon copied byte-for-byte from preserved original. Menu studio link https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/gyje1hc9n076-reedvox-source-archive with exact cumulative147-card studio HTML, published compact studio source and searchable App Factory catalog source/updater. GitHub https://github.com/iLanis-agent/reedvox holds README only; full Git source commit remains pending. Site publication is checked separately before notification. No Pages settings changes or Play rollout. Updated November7,2026.
