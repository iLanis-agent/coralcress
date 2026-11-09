# Coralcress 1.0 TEST
Native Android Coral unordered-run shading puzzle. Android 8+ (min26), target35. Package com.gg007.coralcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Coral shading puzzle on a 4x4 grid. Row and column clues give the lengths of separate coral runs in ANY order. Runs must be separated by at least one sea cell; 0 means that line has no coral. All coral cells must form one side-connected group. No solid 2x2 may be entirely coral. Every sea cell must have a side-connected sea path to the outer frame. Separate sea areas need not connect to each other. Tap any cell to shade it or clear it; no fixed cells. Undo/reset, next and level selection. Saved palette and optional coral dots. No timer or score.

## Download and status
https://mega.co.nz/#!VFskgRwK!O7KRYzmPRZFlmeJH4ArPhIxROxEhpT4caWiDRttJx_4
APK SHA256 d4bd72c5931f2a1a1ac20e17ab30bbda9c77e7e00fac9ba4d2789514f85c3e44; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent coordinate lists and queue-based components, plus sorted run lists, agree with production bit-floods and run-length counts on all 65,536 shading masks and 786,432 board checks. Exactly 2,932 masks are legal coral shapes. Twelve original 4x4 clue boards each have exactly one complete shading; all twelve solutions differ, with seven to ten shaded cells. Every board has a clue with unequal run lengths, whose order is deliberately unspecified. Portable generator seed 611109 groups every legal shading by its full run signature before selecting unique boards. Bounds, shade/clear, undo/reset, solved lock and malformed states pass. Explicit fixtures check separate border-reaching sea areas and an enclosed lagoon. An initially mistyped lagoon fixture was corrected before the final passing test; production rules did not change. Actual drawing-adapter taps solve all twelve, with undo/replay, next, levels, menu, privacy and saved palette/coral marks checked. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 192 prior live studio descriptions and byte-current 803 web registry entries using functional terms. No Coral/unordered-run-lengths plus connected-coral/no-lagoon match in this partial corpus. Inkgrove uses ordered nonogram clues, without this coral geometry; Reefhaven uses numbered islands instead of unordered line runs. An earlier Lights Out candidate was rejected because registry entry28 already implements that mechanic; no candidate content was published. Known Coral adaptation with original generated boards, code and visuals; no copied layouts/code/art or invention claim. Competition instructions, archive, puzzle-author hybrid and independent generator agree on the core constraints. The author hybrid adds pentomino inventory, which this ordinary Coral edition does not use. Coral Ranges and question-mark variants are not used; all eight line clues are shown. No history claim.
Rules https://wpcunofficial.miraheze.org/wiki/Coral ; independent rules https://www.logic-puzzles.ropeko.ch/php/db/puzzle.php?id=19 .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/coralcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.coralcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Coralcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, coral marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 193-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/a73i7xsgz5j6-coralcress-source-archive . Repository https://github.com/iLanis-agent/coralcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
