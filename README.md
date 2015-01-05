# LESS timeline

Минималистичная адаптивная шкала времени с лёгкой настройкой внешнего вида через LESS-переменные.
Демонстрация работы на [codepen.io](http://codepen.io/nicothin/pen/azBagM?editors=110)

## Использование

1. Скопируйте HTML-разметку из `index.html`
2. Настройте внешний вид через LESS-переменные в `less\components\variables.less`
3. Скомпилируйте `less\style.less` (требуется [Autoprefixer](https://github.com/postcss/autoprefixer)) и подключите получившийся стилевой файл к своей разметке.

### Переменные

    @event_color:                #428bca;     // цвет линий и фонов блоков с «вывороткой»
    @event_padding:              1.5rem;     // внутренний отступ блока описания события
    @event_margin_bottom:        2rem;       // нижний отступ блока описания события
    
    @event_line_width:           .2rem;      // толщина линии времени (лучше делать чётным числом)
    @event_bullit_size:          round((@event_date_height * 0.4)); // размер буллита на линии времени
    @event_bullit_margin:        .4rem;      // отступ от буллита до линии времени
    
    @event_date_width:           13rem;      // ширина обычной даты
    @event_date_width--long:     17rem;      // ширина длинной даты
    @event_date_width--short:    10rem;      // ширина короткой даты

    @event_headers_family:       'PT Sans Narrow', sans-serif; // шрифт заголовка
    @event_headers_weight:       700;        // жирность заголовков
    @event_h1_size:              2em;        // размер названия события
    @event_h2_size:              1.5em;      // размер заголовка
    

## Кроссбраузерность

Поддерживаются Chrome, Firefox, Opera последних и предпоследних версий, Internet Explorer 10 и новее.
