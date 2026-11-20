* { box-sizing: border-box; }
:root {
  --ink: #151411;
  --paper: #f6f3ed;
  --gold: #c9ad78;
  --muted: #8e877a;
}
html { scroll-behavior: smooth; }
body { margin: 0; background: var(--paper); color: var(--ink); font-family: "Montserrat", Arial, sans-serif; }
a { color: inherit; text-decoration: none; }
.site-header {
  height: 96px; padding: 10px 5vw; display: flex; align-items: center;
  justify-content: space-between; background: #fff; position: relative; z-index: 5;
}
.brand-mark { display: flex; align-items: center; height: 76px; width: 132px; overflow: hidden; }
.brand-mark img { width: 100%; height: 100%; object-fit: contain; }
.main-nav { display: flex; gap: clamp(18px, 3vw, 48px); align-items: center; }
.main-nav a, .social-links, .role, .eyebrow, .made-in, .site-footer small {
  font-size: 10px; letter-spacing: .22em; font-weight: 500;
}
.main-nav a { transition: color .2s; }
.main-nav a:hover, .social-links a:hover { color: #a27e45; }
.menu-toggle { display: none; border: 0; background: transparent; font-size: 25px; }
.hero { position: relative; background: #191816; overflow: hidden; }
.hero-image { display: block; width: 100%; height: auto; max-height: 690px; object-fit: cover; }
.hero-scroll { position: absolute; bottom: 18px; left: 50%; transform: translateX(-50%); color: white; font-size: 25px; opacity: .8; }
.section-panel { padding: 105px 8vw; text-align: center; }
.eyebrow { color: #9b8055; line-height: 1.8; }
h1, h2, h3 { font-family: "Cormorant Garamond", Georgia, serif; font-weight: 500; }
.story h1 { font-size: clamp(34px, 5vw, 62px); line-height: 1.02; letter-spacing: .035em; margin: 25px 0 12px; }
.story h1 em { color: #9b8055; font-weight: 400; }
.ornament { color: var(--gold); font-size: 25px; margin: 24px 0; }
.story-copy { max-width: 760px; margin: 0 auto; color: #57534c; font-family: "Cormorant Garamond", Georgia, serif; font-size: clamp(20px, 2vw, 25px); line-height: 1.55; }
.made-in { margin-top: 35px; color: #9b8055; }
.heritage-banner {
  min-height: 440px; display: grid; place-items: center; text-align: center; color: white;
  background: linear-gradient(90deg, rgba(12,12,12,.55), rgba(12,12,12,.24)), url("assets/internal-background.png") center/cover no-repeat;
  position: relative;
}
.heritage-content { padding: 55px 20px; text-shadow: 0 2px 14px #000; }
.heritage-content h2 { font-size: clamp(32px, 5vw, 58px); letter-spacing: .14em; margin: 18px 0; }
.heritage-content h2 span { color: var(--gold); }
.heritage-content p:last-child { font-family: "Cormorant Garamond", Georgia, serif; font-size: 23px; }
.people { background: #eee9df; }
.people h2, .contact h2 { font-size: clamp(30px, 4vw, 48px); letter-spacing: .06em; margin: 18px 0; }
.people-grid { max-width: 1000px; margin: 48px auto 0; display: grid; grid-template-columns: repeat(4, 1fr); gap: 22px; }
.person { border-top: 1px solid #c7b48e; padding: 25px 12px 18px; }
.role { color: #9b8055; display: block; }
.person h3 { font-size: 25px; margin: 12px 0; }
.launch {
  min-height: 520px; display: grid; place-items: center; text-align: center; color: #f4e6c8;
  background: linear-gradient(rgba(10,10,10,.58), rgba(10,10,10,.7)), url("assets/internal-background.png") center/cover no-repeat;
  padding: 80px 20px;
}
.launch-inner { max-width: 760px; }
.launch h2 { font-size: clamp(58px, 10vw, 112px); line-height: .78; letter-spacing: .12em; margin: 35px 0; }
.launch h2 span { font-size: .76em; }
.gold-rule { width: 110px; height: 1px; background: var(--gold); margin: 35px auto; }
.launch-inner > p:not(.eyebrow) { letter-spacing: .22em; font-size: 11px; line-height: 2; }
.outline-button { display: inline-block; border: 1px solid var(--gold); padding: 15px 28px; margin-top: 25px; font-size: 10px; letter-spacing: .2em; transition: background .2s, color .2s; }
.outline-button:hover { background: var(--gold); color: #171512; }
.contact { background: #f8f6f1; }
.contact-grid { max-width: 900px; margin: 42px auto 30px; display: grid; grid-template-columns: repeat(3, 1fr); gap: 25px; }
.contact-grid p { font-family: "Cormorant Garamond", Georgia, serif; font-size: 22px; }
.social-links { display: flex; justify-content: center; gap: 15px; margin-top: 35px; }
.site-footer { background: #151411; color: #e8dfcf; text-align: center; padding: 35px 20px 28px; }
.site-footer img { width: 115px; height: 85px; object-fit: contain; background: #fff; }
.site-footer p { font-size: 9px; letter-spacing: .2em; margin: 14px 0 24px; }
.site-footer small { color: #b4a78e; font-size: 8px; }
@media (max-width: 700px) {
  .site-header { height: 76px; }
  .brand-mark { width: 104px; height: 62px; }
  .menu-toggle { display: block; color: #171512; }
  .main-nav { display: none; position: absolute; top: 76px; left: 0; right: 0; background: #fff; padding: 22px; flex-direction: column; gap: 22px; border-top: 1px solid #eee; }
  .main-nav.open { display: flex; }
  .hero-image { min-height: 280px; object-fit: cover; object-position: center; }
  .section-panel { padding: 72px 7vw; }
  .people-grid { grid-template-columns: repeat(2, 1fr); gap: 10px; margin-top: 30px; }
  .person h3 { font-size: 21px; }
  .heritage-banner { min-height: 340px; }
  .contact-grid { grid-template-columns: 1fr; gap: 8px; }
