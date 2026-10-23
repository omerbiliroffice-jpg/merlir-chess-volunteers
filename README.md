# MERLIR CHESS — Volunteer Interest List

**Cinematic Chess — Every Game Is a Movie.**

> **This is not the MERLIR CHESS source code repository.** This repository only describes the project and hosts a volunteer interest list. The game's source code is private and is not open source.

## Who is behind this

MERLIR CHESS is an **independent game development project** run by one person, **Ömer Bilir** ([@omerbiliroffice-jpg](https://github.com/omerbiliroffice-jpg)).

- MERLIR STUDIO and MERLIR GAMES are **project brand names only**. They are not registered companies or legal entities, and they are not registered trademarks.
- There is no company, no paid staff, and no sales yet.
- The game is being developed with the **intention of a future commercial release**.

## The vision

MERLIR CHESS is a planned chess game for Apple platforms (iPhone, iPad and Mac). It keeps the rules of classical chess exactly as they are — and turns significant moves into short, dramatic, sound-designed battle scenes.

We are not simply adding videos to a chess game. We are designing a cinematic chess experience where the meaning of each significant move can trigger a corresponding dramatic scene, presented through a native Apple video system inspired by the visual behavior of live-stream animated gift effects.

## Planned Gameplay & Cinematic Presentation System

> Everything in this section is **planned**. None of it is implemented yet.

**What makes it different.** Most chess apps animate pieces. MERLIR CHESS plans to understand what a move means — an attack, a defense, a sacrifice, a check, a comeback, a promotion, a checkmate — and respond with a short scene that tells that story. Cinematics never change the rules or the game state.

**Visual reference.** On live-stream platforms, an animated gift effect appears briefly on top of the stream while the stream keeps going (TikTok LIVE is a well-known example). MERLIR CHESS takes inspiration from that presentation style only: instead of gifts, chess moves trigger short scenes. The game does not use, depend on, or integrate with TikTok or any of its technology, and has no affiliation with TikTok. TikTok is a trademark of its respective owner.

**How a move becomes a scene (example).**

1. The player's knight captures a bishop.
2. The chess engine validates the move.
3. An event analysis step decides what the move means (here: an attack).
4. A cinematic decision system picks a matching short scene.
5. The scene plays in the cinematic area at the bottom of the game screen, with synchronized sound.
6. When it ends, the area returns to its normal state.

**Screen layout.** The **interactive chessboard** stays the main interface. A **cinematic presentation area** at the bottom of the screen plays scenes as part of the game screen — no separate video page. It may briefly overlap parts of the interface, but important game information stays accessible, and players can skip or turn off cinematics.

**Planned architecture.**

```
ChessCore / MerlirEngine
  → Move Validation
  → Drama & Event Analysis
  → Cinematic Intent
  → Presentation Controller
  → Native Apple Video Playback (AVFoundation)
```

**Planned video targets (development goals, not final decisions).** HEVC (H.265) in MP4 or MOV · 1080 × 1920 source (scaled or cropped to the cinematic area) · 3–5 s standard scenes, 5–15 s key scenes · synchronized sound · AVFoundation / AVPlayer with preloading · HEVC with Alpha for some overlay effects, where useful.

## Where we are today

- **Implemented and tested:** chess engine (legal moves, check, checkmate, stalemate, castling, en passant, promotion, FEN validation, SAN move list) with automated tests; SwiftUI board screen connected to the engine; iPhone / iPad app target that builds on macOS CI.
- **In progress:** simulator UI tests and on-device testing.
- **Not started:** cinematic system, video content, bots, save/resume, Mac version.

## Independent contributor model

> We welcome independent, optional and unpaid code contributions from developers who voluntarily wish to support MERLIR CHESS. Contributors are free to choose whether, when and how to contribute, without mandatory working hours or ongoing work obligations. Any accepted contributions will be governed by separately agreed written intellectual property and commercial licensing terms. This model does not override applicable employment laws where the actual relationship legally constitutes employment.

Contributors are not employees. Possible contributions will be shared as optional opportunities, never as work orders, and can be freely accepted or declined. Not every submitted contribution will be accepted.

## How contributing would work — two separate stages

**Stage A — Volunteer interest (not open yet).** When it opens, you will be able to tell us which areas interest you. That's all.
- No contract, no task, no code accepted, no repository access.
- No obligation for you to ever contribute, and no obligation for us to offer you anything.
- Signing up does **not** mean agreeing to any contributor agreement.

**Stage B — Independent code contribution (later, only if both sides separately decide).** Before any code is written, you would receive in writing: the proposed contribution's scope, confirmation that it is unpaid, the intellectual property terms (an individual contributor license agreement), access and security limits, and how contributions are reviewed, accepted or rejected. No code is included in the project before the written license is signed. You can say no at any point.

## Honest terms

- Contributions would be **unpaid**. No salary, payment, revenue share, equity, or future job offer is promised or implied.
- The game may in the future be **sold as a paid game, licensed, or sold as a project**.
- No working hours, shifts, mandatory meetings, quotas, attendance or mandatory deadlines. You choose whether, when and how to contribute, and you can stop at any time without giving a reason.
- We never ask for any fee or payment from volunteers.
- We do not promise visibility or career opportunities. Being named in an acknowledgements section is optional and only for accepted contributions.
- Stage B is open only to people **18 or older**.
- Your intellectual property is not transferred automatically to anyone. Rights in accepted contributions are set out in a separate written license.
- We do not accept artwork or visual asset contributions.
- These terms do not override applicable employment laws.

## Areas of interest

Swift / SwiftUI · AVFoundation / AVPlayer · iOS video playback optimization · HEVC video / alpha compositing · SpriteKit / SceneKit / RealityKit · chess engine architecture · chess AI / bot development · event-driven animation systems · iPhone / iPad / Mac UI development · Apple platform testing · performance and memory optimization

These are potential areas only. No tasks are being offered at this time.

## Interest list status: not open yet

**Volunteer applications are not being collected at this time.** Issues are disabled in this repository.

- To follow the project, you can **watch or star** this repository. Stars and watches are only a way to follow updates; they are **not** volunteer applications and create no relationship or obligation.
- Please **do not send applications** by email or through other channels yet.
- When the interest list opens, it will be announced here, together with its privacy notice.

See [PRIVACY.md](PRIVACY.md) for how personal data is handled in the meantime.

## Rights in this repository

This repository is **not** licensed as open source. Its text and materials are © Ömer Bilir, all rights reserved, except for the viewing and forking that [GitHub's Terms of Service](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service) allow for public repositories.

---

## Türkçe özet

**Bu depo MERLIR CHESS'in kaynak kod deposu değildir.** Sadece projeyi tanıtır ve gönüllü ilgi listesini barındırır. Oyunun kaynak kodu özeldir ve açık kaynak değildir.

MERLIR CHESS, **Ömer Bilir** tarafından yürütülen bağımsız bir oyun geliştirme projesidir. MERLIR STUDIO ve MERLIR GAMES sadece proje marka adlarıdır; kayıtlı şirket, tüzel kişi veya tescilli marka değildir. Şu an şirket, ücretli çalışan veya satış yoktur; oyun ileride ticari olarak yayımlanmak üzere geliştirilmektedir.

Oyun, klasik satranç kurallarını değiştirmeden önemli hamleleri ekranın alt bölümünde oynatılan kısa, sesli sinematik savaş sahnelerine dönüştürmeyi hedefler. Sunum tarzı canlı yayınlardaki animasyonlu hediye efektlerinden ilham alır; TikTok ile hiçbir bağlantı veya teknoloji ilişkisi yoktur. Sinematik sistem henüz planlama aşamasındadır.

Katkı iki ayrı aşamadan oluşur. **A Aşaması (henüz açık değil):** Açıldığında sadece ilgi bildirilecek; sözleşme, görev, kod kabulü veya depo erişimi olmayacak, kimse için yükümlülük doğmayacak ve bir katkı sözleşmesi kabul edilmiş sayılmayacak. **B Aşaması (ileride, iki taraf da isterse):** Kod yazılmadan önce görev kapsamı, ücretsizlik, fikrî mülkiyet koşulları, erişim sınırları ve kabul yöntemi yazılı olarak sunulur.

**Bağımsız katkı modeli:** Katkıcılar çalışan değildir; katkı sunup sunmayacaklarına, ne zaman ve nasıl sunacaklarına kendileri karar verir. Görev önerileri iş emri değil, isteğe bağlı katkı fırsatıdır; özgürce kabul veya reddedilebilir. Sunulan her katkının kabul edilmesi zorunlu değildir. Katkı ücretsizdir; maaş, ödeme, gelir payı, hisse veya iş teklifi sözü yoktur. Çalışma saati, vardiya, zorunlu toplantı, kota veya zorunlu teslim tarihi yoktur; katkıcı istediği zaman gerekçe göstermeden bırakabilir. Fikrî mülkiyet hakları kendiliğinden kimseye geçmez; kabul edilen katkılar ayrı yazılı lisansla düzenlenir. Bu model, ilişkinin fiilen iş ilişkisi olduğu durumlarda uygulanacak zorunlu iş hukuku kurallarını ortadan kaldırmaz. B Aşaması 18 yaş ve üzeri kişilere açıktır. Görsel katkı kabul edilmez. **İlgi listesi henüz açık değildir;** şu an gönüllü başvurusu toplanmıyor ve issue'lar kapalıdır. Projeyi izlemek isteyenler depoyu takip edebilir veya yıldızlayabilir; bunlar başvuru sayılmaz ve hiçbir ilişki veya yükümlülük doğurmaz. Lütfen henüz e-postayla veya başka bir kanaldan başvuru göndermeyin. Kişisel veriler hakkında bilgi için [PRIVACY.md](PRIVACY.md) dosyasına bakın.
