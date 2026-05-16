export default function FearlessFitLuxuryHomepage() {
  return (
    <div className="bg-black text-white min-h-screen font-sans overflow-hidden">
      {/* NAVBAR */}
      <nav className="flex items-center justify-between px-8 py-6 border-b border-white/10 backdrop-blur-md sticky top-0 z-50 bg-black/70">
        <div className="flex items-center gap-3">
          <img
            src="/logo.png"
            alt="Fearless Fit Logo"
            className="w-12 h-12 object-contain"
          />
          <h1 className="text-2xl font-bold tracking-[0.2em] uppercase">
            Fearless Fit
          </h1>
        </div>

        <div className="hidden md:flex gap-8 text-sm uppercase tracking-widest">
          <a href="#shop" className="hover:text-gray-400 transition">
            Shop
          </a>
          <a href="#drops" className="hover:text-gray-400 transition">
            New Drops
          </a>
          <a href="#lookbook" className="hover:text-gray-400 transition">
            Lookbook
          </a>
          <a href="#contact" className="hover:text-gray-400 transition">
            Contact
          </a>
        </div>
      </nav>

      {/* HERO */}
      <section className="relative h-screen flex items-center justify-center text-center px-6">
        <div className="absolute inset-0">
          <img
            src="https://images.unsplash.com/photo-1523398002811-999ca8dec234?q=80&w=1974&auto=format&fit=crop"
            className="w-full h-full object-cover opacity-40"
            alt="Streetwear model"
          />
          <div className="absolute inset-0 bg-gradient-to-b from-black/40 to-black" />
        </div>

        <div className="relative z-10 max-w-5xl">
          <p className="uppercase tracking-[0.4em] text-gray-300 mb-6 text-sm">
            Luxury Streetwear
          </p>

          <h1 className="text-6xl md:text-8xl font-black leading-none uppercase mb-6">
            Fearless
            <br />
            Fit
          </h1>

          <p className="text-gray-300 text-lg md:text-xl max-w-2xl mx-auto mb-10">
            Built for the fearless. Hood rich aesthetic with oversized fits,
            luxury vibes, and premium streetwear energy.
          </p>

          <div className="flex gap-4 justify-center flex-wrap">
            <button className="px-8 py-4 bg-white text-black font-bold rounded-full hover:scale-105 transition uppercase tracking-wider">
              Shop Now
            </button>

            <button className="px-8 py-4 border border-white/40 rounded-full hover:bg-white hover:text-black transition uppercase tracking-wider">
              New Drop
            </button>
          </div>
        </div>
      </section>

      {/* FEATURED */}
      <section id="shop" className="px-6 md:px-14 py-24">
        <div className="flex items-center justify-between mb-12">
          <h2 className="text-4xl md:text-5xl font-black uppercase">
            Featured Drop
          </h2>

          <button className="border border-white/20 px-5 py-2 rounded-full hover:bg-white hover:text-black transition">
            View All
          </button>
        </div>

        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
          {[
            {
              name: 'FF Hoodie',
              price: '$89',
              image:
                'https://images.unsplash.com/photo-1503342217505-b0a15ec3261c?q=80&w=1974&auto=format&fit=crop',
            },
            {
              name: 'Baggy Pants',
              price: '$75',
              image:
                'https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?q=80&w=1974&auto=format&fit=crop',
            },
            {
              name: 'Oversized Tee',
              price: '$55',
              image:
                'https://images.unsplash.com/photo-1521572267360-ee0c2909d518?q=80&w=1974&auto=format&fit=crop',
            },
          ].map((item, index) => (
            <div
              key={index}
              className="group bg-zinc-900 rounded-3xl overflow-hidden border border-white/10 hover:border-white/30 transition"
            >
              <div className="overflow-hidden">
                <img
                  src={item.image}
                  alt={item.name}
                  className="w-full h-[500px] object-cover group-hover:scale-110 transition duration-700"
                />
              </div>

              <div className="p-6">
                <div className="flex items-center justify-between">
                  <div>
                    <h3 className="text-2xl font-bold uppercase">
                      {item.name}
                    </h3>
                    <p className="text-gray-400 mt-1">Limited Drop</p>
                  </div>

                  <span className="text-xl font-bold">{item.price}</span>
                </div>

                <button className="mt-6 w-full bg-white text-black py-3 rounded-full font-bold uppercase hover:scale-[1.02] transition">
                  Buy Now
                </button>
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* LOOKBOOK */}
      <section id="lookbook" className="px-6 md:px-14 py-24 bg-zinc-950">
        <div className="text-center mb-16">
          <h2 className="text-5xl font-black uppercase mb-4">
            Fearless Lookbook
          </h2>
          <p className="text-gray-400 max-w-2xl mx-auto">
            Street luxury inspired by hood rich culture and oversized fashion.
          </p>
        </div>

        <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
          <img
            src="https://images.unsplash.com/photo-1496747611176-843222e1e57c?q=80&w=1973&auto=format&fit=crop"
            className="rounded-3xl h-[700px] object-cover w-full"
            alt="Lookbook"
          />

          <img
            src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1974&auto=format&fit=crop"
            className="rounded-3xl h-[700px] object-cover w-full"
            alt="Lookbook"
          />
        </div>
      </section>

      {/* NEWSLETTER */}
      <section
        id="contact"
        className="px-6 md:px-14 py-28 text-center relative"
      >
        <div className="absolute inset-0 bg-gradient-to-r from-zinc-900 via-black to-zinc-900 opacity-70" />

        <div className="relative z-10 max-w-3xl mx-auto">
          <p className="uppercase tracking-[0.3em] text-gray-400 mb-4 text-sm">
            Join The Family
          </p>

          <h2 className="text-5xl md:text-6xl font-black uppercase mb-6">
            Stay Updated
          </h2>

          <p className="text-gray-400 mb-10 text-lg">
            Enter your email for exclusive drops, updates, and early access.
          </p>

          <div className="flex flex-col md:flex-row gap-4 justify-center">
            <input
              type="email"
              placeholder="Enter your email"
              className="bg-zinc-900 border border-white/10 px-6 py-4 rounded-full w-full md:w-[450px] outline-none"
            />

            <button className="bg-white text-black px-8 py-4 rounded-full font-bold uppercase hover:scale-105 transition">
              Subscribe
            </button>
          </div>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="border-t border-white/10 py-10 px-6 md:px-14 flex flex-col md:flex-row justify-between gap-6 items-center">
        <div className="flex items-center gap-3">
          <img
            src="/logo.png"
            alt="Fearless Fit"
            className="w-10 h-10 object-contain"
          />
          <p className="uppercase tracking-[0.2em] text-sm text-gray-400">
            Fearless Fit © 2026
          </p>
        </div>

        <div className="flex gap-6 text-sm text-gray-400 uppercase tracking-wider">
          <a href="#">Instagram</a>
          <a href="#">TikTok</a>
          <a href="#">Shop</a>
        </div>
      </footer>
    </div>
  )
}
