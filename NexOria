import React from "react";
import { Play, Tv, Radio, Film, Star } from "lucide-react";
import { motion } from "framer-motion";

export default function NexoriaHome() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-black via-zinc-900 to-black text-white font-sans relative">
      {/* Background glow */}
      <div className="absolute inset-0 bg-[radial-gradient(circle_at_top,rgba(59,130,246,0.15),transparent_60%)]" />

      {/* Header */}
      <header className="relative z-10 flex items-center justify-between px-10 py-6">
        <h1 className="text-3xl font-extrabold tracking-[0.3em]">NEXORIA</h1>
        <div className="px-6 py-3 rounded-2xl bg-green-500/90 text-black font-semibold shadow-xl">
          Accès gratuit (Bêta)
        </div>
      </header>

      {/* Hero */}
      <section className="relative z-10 px-10 py-24 grid lg:grid-cols-2 gap-16 items-center">
        <motion.div initial={{ opacity: 0, y: 40 }} animate={{ opacity: 1, y: 0 }}>
          <h2 className="text-6xl font-extrabold leading-tight">
            L’univers du streaming<br /> nouvelle génération
          </h2>
          <p className="text-gray-300 mt-8 max-w-xl text-lg">
            Films, télévision en direct et radios internationales accessibles
            <span className="text-green-400 font-semibold"> gratuitement </span>
            pendant la phase bêta. Profitez maintenant, l’abonnement viendra plus tard.
          </p>
          <div className="flex gap-5 mt-10">
            <button className="flex items-center gap-3 px-8 py-4 rounded-2xl bg-green-600 hover:bg-green-500 transition shadow-2xl">
              <Play size={20} /> Regarder maintenant (Gratuit)
            </button>
            <button className="px-8 py-4 rounded-2xl border border-gray-600 hover:bg-white/5 transition">
              Découvrir la plateforme
            </button>
          </div>
        </motion.div>

        {/* Hero visual */}
        <motion.div
          initial={{ opacity: 0, scale: 0.9 }}
          animate={{ opacity: 1, scale: 1 }}
          className="relative h-[420px] rounded-[2.5rem] overflow-hidden shadow-2xl bg-gradient-to-br from-blue-600/40 to-purple-700/30 flex items-end p-6"
        >
          <div>
            <p className="text-sm text-gray-200">Exclusive Premiere</p>
            <h3 className="text-2xl font-bold">NEXORIA Originals</h3>
          </div>
        </motion.div>
      </section>

      {/* Featured films */}
      <section className="relative z-10 px-10 py-20">
        <h3 className="text-3xl font-bold mb-10">Films à la une</h3>
        <div className="grid sm:grid-cols-2 lg:grid-cols-4 gap-8">
          {[
            { title: "Action", gradient: "from-red-600/40 to-black" },
            { title: "Drame", gradient: "from-purple-600/40 to-black" },
            { title: "Science‑Fiction", gradient: "from-blue-600/40 to-black" },
            { title: "Thriller", gradient: "from-emerald-600/40 to-black" },
          ].map((film, i) => (
            <motion.div
              key={i}
              whileHover={{ scale: 1.05 }}
              className="rounded-3xl overflow-hidden shadow-xl"
            >
              <div className={`h-64 bg-gradient-to-br ${film.gradient} flex items-end p-6`}>
                <span className="text-xl font-bold tracking-wide">{film.title}</span>
              </div>
              <div className="p-5">
                <div className="flex items-center gap-1 text-yellow-400">
                  <Star size={14} /> <span className="text-sm">4.8</span>
                </div>
              </div>
            </motion.div>
          ))}
        </div>
      </section>

      {/* Services */}
      <section className="relative z-10 px-10 py-20 grid md:grid-cols-3 gap-10">
        <Feature icon={<Tv />} title="TV Live" text="Chaînes HD avec zapping instantané." />
        <Feature icon={<Film />} title="Cinéma Premium" text="Catalogue élégant et exclusif." />
        <Feature icon={<Radio />} title="Radios" text="Écoutez partout, sans interruption." />
      </section>

      {/* Footer */}
      <footer className="relative z-10 px-10 py-12 text-gray-400 border-t border-white/10">
        © 2026 NEXORIA — Streaming Luxury Experience
      </footer>
    </div>
  );
}

function Feature({ icon, title, text }) {
  return (
    <motion.div
      whileHover={{ y: -8 }}
      className="p-10 rounded-[2.5rem] bg-gradient-to-br from-zinc-900 to-zinc-800 shadow-2xl"
    >
      <div className="w-14 h-14 flex items-center justify-center rounded-2xl bg-blue-600 mb-6">
        {icon}
      </div>
      <h3 className="text-2xl font-semibold mb-3">{title}</h3>
      <p className="text-gray-300">{text}</p>
    </motion.div>
  );
}
