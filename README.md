export default function CheburekLauncher() { const news = [ 'Обновление 1.0 — добавлены летающие чебуреки', 'Новый район: Завистливые кварталы', 'Онлайн гонки на фудтраках уже доступны', ];

return ( <div className="min-h-screen bg-black text-white p-6"> <div className="max-w-6xl mx-auto"> <div className="bg-zinc-900 rounded-3xl shadow-2xl overflow-hidden border border-orange-500"> <div className="relative h-72 bg-gradient-to-r from-orange-600 via-red-500 to-yellow-500 flex items-center justify-center"> <div className="absolute inset-0 opacity-20 bg-[radial-gradient(circle_at_center,white,transparent)]" />

<div className="text-center z-10">
          <h1 className="text-6xl font-black tracking-widest drop-shadow-2xl">
            ЧЕБУРЕК-СИТИ
          </h1>

          <p className="mt-4 text-xl text-orange-100">
            Открытый мир • Люди-Чебуреки • Хаос • Мемы
          </p>

          <button className="mt-8 px-10 py-4 text-2xl font-bold rounded-2xl bg-black hover:scale-105 transition-transform border-2 border-white">
            ИГРАТЬ
          </button>
        </div>
      </div>

      <div className="grid grid-cols-1 md:grid-cols-3 gap-6 p-6 bg-zinc-950">
        <div className="md:col-span-2 bg-zinc-900 rounded-2xl p-5 border border-zinc-700">
          <h2 className="text-2xl font-bold mb-4 text-orange-400">
            Новости
          </h2>

          <div className="space-y-4">
            {news.map((item, index) => (
              <div
                key={index}
                className="p-4 rounded-xl bg-zinc-800 hover:bg-zinc-700 transition"
              >
                {item}
              </div>
            ))}
          </div>
        </div>

        <div className="bg-zinc-900 rounded-2xl p-5 border border-zinc-700">
          <h2 className="text-2xl font-bold mb-4 text-yellow-400">
            Профиль
          </h2>

          <div className="space-y-3 text-zinc-300">
            <div>Имя: Главный Чебурек</div>
            <div>Уровень хрустящести: 99</div>
            <div>Фудтраков: 12</div>
            <div>Ресторанов: 5</div>
          </div>

          <button className="w-full mt-6 py-3 rounded-xl bg-orange-500 hover:bg-orange-400 text-black font-bold transition">
            МАГАЗИН
          </button>
        </div>
      </div>

      <div className="grid grid-cols-2 md:grid-cols-4 gap-4 p-6 bg-black border-t border-zinc-800">
        {['Настройки', 'Моды', 'Друзья', 'Выход'].map((item) => (
          <button
            key={item}
            className="py-4 rounded-2xl bg-zinc-900 hover:bg-orange-500 hover:text-black transition font-bold border border-zinc-700"
          >
            {item}
          </button>
        ))}
      </div>
    </div>
  </div>
</div>

); }
