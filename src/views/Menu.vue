<script>
export default {
  data() {
    return {
      activeCategory: 'все',
      filters: [
        {
          name: "Классические напитки",
          link: "classic"
        },
        {
          name: "Авторские напитки",
          link: "authors"
        },
        {
          name: "Холодные напитки",
          link: "cold"
        },
        {
          name: "Чаи",
          link: "teas"
        },
        {
          name: "Лимонады",
          link: "lemonades"
        },
        {
          name: "Фреши",
          link: "freshes"
        },
        {
          name: "Еда",
          link: "eats"
        },
      ],
      eatsCategories: [
        {
          name: "Завтраки"
        },
        {
          name: "Горячие блюда"
        },
        {
          name: "Салаты"
        },
        {
          name: "Сендвичи"
        },
        {
          name: "Десерты"
        },
        {
          name: "Выпечка"
        }
      ],
      eats: [
        {
          id: 1,
          name: 'Авокадо-тост с яйцом пашот',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '650'
        },
        {
          id: 2,
          name: 'Банановые оладьи',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '410'
        },
        {
          id: 3,
          name: 'Блинчики с индейкой и сыром',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '330'
        },
        {
          id: 4,
          name: 'Блинчики с творогом',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '320'
        },
        {
          id: 5,
          name: 'Вафли с цеплёнком',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '320'
        },
        {
          id: 6,
          name: 'Вафли с лососем и крем-чизом',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '420'
        },
        {
          id: 7,
          name: 'Гречневая каша с запеченными шампиньонами',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '290'
        },
        {
          id: 8,
          name: 'Овсяная каша с яблоками и корицей',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '310'
        },
        {
          id: 9,
          name: 'Оладьи из цукини с лососем',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '730'
        },
        {
          id: 10,
          name: 'Сырники с домашним вареньем и сметаной',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '470'
        },
        {
          id: 11,
          name: 'Запеканка с тыквой с яблоком',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '250'
        },
        {
          id: 12,
          name: 'Шакшука',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '420'
        },
        {
          id: 13,
          name: 'Бефстроганов с пюре',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '480'
        },
        {
          id: 14,
          name: 'Говяжьи котлеты с птитимом',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '450'
        },
        {
          id: 15,
          name: 'Котлеты куриные с булгуром',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '420'
        },
        {
          id: 16,
          name: 'Говядина с пюре из батата',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '630'
        },
        {
          id: 17,
          name: 'Жаркое с копченой говядиной',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '520'
        },
        {
          id: 18,
          name: 'Куриное филе с рисом и овощами',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '420'
        },
        {
          id: 19,
          name: 'Лазанья',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '650'
        },
        {
          id: 20,
          name: 'Паста с орзо и цеплёнком',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '590'
        },
        {
          id: 21,
          name: 'Фетучини с курицей и грибами',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '420'
        },
        {
          id: 22,
          name: 'Фетучини с креветками',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '480'
        },
        {
          id: 23,
          name: 'Боул с цеплёнком',
          category: 'Еда',
          subcategory: "Салаты",
          price: '450'
        },
        {
          id: 24,
          name: 'Боул с запеченым лососем',
          category: 'Еда',
          subcategory: "Салаты",
          price: '510'
        },
        {
          id: 25,
          name: 'Жаренные баклажаны',
          category: 'Еда',
          subcategory: "Салаты",
          price: '390'
        },
        {
          id: 26,
          name: 'Зеленый салат с ореховым соусом',
          category: 'Еда',
          subcategory: "Салаты",
          price: '450'
        },
        {
          id: 27,
          name: 'Цезарь с курицей',
          category: 'Еда',
          subcategory: "Салаты",
          price: '440'
        },
        {
          id: 28,
          name: 'Цезарь с креветками',
          category: 'Еда',
          subcategory: "Салаты",
          price: '470'
        },
        {
          id: 39,
          name: 'Бейгл с индейкой',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '320'
        },
        {
          id: 30,
          name: 'Грильчиз с говядиной',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '390'
        },
        {
          id: 31,
          name: 'Сендвич с индейкой и сыром',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '290'
        },
        {
          id: 32,
          name: 'Сендвич с копченым тунцом и яйцом',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '420'
        },
        {
          id: 33,
          name: 'Сендвич с куриным рулетом',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '270'
        },
        {
          id: 34,
          name: 'Сендвич с лососем',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '420'
        },
        {
          id: 35,
          name: 'Чизкейк классический',
          category: 'Еда',
          subcategory: "Десерты",
          price: '290'
        },
        {
          id: 36,
          name: 'Тартолетка малиновая',
          category: 'Еда',
          subcategory: "Десерты",
          price: '310'
        },
        {
          id: 37,
          name: 'Тарталетка карамельно-ореховая',
          category: 'Еда',
          subcategory: "Десерты",
          price: '320'
        },
        {
          id: 38,
          name: 'Медовик',
          category: 'Еда',
          subcategory: "Десерты",
          price: '250'
        },
        {
          id: 39,
          name: 'Пирожное "Картошка"',
          category: 'Еда',
          subcategory: "Десерты",
          price: '150'
        },
        {
          id: 40,
          name: 'Тирамису',
          category: 'Еда',
          subcategory: "Десерты",
          price: '390'
        },
        {
          id: 41,
          name: 'Трайфл "Сникерс"',
          category: 'Еда',
          subcategory: "Десерты",
          price: '270'
        },
        {
          id: 42,
          name: 'Трайфл черничный',
          category: 'Еда',
          subcategory: "Десерты",
          price: '280'
        },
        {
          id: 43,
          name: 'Трайфл финиковый',
          category: 'Еда',
          subcategory: "Десерты",
          price: '300'
        },
        {
          id: 44,
          name: 'Круассан с куриной грудкой и соусом барбекю',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '360'
        },
        {
          id: 45,
          name: 'Круассан с лососем и мягким сыром',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '380'
        },
        {
          id: 46,
          name: 'Круассан миндальный',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '285'
        },
        {
          id: 47,
          name: 'Круассан фисташковый',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '285'
        },
        {
          id: 48,
          name: 'Круассан с шоколадом',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '285'
        },
        {
          id: 49,
          name: 'Слойка с корицей и кремом маскарпоне',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '230'
        },
        {
          id: 50,
          name: 'Слойка с персиком',
          category: 'Еда',
          subcategory: "Выпечка",
          price: '200'
        }
      ],
      drinks: [
        {
          id: 1,
          name: 'Эспрессо',
          description: 'Крепкий кофе, приготовленный под высоким давлением. Имеет насыщенный вкус и характерную золотистую пенку',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/espresso.png',
          sizes: [
            { name: 'Стандартный', volume: '60 мл', price: 220 }
          ],
          isRecommended: true,
        },
        {
          id: 2,
          name: 'Американо',
          description: 'Эспрессо, разбавленный горячей водой. Обладает насыщенным вкусом, но более легкой текстурой, чем чистый эспрессо. Идеален для большой чашки.',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/americano.jpg',
          sizes: [
            { name: 'Стандартный', volume: '200 мл', price: 220 }
          ],
          isRecommended: false,
        },
        {
          id: 3,
          name: 'Капучино',
          description: 'Идеальный баланс эспрессо, молока и воздушной молочной пены. Классика, где кофе и нежность молока звучат в унисон.',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/capusino.jpg',
          sizes: [
            { name: 'Средний', volume: '200 мл', price: 250 },
            { name: 'Большой', volume: '300 мл', price: 270 }
          ],
          isRecommended: true,
        },
        {
          id: 4,
          name: 'Латте',
          description: 'Нежный и сливочный напиток на основе эспрессо с большим количеством молока и тонкой пенкой. Мягкий кофейный вкус для неторопливого наслаждения.',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/latte.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 280 },
            { name: 'Большой', volume: '400 мл', price: 320 }
          ],
          isRecommended: true,
        },
        {
          id: 5,
          name: 'Флет уайт',
          description: 'Австралийская классика. Готовится на двойном эспрессо с молоком, взбитым в плотную, но не воздушную пену, создающую гладкую пенку.',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/flet.jpg',
          sizes: [
            { name: 'Стандартный', volume: '200 мл', price: 250 }
          ],
          isRecommended: false,
        },
        {
          id: 6,
          name: 'Раф',
          description: 'Приготовлен на основе эспрессо, сливок и ванильного сахара, взбитых вместе. Невероятно нежный, кремовый и сладковатый',
          category: 'Классические напитки',
          imageUrl: '../src/images/drinks/raf.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 320 }
          ],
          isRecommended: true,
        },

        {
          id: 7,
          name: 'Шепот зеркал',
          description: 'Двойной шот эспрессо, влитый в тоник с маракуйей и щепоткой розовой гималайской соли. Невероятно чистый, освежающий вкус с игристым послевкусием и лёгкой солёной пенкой.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a1.png',
          sizes: [
            { name: 'Средний', volume: '250 мл', price: 280 },
            { name: 'Большой', volume: '350 мл', price: 330 }
          ],
          isRecommended: true,
        },
        {
          id: 8,
          name: 'Серое небо',
          description: 'Латте с добавлением натурального пищевого угля, кокосового молока и финикового сиропа.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a2.png',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 380 }
          ],
          isRecommended: true,
        },
        {
          id: 9,
          name: 'Восточный ветер',
          description: 'Традиционный раф, приготовленный на основе ванильно-имбирного сиропа, сливок и апельсиновой цедры, взбитый до состояния облака.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a3.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 320 },
            { name: 'Большой', volume: '400 мл', price: 370 }
          ],
          isRecommended: false,
        },
        {
          id: 10,
          name: 'Хвойный шепот',
          description: 'Капучино с фирменным сиропом из облепихи, можжевельника и кленового сиропа. Украшается веточкой розмарина.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a4.png',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 340 }
          ],
          isRecommended: true,
        },
        {
          id: 11,
          name: 'Дымный переулок',
          description: 'Холодный американо, настоянный на копчёных палочках ванили и щепотке молотого чёрного перца, с добавлением тоника.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a5.png',
          sizes: [
            { name: 'Стандартный', volume: '350 мл', price: 300 }
          ],
          isRecommended: false,
        },
        {
          id: 12,
          name: 'Вечерний фольклор',
          description: 'Крепкий фильтр-кофе со взбитыми сливками и сиропом, имитирующим вкус виски (с дымными, солодовыми и ванильными нотами).',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a6.png',
          sizes: [
            { name: 'Стандартный', volume: '250 мл', price: 360 }
          ],
          isRecommended: false,
        },
        {
          id: 13,
          name: 'Темный мед',
          description: 'Густой горячий шоколад на миндальном молоке с добавлением сиропа из жареного фундука, щепотки чили и апельсинового масла.',
          category: 'Авторские напитки',
          imageUrl: '../src/images/drinks/a6.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 370 },
            { name: 'Большой', volume: '400 мл', price: 420 }
          ],
          isRecommended: true,
        },

        {
          id: 14,
          name: 'Айс латте',
          description: 'Прохладная классика. Двойной эспрессо, лед и молоко, создающие освежающий и сбалансированный кофейный коктейль. ',
          category: 'Холодные напитки',
          imageUrl: '../src/images/drinks/x2.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 280 },
            { name: 'Большой', volume: '400 мл', price: 320 }
          ],
          isRecommended: true,
        },
        {
          id: 15,
          name: 'Колд Брю',
          description: 'Наш кофе, приготовленный методом холодного заваривания. Отличается мягким, сбалансированным вкусом без горечи и высокой крепостью. Подается со льдом.',
          category: 'Холодные напитки',
          imageUrl: '../src/images/drinks/x4.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 240 }
          ],
          isRecommended: false,
        },
        {
          id: 16,
          name: 'Эспрессо-тоник',
          description: 'Охлаждённый тоник, двойной эспрессо и лёд. Освежающая горчинка тоника и цитрусовые ноты идеально оттеняют кофе, создавая яркий игристый вкус.',
          category: 'Холодные напитки',
          imageUrl: '../src/images/drinks/x3.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 290 }
          ],
          isRecommended: false,
        },
        {
          id: 17,
          name: 'Фильтр "Станция мир"',
          description: 'фильтр, сироп из горных трав, клюква, сливочно-сырный крем сироп собственного приготовления',
          category: 'Холодные напитки',
          imageUrl: '../src/images/drinks/x1.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 280 }
          ],
          isRecommended: true,
        },

        {
          id: 18,
          name: 'Манго - Цитрус',
          description: 'Освежающий микс тропической сладости спелого манго с яркой кислинкой лимона и лайма. Согревающий и бодрящий.',
          category: 'Чаи',
          imageUrl: '../src/images/drinks/tea1.png',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 280 }
          ],
          isRecommended: true,
        },
        {
          id: 19,
          name: 'Каркаде - Гранат',
          description: 'Горячий яркий тандем: насыщенная кислинка гибискуса с глубокой сладостью граната. Бодрящий и согревающий напиток с рубиновым цветом.',
          category: 'Чаи',
          imageUrl: '../src/images/drinks/tea2.png',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 280 }
          ],
          isRecommended: false,
        },
        {
          id: 20,
          name: 'Облепиха - Клюква',
          description: 'Согревающий витаминный взрыв: яркая кислинка облепихи и терпкая ягода клюквы в горячем гармоничном дуэте.',
          category: 'Чаи',
          imageUrl: '../src/images/drinks/tea3.png',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 280 }
          ],
          isRecommended: false,
        },
        {
          id: 21,
          name: 'Имбирь - Лимон - Мед',
          description: 'Горячий огненный эликсир: острая свежесть имбиря, яркость лимона и мягкая сладость мёда. Идеальная защита от холода и хандры.',
          category: 'Чаи',
          imageUrl: '../src/images/drinks/tea4.png',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 280 }
          ],
          isRecommended: false,
        },

        {
          id: 22,
          name: 'Малина - Маракуйя',
          description: 'Освежающий микс сочной ягодной сладости и яркой тропической кислотности. Идеальный баланс вкусов в прохладном напитке.',
          category: 'Лимонады',
          imageUrl: '../src/images/drinks/l1.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 310 },
            { name: 'Большой', volume: '400 мл', price: 380 }
          ],
          isRecommended: true,
        },
        {
          id: 23,
          name: 'Гранат - Клюква',
          description: 'Сбалансированный дуэт насыщенной сладости граната и яркой кислинки клюквы. Прохладный, тонизирующий и не приторный напиток.',
          category: 'Лимонады',
          imageUrl: '../src/images/drinks/l2.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 310 },
            { name: 'Большой', volume: '400 мл', price: 380 }
          ],
          isRecommended: false,
        },
        {
          id: 24,
          name: 'Ягодный',
          description: 'Классическое сочетание спелой клубники, сладкой малины и лёгкой терпкости смородины. Освежающий и гармоничный вкус лета.',
          category: 'Лимонады',
          imageUrl: '../src/images/drinks/l4.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 310 },
            { name: 'Большой', volume: '400 мл', price: 380 }
          ],
          isRecommended: false,
        },
        {
          id: 25,
          name: 'Персик - Каламанси',
          description: 'Освежающее сочетание нежной сладости персика и цитрусовой свежести каламанси. Газированный, лёгкий и сбалансированный напиток.',
          category: 'Лимонады',
          imageUrl: '../src/images/drinks/l3.jpg',
          sizes: [
            { name: 'Средний', volume: '300 мл', price: 310 },
            { name: 'Большой', volume: '400 мл', price: 380 }
          ],
          isRecommended: true,
        },

        {
          id: 3,
          name: 'Апельсин',
          description: 'Свежевыжатый апельсиновый сок',
          category: 'Фреши',
          imageUrl: '../src/images/drinks/f1.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 390 }
          ],
          isRecommended: true,
        },
        {
          id: 26,
          name: 'Яблоко',
          description: 'Свежевыжатый яблочный сок',
          category: 'Фреши',
          imageUrl: '../src/images/drinks/f4.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 320 }
          ],
          isRecommended: true,
        },
        {
          id: 27,
          name: 'Морковь',
          description: 'Свежевыжатый морковный сок с яблоком',
          category: 'Фреши',
          imageUrl: '../src/images/drinks/f6.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 290 }
          ],
          isRecommended: false,
        },
        {
          id: 28,
          name: 'Грейпфрут',
          description: 'Свежевыжатый грейпфрутовый сок',
          category: 'Фреши',
          imageUrl: '../src/images/drinks/f2.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 420 }
          ],
          isRecommended: false,
        },
        {
          id: 29,
          name: 'Гранат',
          description: 'Свежевыжатый гранатовый сок',
          category: 'Фреши',
          imageUrl: '../src/images/drinks/f3.jpg',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 370 }
          ],
          isRecommended: true,
        }
      ]
    }
  },
  methods: {
    scrollToSection(id, name) {
      this.activeCategory = name
      const element = document.getElementById(id);
      if (element) {
        element.scrollIntoView({behavior: 'smooth'});
      }
    },
    leftColumnFilters() {
      return this.eatsCategories.slice(0, Math.ceil(this.eatsCategories.length / 2));
    },
    rightColumnFilters() {
      return this.eatsCategories.slice(Math.ceil(this.eatsCategories.length / 2));
    }
  }
}
</script>

<template>
  <div class="flex flex-column h-screen w-full gap-4 align-items-center">
    <div class="flex flex-column w-9 gap-5 h-full">
      <div class="text-7xl font-normal text-gray-900">
        Меню
      </div>

      <div class="sticky top-0 z-5 bg-transparent py-3">
        <div class="flex w-full">
          <div v-for="filter in filters"
               class="border-none h-fit mx-1 px-3 py-2 border-round-2xl cursor-pointer text-white no-underline text-xl"
               @click="this.scrollToSection(filter.link, filter.name)"
               :class="activeCategory === `${filter.name}`?'btn-bg-color':'bg-gray-900'">
            {{ filter.name }}
          </div>
        </div>
      </div>

      <div class="flex-grow-1 overflow-y-auto" style="scrollbar-width: none; -ms-overflow-style: none;">
        <div v-for="filter in filters"
             :id="filter.link"
             class="text-8xl font-medium text-gray-900 text-center mb-6">
          {{ filter.name }}

          <div v-if="filter.name !== 'Еда'" v-for="drink in drinks" :key="drink.id">
            <div v-if="drink.category === filter.name" class="flex w-full h-full gap-4 border-round-3xl card-bg-color p-4 mb-2">
              <div class="w-15rem h-15rem border-round-3xl overflow-hidden">
                <img :src="drink.imageUrl"
                     :alt="drink.name"
                     class="w-full h-full object-cover"/>
              </div>

              <div class="flex-1 flex flex-column gap-3">
                <div class="flex justify-content-between align-items-start">
                  <div>
                    <p class="text-2xl font-bold mb-1 text-gray-900">{{ drink.name }}</p>
                  </div>
                  <div class="flex gap-2">
                    <span v-if="drink.isRecommended"
                          class="inline-block px-3 py-1 text-sm border-round-3xl bg-yellow-100 text-yellow-700">
                      Рекомендуем
                    </span>
                  </div>
                </div>

                <p class="text-xl text-left text-gray-700 leading-relaxed">{{ drink.description }}</p>

                <div>
                  <h4 class="text-xl text-left font-semibold mb-2 text-gray-900">Размеры и цены:</h4>
                  <div class="flex flex-wrap gap-3">
                    <div v-for="size in drink.sizes"
                         :key="size.name"
                         class="border-1 border-gray-200 border-round-3xl p-3 bg-white">
                      <div class="text-lg font-medium text-gray-900">{{ size.name }}</div>
                      <div class="text-sm text-gray-600 mb-1">
                        {{ size.volume || size.weight }}
                      </div>
                      <div class="text-lg font-bold text-blue-600">{{ size.price }} ₽</div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div v-else class="flex w-full h-full border-round-3xl card-bg-color p-4">
            <div class="flex flex-row flex-wrap w-full">
              <div v-for="cat in leftColumnFilters()" :key="cat.name" class="w-full text-4xl font-semibold label_text_color p-2 mb-1"
                   style="width: 50%; max-width: 50%">
                {{cat.name}}
                <div v-for="eat in eats" class="flex w-full">
                  <div v-if="eat.subcategory === cat.name" class="flex justify-content-around w-full px-4">
                    <p class="text-gray-900 font-normal text-2xl">{{eat.name}}</p>
                    <p class="text-gray-900 font-normal text-2xl ml-auto">{{eat.price}}</p>
                  </div>
                </div>
              </div>

              <div v-for="cat in rightColumnFilters()" :key="cat.name" class="w-full text-4xl font-semibold label_text_color p-2 mb-1"
                   style="width: 50%; max-width: 50%">
                {{cat.name}}
                <div v-for="eat in eats" class="flex w-full">
                  <div v-if="eat.subcategory === cat.name" class="flex w-full px-4">
                    <p class="text-gray-900 font-normal text-2xl">{{eat.name}}</p>
                    <p class="text-gray-900 font-normal text-2xl ml-auto">{{eat.price}}</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.footer-bg-color {
  background-color: #122343;
}

.card-bg-color {
  background-color: #ffffff !important;
}

.label_text_color {
  color: #ac3b61;
}

.btn-bg-color {
  background: #ac3b61;
}
</style>