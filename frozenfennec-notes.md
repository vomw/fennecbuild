Settings below notes in quotes can be adjusted by naviating to the special `about:config` page.

Known Issues
------------

- Some fonts, particularly ones used for displaying Korean text, may not display correctly due the font restrictions by `privacy.resistFingerprinting`.
- Dark mode for websites is disabled due to `privacy.resistFingerprinting`.
- Refresh rate is capped to 60hz due to `privacy.resistFingerprinting`.
- Multitouch gestures will not work due to `privacy.resistFingerprinting`.

Workarounds
-----------

- The JavaScript JIT is disabled to increase security at the cost of slowing down webapps, complex websites, and the PDF viewer. Change `javascript.options.ion` and `javascript.options.baselinejit` to true to restore their performance.
- Referrers are stripped. This often breaks loading of images on websites with hotlink protection. Change `network.http.referer.XOriginPolicy` from 2 to 1, this is however a privacy risk.
- Visted link highlighting is disabled. Change `layout.css.visited_links_enabled` to true if needed, this is however a privacy risk.
- WebAssembly is disabled. This is often used for web apps. Change `javascript.options.wasm` to true if needed, this is however a security risk.
- WebGL is disabled. This is often used for games and maps. Change `webgl.disabled` to false if needed, this is however a privacy risk.
- WebRTC is disabled. This is often used for audio/video calls. Change `media.peerconnection.enabled` to true if needed, this is however a privacy risk.
- Strict certificate revocation checks are enabled. The CA revocation servers are frequently down/blocked/inaccessible and will result in a "Secure Connection Failed" error. Change `security.OCSP.require` to false, this is however a security and privacy risk.
- Safe renegotiation is required for connections. Some few websites do not support this and will result in a "Secure Connection Failed" error. Change `security.ssl.require_safe_negotiation` to false, this is however a security and privacy risk.
- Strict certificate pinning is enabled. If you are using a proxy or VPN that does HTTPS manipulation you'll encounter a "Secure Connection Failed" error. Change `security.cert_pinning.enforcement_level` from 2 to 1, this is however a security and privacy risk.
- User-added CA certificates are not trusted, you can optionally enable them at your own extreme risk: Settings > About FrozenFennec > Tap Fennec logo until debug settings are enabled > back a menu > Secret Settings > Use third party CA certificates > Enabled, this is however a security and privacy risk.
- If the button to "Accept the risk & continue" doesn't work change `browser.ssl_override_behavior` from 1 to 2.
- If you have issues playing some videos change `media.android-media-codec.preferred` from true to false. This may reduce battery life.
- If audio/video content fails to play in private tab. Change `browser.privatebrowsing.forceMediaMemoryCache` to false, this is however a privacy risk.
