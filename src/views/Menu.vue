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
          name: "Боулы"
        }
      ],
      eats: [
        {
          id: 1,
          name: 'Сырники с ягодами',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '690'
        },
        {
          id: 2,
          name: 'Зеленый салат',
          category: 'Еда',
          subcategory: "Салаты",
          price: '740'
        },
        {
          id: 3,
          name: 'Боул с курицей',
          category: 'Еда',
          subcategory: "Боулы",
          price: '760'
        },
        {
          id: 4,
          name: 'Фетучини с курицей',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '690'
        },
        {
          id: 5,
          name: 'Сендвич с курицей',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '450'
        },
        {
          id: 6,
          name: 'Чизкейк',
          category: 'Еда',
          subcategory: "Десерты",
          price: '260'
        },
        {
          id: 7,
          name: 'Творожная запеканка',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '650'
        },
        {
          id: 8,
          name: 'Омлет с ветчиной',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '580'
        },
        {
          id: 9,
          name: 'Греческий салат',
          category: 'Еда',
          subcategory: "Салаты",
          price: '720'
        },
        {
          id: 10,
          name: 'Салат Цезарь',
          category: 'Еда',
          subcategory: "Салаты",
          price: '780'
        },
        {
          id: 11,
          name: 'Боул с лососем',
          category: 'Еда',
          subcategory: "Боулы",
          price: '850'
        },
        {
          id: 12,
          name: 'Боул вегетарианский',
          category: 'Еда',
          subcategory: "Боулы",
          price: '680'
        },
        {
          id: 13,
          name: 'Паста Карбонара',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '720'
        },
        {
          id: 14,
          name: 'Куриные крылышки',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '690'
        },
        {
          id: 15,
          name: 'Сендвич с ветчиной',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '420'
        },
        {
          id: 16,
          name: 'Сендвич вегетарианский',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '380'
        },
        {
          id: 17,
          name: 'Тирамису',
          category: 'Еда',
          subcategory: "Десерты",
          price: '320'
        },
        {
          id: 18,
          name: 'Маффин шоколадный',
          category: 'Еда',
          subcategory: "Десерты",
          price: '240'
        },
        // Добавляем еще несколько позиций
        {
          id: 19,
          name: 'Сырники с медом',
          category: 'Еда',
          subcategory: "Завтраки",
          price: '670'
        },
        {
          id: 20,
          name: 'Салат с тунцом',
          category: 'Еда',
          subcategory: "Салаты",
          price: '710'
        },
        {
          id: 21,
          name: 'Боул с тофу',
          category: 'Еда',
          subcategory: "Боулы",
          price: '640'
        },
        {
          id: 22,
          name: 'Лазанья',
          category: 'Еда',
          subcategory: "Горячие блюда",
          price: '750'
        },
        {
          id: 23,
          name: 'Сендвич с сыром',
          category: 'Еда',
          subcategory: "Сендвичи",
          price: '400'
        },
        {
          id: 24,
          name: 'Брауни',
          category: 'Еда',
          subcategory: "Десерты",
          price: '280'
        }
      ],
      drinks: [
        // Классические напитки
        {
          id: 1,
          name: 'Латте "Осенний вечер"',
          description: 'Нежный латте с карамельным сиропом и пенкой из взбитых сливок, украшенный карамельным соусом',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Маленький', volume: '250 мл', price: 280 },
            { name: 'Средний', volume: '350 мл', price: 320 },
            { name: 'Большой', volume: '450 мл', price: 370 }
          ],
          isRecommended: true,
        },
        {
          id: 5,
          name: 'Капучино "Классический"',
          description: 'Идеальное сочетание эспрессо и молочной пенки с нежной текстурой',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Маленький', volume: '200 мл', price: 260 },
            { name: 'Средний', volume: '300 мл', price: 300 },
            { name: 'Большой', volume: '400 мл', price: 350 }
          ],
          isRecommended: true,
        },
        {
          id: 6,
          name: 'Американо "Бодрость"',
          description: 'Крепкий черный кофе для настоящих ценителей',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '200 мл', price: 220 },
            { name: 'Большой', volume: '300 мл', price: 270 }
          ],
          isRecommended: false,
        },
        {
          id: 7,
          name: 'Эспрессо "Итальянский"',
          description: 'Концентрированный кофе с насыщенным вкусом и ароматом',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Порция', volume: '30 мл', price: 180 }
          ],
          isRecommended: true,
        },
        {
          id: 14,
          name: 'Раф "Ванильный"',
          description: 'Кофейный напиток со сливками и ванильным сиропом',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 350 },
            { name: 'Большой', volume: '400 мл', price: 420 }
          ],
          isRecommended: true,
        },
        {
          id: 18,
          name: 'Мокачино',
          description: 'Кофе с шоколадом и молоком',
          category: 'Классические напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Маленький', volume: '250 мл', price: 300 },
            { name: 'Средний', volume: '350 мл', price: 350 },
            { name: 'Большой', volume: '450 мл', price: 400 }
          ],
          isRecommended: true,
        },

        // Авторские напитки
        {
          id: 19,
          name: 'Латте "Медовая груша"',
          description: 'Авторский латте с сиропом груши, медом и корицей',
          category: 'Авторские напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Средний', volume: '350 мл', price: 380 },
            { name: 'Большой', volume: '450 мл', price: 440 }
          ],
          isRecommended: true,
        },
        {
          id: 20,
          name: 'Капучино "Карамельный орех"',
          description: 'Авторский капучино с карамелью и фундуком',
          category: 'Авторские напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Средний', volume: '350 мл', price: 360 },
            { name: 'Большой', volume: '450 мл', price: 420 }
          ],
          isRecommended: true,
        },
        {
          id: 21,
          name: 'Раф "Кокосовый рай"',
          description: 'Авторский раф с кокосовым сиропом и стружкой кокоса',
          category: 'Авторские напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 390 },
            { name: 'Большой', volume: '400 мл', price: 460 }
          ],
          isRecommended: true,
        },
        {
          id: 22,
          name: 'Матча "Ягодный взрыв"',
          description: 'Авторский матча латте с ягодным сиропом',
          category: 'Авторские напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 400 },
            { name: 'Большой', volume: '400 мл', price: 470 }
          ],
          isRecommended: false,
        },

        // Холодные напитки
        {
          id: 12,
          name: 'Лимонад "Мятный"',
          description: 'Освежающий лимонад с мятой и лаймом',
          category: 'Холодные напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 320 },
            { name: 'Большой', volume: '600 мл', price: 420 }
          ],
          isRecommended: true,
        },
        {
          id: 13,
          name: 'Молочный коктейль "Шоколадный"',
          description: 'Нежный молочный коктейль с шоколадным сиропом',
          category: 'Холодные напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 380 },
            { name: 'Большой', volume: '600 мл', price: 480 }
          ],
          isRecommended: true,
        },
        {
          id: 17,
          name: 'Кола со льдом',
          description: 'Классическая кола со льдом',
          category: 'Холодные напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Банка', volume: '330 мл', price: 180 },
            { name: 'Стакан', volume: '500 мл', price: 220 }
          ],
          isRecommended: false,
        },
        {
          id: 23,
          name: 'Айс латте',
          description: 'Холодный латте со льдом',
          category: 'Холодные напитки',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Средний', volume: '400 мл', price: 340 },
            { name: 'Большой', volume: '500 мл', price: 410 }
          ],
          isRecommended: true,
        },

        // Чаи
        {
          id: 2,
          name: 'Матча латте',
          description: 'Традиционный японский чай матча, взбитый с молоком в нежный кремовый напиток',
          category: 'Чаи',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 350 },
            { name: 'Большой', volume: '400 мл', price: 420 }
          ],
          isRecommended: false,
        },
        {
          id: 8,
          name: 'Чай "Английский завтрак"',
          description: 'Классический черный чай с насыщенным вкусом',
          category: 'Чаи',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Чайник', volume: '500 мл', price: 320 },
            { name: 'Чашка', volume: '250 мл', price: 200 }
          ],
          isRecommended: false,
        },
        {
          id: 9,
          name: 'Зеленый чай "Жасмин"',
          description: 'Нежный зеленый чай с цветами жасмина',
          category: 'Чаи',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Чайник', volume: '500 мл', price: 350 },
            { name: 'Чашка', volume: '250 мл', price: 220 }
          ],
          isRecommended: true,
        },
        {
          id: 15,
          name: 'Чай "Фруктовый микс"',
          description: 'Ароматный фруктовый чай с ягодами',
          category: 'Чаи',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Чайник', volume: '500 мл', price: 380 },
            { name: 'Чашка', volume: '250 мл', price: 240 }
          ],
          isRecommended: false,
        },
        {
          id: 19,
          name: 'Чай "Ромашковый"',
          description: 'Успокаивающий травяной чай',
          category: 'Чаи',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Чайник', volume: '500 мл', price: 300 },
            { name: 'Чашка', volume: '250 мл', price: 180 }
          ],
          isRecommended: false,
        },

        // Лимонады
        {
          id: 24,
          name: 'Лимонад "Классический"',
          description: 'Освежающий лимонад с лимоном и мятой',
          category: 'Лимонады',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 300 },
            { name: 'Большой', volume: '600 мл', price: 400 }
          ],
          isRecommended: true,
        },
        {
          id: 25,
          name: 'Лимонад "Ягодный"',
          description: 'Лимонад с клубникой и малиной',
          category: 'Лимонады',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 340 },
            { name: 'Большой', volume: '600 мл', price: 440 }
          ],
          isRecommended: true,
        },
        {
          id: 26,
          name: 'Лимонад "Имбирный"',
          description: 'Пряный лимонад с имбирем и медом',
          category: 'Лимонады',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '400 мл', price: 320 },
            { name: 'Большой', volume: '600 мл', price: 420 }
          ],
          isRecommended: false,
        },

        // Фреши
        {
          id: 3,
          name: 'Фреш "Апельсиновый"',
          description: 'Свежевыжатый апельсиновый сок',
          category: 'Фреши',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 380 },
            { name: 'Большой', volume: '450 мл', price: 480 }
          ],
          isRecommended: true,
        },
        {
          id: 10,
          name: 'Фреш "Яблочный"',
          description: 'Свежевыжатый яблочный сок',
          category: 'Фреши',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 350 },
            { name: 'Большой', volume: '450 мл', price: 450 }
          ],
          isRecommended: false,
        },
        {
          id: 11,
          name: 'Фреш "Морковный"',
          description: 'Свежевыжатый морковный сок с яблоком',
          category: 'Фреши',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 320 },
            { name: 'Большой', volume: '450 мл', price: 420 }
          ],
          isRecommended: true,
        },
        {
          id: 16,
          name: 'Фреш "Ананасовый"',
          description: 'Свежевыжатый ананасовый сок',
          category: 'Фреши',
          imageUrl: 'https://i0.wp.com/www.m5zn.com/wp-content/uploads/2022/05/%D8%A7%D9%81%D8%B6%D9%84-%D9%85%D8%B4%D8%B1%D9%88%D8%A8-%D9%81%D9%8A-%D8%AA%D9%8A%D9%85-%D9%87%D9%88%D8%B1%D8%AA%D9%86%D8%B2.webp?ssl=1',
          sizes: [
            { name: 'Стандартный', volume: '300 мл', price: 420 },
            { name: 'Большой', volume: '450 мл', price: 520 }
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
      <div id="bonuses" class="text-7xl font-normal text-gray-900">
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

                <div class="flex gap-4 text-lg text-gray-600">
                  <div v-if="drink.allergens"
                       class="flex align-items-center gap-1">
                    <i class="pi pi-exclamation-circle"></i>
                    <span>Аллергены: {{ drink.allergens.join(', ') }}</span>
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