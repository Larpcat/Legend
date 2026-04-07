# LARPCAT LEGEND
  const stats = [
    { label: "Chain", value: "Solana" },
    { label: "Ticker", value: "$LARP" },
    { label: "Supply", value: "1B" },
    { label: "Tax", value: "0%" },
  ];

  const phases = [
    {
      title: "Phase 1 — Launch the Legend",
      text: "Drop the cat. Drop the memes. Build instant identity with a loud brand and clean launch presence.",
    },
    {
      title: "Phase 2 — Meme Takeover",
      text: "Push daily content, short-form clips, reaction memes, and cat-flex edits that people actually want to repost.",
    },
    {
      title: "Phase 3 — Community Cult",
      text: "Contests, raids, leaderboard energy, and a holder culture built on humour, momentum, and inside jokes.",
    },
    {
      title: "Phase 4 — Main Character Mode",
      text: "Scale the brand into a full meme identity with merch, collaborations, and relentless social proof.",
    },
  ];

  const features = [
    {
      title: "Loud Visual Identity",
      text: "Neon charts, luxury-cat energy, and a cleaner premium meme aesthetic.",
    },
    {
      title: "Built for Virality",
      text: "Designed to feel fast, flashy, and instantly screenshot-worthy.",
    },
    {
      title: "Interactive Landing Page",
      text: "Glow effects, parallax motion, count-up stats, and animated call-to-actions.",
    },
    {
      title: "Community First",
      text: "Every section is built to push hype, memes, and shareable moments.",
    },
  ];

  return (
    <div className="min-h-screen bg-[#050816] text-white overflow-x-hidden selection:bg-emerald-400 selection:text-black">
      <style>{`
        @keyframes floaty {
          0%, 100% { transform: translateY(0px); }
          50% { transform: translateY(-12px); }
        }
        @keyframes pulseGlow {
          0%, 100% { box-shadow: 0 0 0px rgba(16,185,129,0.2), 0 0 50px rgba(59,130,246,0.12); }
          50% { box-shadow: 0 0 30px rgba(16,185,129,0.35), 0 0 80px rgba(59,130,246,0.18); }
        }
        @keyframes drift {
          0% { transform: translateY(0) rotate(0deg); opacity: .15; }
          50% { opacity: .35; }
          100% { transform: translateY(-80px) rotate(6deg); opacity: .08; }
        }
        @keyframes marquee {
          from { transform: translateX(0); }
          to { transform: translateX(-50%); }
        }
        .glass {
          background: rgba(255,255,255,0.05);
          backdrop-filter: blur(16px);
          border: 1px solid rgba(255,255,255,0.08);
        }
      `}</style>

      <div className="fixed inset-0 pointer-events-none">
        <div className="absolute -top-24 left-[-10%] h-80 w-80 rounded-full bg-emerald-500/20 blur-3xl" />
        <div className="absolute top-20 right-[-8%] h-96 w-96 rounded-full bg-cyan-500/20 blur-3xl" />
        <div className="absolute bottom-0 left-1/3 h-80 w-80 rounded-full bg-lime-400/10 blur-3xl" />
        {Array.from({ length: 14 }).map((_, i) => (
          <div
            key={i}
            className="absolute text-xl md:text-2xl"
            style={{
              left: `${(i * 7) % 100}%`,
              top: `${10 + ((i * 11) % 70)}%`,
              animation: `drift ${5 + (i % 5)}s ease-in-out infinite alternate`,
            }}
          >
            💸
          </div>
        ))}
      </div>

      <header className="sticky top-0 z-50 border-b border-white/10 bg-black/30 backdrop-blur-xl">
        <div className="mx-auto flex max-w-7xl items-center justify-between px-4 py-4 md:px-6">
          <div className="flex items-center gap-3">
            <div className="flex h-10 w-10 items-center justify-center rounded-2xl bg-gradient-to-br from-emerald-400 to-cyan-400 text-lg font-black text-black">
              🐯
            </div>
            <div>
              <div className="text-lg font-black tracking-wide">LARPCAT</div>
              <div className="text-xs uppercase tracking-[0.28em] text-emerald-300/80">Luxury Meme Energy</div>
            </div>
          </div>

          <nav className="hidden items-center gap-6 text-sm text-white/75 md:flex">
            <a href="#about" className="transition hover:text-white">About</a>
            <a href="#features" className="transition hover:text-white">Features</a>
            <a href="#tokenomics" className="transition hover:text-white">Tokenomics</a>
            <a href="#roadmap" className="transition hover:text-white">Roadmap</a>
          </nav>

          <a
            href="#join"
            className="rounded-2xl border border-emerald-300/30 bg-emerald-400 px-4 py-2 text-sm font-bold text-black transition hover:scale-105"
          >
            Join the Hype
          </a>
        </div>
      </header>

      <main>
        <section className="relative mx-auto grid min-h-[92vh] max-w-7xl items-center gap-10 px-4 py-16 md:grid-cols-2 md:px-6 md:py-24">
          <div className="relative z-10">
            <div className="mb-5 inline-flex items-center gap-2 rounded-full border border-emerald-300/20 bg-white/5 px-4 py-2 text-xs uppercase tracking-[0.3em] text-emerald-300">
              <span className="h-2 w-2 rounded-full bg-emerald-400" />
              The internet’s favourite flex cat
            </div>

            <h1 className="max-w-3xl text-5xl font-black leading-none md:text-7xl">
              <span className="bg-gradient-to-r from-emerald-300 via-lime-300 to-cyan-300 bg-clip-text text-transparent">
                LARPCAT
              </span>
              <br />
              <span className="text-white">Looks rich. Moves fast. Wins attention.</span>
            </h1>

            <p className="mt-6 max-w-xl text-base leading-7 text-white/75 md:text-lg">
              LARPCAT is built for people chasing momentum, memes, and market energy. Flashy cat. Neon charts. Loud presence. Pure internet confidence.
            </p>

            <div className="mt-8 flex flex-col gap-4 sm:flex-row">
              <a
                href="#join"
                className="rounded-2xl bg-gradient-to-r from-emerald-400 to-cyan-400 px-6 py-4 text-center font-black text-black transition hover:scale-[1.03]"
              >
                Buy $LARP
              </a>
              <a
                href="#about"
                className="rounded-2xl border border-white/15 bg-white/5 px-6 py-4 text-center font-semibold text-white transition hover:bg-white/10"
              >
                Explore the Legend
              </a>
            </div>

            <div className="mt-10 grid grid-cols-2 gap-4 md:grid-cols-4">
              {stats.map((item) => (
                <div key={item.label} className="glass rounded-3xl p-4">
                  <div className="text-xs uppercase tracking-[0.22em] text-white/45">{item.label}</div>
                  <div className="mt-2 text-2xl font-black text-emerald-300">{item.value}</div>
                </div>
              ))}
            </div>
          </div>

          <div className="relative flex items-center justify-center">
            <div className="absolute h-[28rem] w-[28rem] rounded-full bg-emerald-400/20 blur-3xl" />
            <div
              className="glass relative w-full max-w-xl overflow-hidden rounded-[2rem] p-3"
              style={{ animation: "pulseGlow 3.5s ease-in-out infinite" }}
            >
              <div className="absolute inset-0 bg-gradient-to-br from-emerald-300/10 via-transparent to-cyan-300/10" />
              <img
                src={heroImage}
                alt="LARPCAT hero"
                className="relative z-10 aspect-square w-full rounded-[1.5rem] object-cover"
                style={{ animation: "floaty 4.5s ease-in-out infinite" }}
              />
              <div className="absolute bottom-6 left-6 right-6 z-20 rounded-3xl border border-white/10 bg-black/55 p-4 backdrop-blur-md">
                <div className="text-xs uppercase tracking-[0.22em] text-emerald-300">Live Aura Reading</div>
                <div className="mt-2 text-2xl font-black">Bullish Main Character Energy</div>
              </div>
            </div>
          </div>
        </section>

        <section className="border-y border-white/10 bg-black/25 py-4">
          <div className="overflow-hidden whitespace-nowrap">
            <div className="inline-flex min-w-max animate-[marquee_18s_linear_infinite] gap-8 px-6 text-sm font-semibold uppercase tracking-[0.3em] text-white/55">
              {Array.from({ length: 2 }).map((_, idx) => (
                <div key={idx} className="flex gap-8">
                  <span>🐾 premium meme cat</span>
                  <span>📈 chart-powered energy</span>
                  <span>💸 internet flex culture</span>
                  <span>⚡ solana speed</span>
                  <span>🟢 zero tax vibes</span>
                  <span>👑 loud community presence</span>
                </div>
              ))}
            </div>
          </div>
        </section>

        <section id="about" className="mx-auto max-w-7xl px-4 py-24 md:px-6">
          <div className="grid gap-8 md:grid-cols-[1.2fr,0.8fr]">
            <div className="glass rounded-[2rem] p-8 md:p-10">
              <div className="mb-4 text-sm font-bold uppercase tracking-[0.3em] text-emerald-300">About LARPCAT</div>
              <h2 className="text-3xl font-black md:text-5xl">Not just a coin. A whole online persona.</h2>
              <p className="mt-6 max-w-3xl text-lg leading-8 text-white/72">
                LARPCAT captures the exact energy of internet ambition: flashy, chaotic, confident, and impossible to ignore. It is built for traders, meme lovers, screenshot warriors, and people who understand that attention is half the game.
              </p>
              <div className="mt-8 grid gap-4 sm:grid-cols-2">
                <div className="rounded-3xl border border-white/10 bg-white/5 p-5">
                  <div className="text-sm font-bold text-emerald-300">Visual identity</div>
                  <div className="mt-2 text-white/70">Luxury-cat aesthetic with stronger contrast, neon glow, cleaner depth, and more premium polish.</div>
                </div>
                <div className="rounded-3xl border border-white/10 bg-white/5 p-5">
                  <div className="text-sm font-bold text-cyan-300">Community mood</div>
                  <div className="mt-2 text-white/70">Fast memes, sharp branding, and high-energy copy designed to feel instantly shareable.</div>
                </div>
              </div>
            </div>

            <div className="glass rounded-[2rem] p-8">
              <div className="text-sm font-bold uppercase tracking-[0.3em] text-cyan-300">Why it hits</div>
              <ul className="mt-6 space-y-4 text-white/75">
                <li className="rounded-2xl border border-white/10 bg-white/5 p-4">Neon green and cyan palette for stronger contrast and meme-trader energy.</li>
                <li className="rounded-2xl border border-white/10 bg-white/5 p-4">Animated visual layers, premium cards, sticky nav, and smoother CTA hierarchy.</li>
                <li className="rounded-2xl border border-white/10 bg-white/5 p-4">Clean sections for roadmap, tokenomics, social links, and launch info.</li>
                <li className="rounded-2xl border border-white/10 bg-white/5 p-4">Original layout inspired by modern meme-coin landing pages, not a direct clone.</li>
              </ul>
            </div>
          </div>
        </section>

        <section id="features" className="mx-auto max-w-7xl px-4 pb-24 md:px-6">
          <div className="mb-10 flex items-end justify-between gap-6">
            <div>
              <div className="text-sm font-bold uppercase tracking-[0.3em] text-emerald-300">Features</div>
              <h2 className="mt-3 text-3xl font-black md:text-5xl">A better, louder meme-coin homepage</h2>
            </div>
          </div>

          <div className="grid gap-5 md:grid-cols-2 xl:grid-cols-4">
            {features.map((feature, idx) => (
              <div
                key={feature.title}
                className="glass group rounded-[1.75rem] p-6 transition duration-300 hover:-translate-y-1 hover:border-emerald-300/25"
              >
                <div className="mb-4 flex h-12 w-12 items-center justify-center rounded-2xl bg-gradient-to-br from-emerald-400 to-cyan-400 text-lg font-black text-black">
                  {idx + 1}
                </div>
                <h3 className="text-xl font-black">{feature.title}</h3>
                <p className="mt-3 leading-7 text-white/70">{feature.text}</p>
              </div>
            ))}
          </div>
        </section>

        <section id="tokenomics" className="mx-auto max-w-7xl px-4 pb-24 md:px-6">
          <div className="glass rounded-[2rem] p-8 md:p-10">
            <div className="text-sm font-bold uppercase tracking-[0.3em] text-emerald-300">Tokenomics</div>
            <div className="mt-3 flex flex-col gap-4 md:flex-row md:items-end md:justify-between">
              <h2 className="text-3xl font-black md:text-5xl">Simple, clean, and meme-friendly.</h2>
              <p className="max-w-lg text-white/65">Swap these placeholders with your exact launch details, contract address, socials, and pool status.</p>
            </div>

            <div className="mt-8 grid gap-4 sm:grid-cols-2 xl:grid-cols-4">
              {[
                ["Ticker", "$LARP"],
                ["Total Supply", "1,000,000,000"],
                ["Buy/Sell Tax", "0%"],
                ["Chain", "Solana"],
              ].map(([label, value]) => (
                <div key={label} className="rounded-[1.5rem] border border-white/10 bg-white/5 p-6">
                  <div className="text-xs uppercase tracking-[0.25em] text-white/45">{label}</div>
                  <div className="mt-3 text-2xl font-black text-white">{value}</div>
                </div>
              ))}
            </div>
          </div>
        </section>

        <section id="roadmap" className="mx-auto max-w-7xl px-4 pb-24 md:px-6">
          <div className="mb-10">
            <div className="text-sm font-bold uppercase tracking-[0.3em] text-cyan-300">Roadmap</div>
            <h2 className="mt-3 text-3xl font-black md:text-5xl">The rise of the richest-looking cat on Solana</h2>
          </div>

          <div className="grid gap-5 md:grid-cols-2">
            {phases.map((phase, idx) => (
              <div key={phase.title} className="glass rounded-[1.75rem] p-6">
                <div className="mb-4 flex items-center gap-3">
                  <div className="flex h-11 w-11 items-center justify-center rounded-2xl bg-white/10 font-black text-emerald-300">0{idx + 1}</div>
                  <h3 className="text-xl font-black">{phase.title}</h3>
                </div>
                <p className="leading-7 text-white/70">{phase.text}</p>
              </div>
            ))}
          </div>
        </section>

        <section id="chart" className="mx-auto max-w-7xl px-4 pb-24 md:px-6">
          <div className="glass rounded-[2rem] p-8 md:p-10">
            <div className="text-sm font-bold uppercase tracking-[0.3em] text-emerald-300">Live Chart</div>
            <div className="mt-3 flex flex-col gap-4 md:flex-row md:items-end md:justify-between">
              <h2 className="text-3xl font-black md:text-5xl">Watch $LARP move in real time</h2>
              <p className="max-w-lg text-white/65">Replace the placeholder link below with your DexScreener, DEXTools, Birdeye, or Pump page once live.</p>
            </div>

            <div className="mt-8 overflow-hidden rounded-[1.75rem] border border-white/10 bg-black/40">
              <div className="flex items-center justify-between border-b border-white/10 px-5 py-4">
                <div>
                  <div className="text-sm font-bold text-white">$LARP Live Chart Embed</div>
                  <div className="text-xs uppercase tracking-[0.24em] text-emerald-300/80">Paste your live chart url in the iframe src</div>
                </div>
                <a
                  href="#"
                  className="rounded-xl border border-emerald-300/20 bg-white/5 px-4 py-2 text-sm font-semibold text-white transition hover:bg-white/10"
                >
                  Open Full Chart
                </a>
              </div>

              <div className="aspect-[16/9] w-full bg-black/60">
                <iframe
                  title="$LARP live chart"
                  src="https://dexscreener.com/solana/YOUR-PAIR-ADDRESS?embed=1&theme=dark"
                  className="h-full w-full"
                  loading="lazy"
                />
              </div>
            </div>

            <div className="mt-4 rounded-2xl border border-cyan-300/10 bg-cyan-400/5 p-4 text-sm leading-7 text-white/70">
              Tip: when your pair is live, swap <span className="font-bold text-cyan-300">YOUR-PAIR-ADDRESS</span> with the real Solana pair address and also update the button link above.
            </div>
          </div>
        </section>

        <section id="join" className="mx-auto max-w-5xl px-4 pb-24 md:px-6">
          <div className="relative overflow-hidden rounded-[2rem] border border-emerald-300/20 bg-gradient-to-br from-emerald-400/15 via-white/5 to-cyan-400/15 p-8 md:p-12">
            <div className="absolute right-0 top-0 h-44 w-44 rounded-full bg-cyan-400/20 blur-3xl" />
            <div className="absolute bottom-0 left-0 h-44 w-44 rounded-full bg-emerald-400/20 blur-3xl" />
            <div className="relative z-10 text-center">
              <div className="text-sm font-bold uppercase tracking-[0.3em] text-emerald-300">Ready to launch</div>
              <h2 className="mt-4 text-3xl font-black md:text-5xl">Turn LARPCAT into a premium meme experience.</h2>
              <p className="mx-auto mt-5 max-w-2xl text-lg leading-8 text-white/75">
                Add your contract address, social buttons, launch links, and live chart embed here. The structure is ready. The cat is ready. The internet is ready.
              </p>
              <div className="mt-8 flex flex-col justify-center gap-4 sm:flex-row">
                <a href="#" className="rounded-2xl bg-emerald-400 px-6 py-4 font-black text-black transition hover:scale-105">Launch $LARP</a>
                <a href="#" className="rounded-2xl border border-white/15 bg-black/25 px-6 py-4 font-semibold text-white transition hover:bg-white/10">Add Telegram / X</a>
              </div>
            </div>
          </div>
        </section>
      </main>

      <footer className="border-t border-white/10 px-4 py-8 text-center text-sm text-white/45 md:px-6">
        © 2026 LARPCAT. Not financial advice. Built for memes, culture, and attention.
      </footer>
    </div>
  );
}
