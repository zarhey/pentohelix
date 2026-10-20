# pentohelix
### Open-Source Low-Poly Helical Filter Topology / Доступная лоу-поли гофро-спиральная топология фильтра

> **Полезная форма лоу-поли топологии, применимая для свёртывания площади цилиндров в меньший объём, с тенсегрити-эффектом и возможностью самоочистки через тангенциальный поток.**
> 
> *A useful low-poly topology designed for folding cylinder surface area into a smaller volume, featuring a tensegrity effect and self-cleaning via tangential helical flow.*

---

## 🌍 English Description

### Overview
**Pentohelix** is a fundamental geometric solution for high-speed fluids and gas filtration. It bridges the gap between pleated, pocket, and disc filters. Developed independently through spatial coordinate transformation (from Cartesian to cylindrical Polar), it provides a mathematically optimized pattern: **minimum polygons (facets) with maximum zigzag amplitude**.

### Core Engineering Principles
1. **Direct Helical Flow:** Engineered for high-volume flow rates with minimal dynamic resistance, such as immediately following centrifugal pumps. Fluid smoothly swirls along spiral wave channels, maximizing kinetic energy retention without significant hydraulic losses from abrupt flow redirections.
2. **Tensegrity Self-Support:** Vertices of adjacent spiral turns form spatial interlocking nodes. The structure autonomously resists radial loads without requiring heavy internal perforated cores or external grid mesh supports.
3. **Integrated Spacer-free Gap:** The twisted nature of the low-poly corrugation prevents planes from flattening against each other, maintaining open channels for fluid velocity and eliminating bio-fouling "dead zones".
4. **Gradient Cone Core:** Instead of a generic pipe, fluid moves along a rear cone fairing. As fluid volume filters outward, the channel cross-section shrinks, keeping velocity constant and equalizing surface wear.

### Physical Implementations
*   **Metal (Seamless Foil/Tube):** Formed via uniform plastic deformation of an aluminum blank, then perforated. 100% seamless seal without seams.
*   **Polymer Ribbon (Spunbond):** Spirally wound with pre-scoring/embossing. Fluid pressure acts as a "ship's leak-stopping patch," sealing the overlap under load.
*   **Textiles (Nylon/Canvas):** A pocket-style design with internal structural struts/lines (parachute-wing style). Flow inflates the pockets, tensioning the struts into a rigid 3D form.

---

## 🇷🇺 Описание на русском языке

### Суть разработки
**Pentohelix** — это гибридное геометрическое решение, объединяющее лучшие свойства гофрированных, карманных и пластинчатых систем фильтрации. Разработанный через переход из декартовых координат в полярные координаты цилиндра, этот паттерн обеспечивает идеальный баланс: **минимум полигонов (граней) при максимуме амплитуды зигзага**.

### Главные инженерные преимущества
1. **Прямоточный Helical-поток:** Спроектирован под большие потоки пропускания и с минимальным динамическим сопротивлением, например, как сразу после центробежных насосов. Вода плавно закручивается по спиральным винтовым канавкам, максимально сохраняя кинетическую энергию без больших гидропотерь на резкие развороты потока.

2. **Эффект Тенсегрити:** Скрученная гофра сама удерживает форму. Вершины смежных витков спирали упираются друг в друга в заданных точках, формируя самонесущую пространственную ферму, устойчивую к давлению без внутренних трубок-распорок.
3. **Отсутствие спайсеров (сепараторов):** Из-за закручивания грани никогда не смыкаются плоскость к плоскости, автоматически сохраняя зазор для бегущей воды и исключая зоны застоя грязи и бактерий.
4. **Градиентный конус-обтекатель:** Канал плавно сужается по ходу движения среды, сохраняя постоянную скорость потока по закону Бернулли и выравнивая статическое давление по всей высоте элемента.

### Три среды воплощения геометрии
*   **Металл (Алюминий):** Направленная деформация бесшовной трубы с последующей перфорацией иглами. Максимальная надежность.
*   **Полимерная лента (Спанбонд):** Непрерывная спиральная намотка с предукладкой (биговкой) внахлест. Эффект «судового пластыря» — давление среды само герметизирует стык, исключая узел сварки.
*   **Текстиль (Парусина/Нейлон):** Карманный фильтр с системой внутренних строп (парашютная схема). Поток раздувает карманы изнутри, а стропы натягивают парусину, фиксируя жесткую 3D-форму.
---

### ⚠️ Infrastructure Note / Важное примечание по корпусам фильтров

*   **EN:** Standard domestic Big Blue 20BB filter housings with a radial inlet **cannot** be used out-of-the-box, as they redirect flow and destroy the helical kinetic energy. Since right-handed tangential housings do not exist in the retail consumer market, you must use industrial stainless steel direct-flow housings (In-Line filter housing 20") or manufacture a custom 3D-printed housing head with a tangential clockwise inlet designed specifically to match the Pentohelix step.
*   **RU:** Стандартные бытовые колбы Big Blue 20BB с радиальным входом **не подходят** для прямого использования, так как они ломают направление потока и гасят кинетическую энергию вихря. Поскольку корпусов с правой тангенциальной закруткой в розничной продаже не существует, необходимо использовать промышленные прямоточные корпуса из нержавеющей стали (In-Line housing 20") либо изготовить кастомную «голову» фильтра методом 3D-печати, заложив в неё правый тангенциальный ввод потока по касательной, согласованный с шагом Pentohelix.

---

## 🛠️ Repository Content / Содержимое
*   `pentohelix.stl` — Core 3D surface mesh model of the optimized low-poly geometry. This file represents a single repeatable segment of the open helical surface (not a solid body). It serves as a geometric invariant for further thickening, sheet metal/fabric deformation, or toolpath generation. The model features a **strictly right-handed (clockwise) helical twist direction**. This direction is geometrically invariant and must align with the rotation of the preceding centrifugal pump impeller to ensure a smooth hydrodynamic transition.
 You can click on the file above to explore the surface in GitHub's interactive 3D viewer. / Базовая 3D-модель поверхности (mesh) оптимизированной лоу-поли геометрии. Данный файл представляет собой незамкнутый фрагмент поверхности как один повторяемый шаг спирали (не твердое тело). Служит геометрическим инвариантом для последующего придания толщины, формовки листовых металлов/тканей или проектирования оснастки. Модель имеет **строго правое (по часовой стрелке) направление закрутки спирали**. Это важный геометрический инвариант: направление винта должно совпадать с направлением вращения крыльчатки центробежного насоса, чтобы закрученный поток заходил в канавки гладко, без встречного удара и кавитации.
 Вы можете кликнуть на файл в списке выше, чтобы изучить топологию поверхности в интерактивном 3D-плеере прямо в браузере.

*   `/images/paper_prototype.jpg` — Structural paper origami model proving expandability / Фото бумажного макета, доказывающее чистую геометрию сгибов.

## 👥 Links & Acknowledgments / Ссылки и Благодарности
*   **Origami Inspiration / Источник вдохновения:** The structural paper prototype was made using the excellent crease pattern from the open DIY project [Pentagonal High-Tower Spring on Instructables](https://www.instructables.com/Pentagonal-High-Tower-Spring/) by user *sphere360*. / Бумажный макет структуры был собран на основе прекрасной схемы развертки из открытого проекта [Pentagonal High-Tower Spring на Instructables](https://www.instructables.com/Pentagonal-High-Tower-Spring/) автора *sphere360*.
*   **Russian Mirror / Российское зеркало проекта:** [GitFlic zarhey/pentohelix](https://gitflic.ru)
*   **Developer Profiles:** Follow `zarhey` on YouTube and X (Twitter) for live workshop tests and updates.

## ⚠️ Disclaimer & Limitations / Дисклеймер и упреждения (Важно!)

### RU: Предупреждение для мастеров
Данный проект описывает фундаментальную информационную праформу (геометрическую «корзу»). Попытка скопировать форму Pentohelix «в лоб», без понимания физики сред, механики материалов и сопромата, приведет к ошибкам (эффект «мраморного телефона Старика Хоттабыча»). Помните о следующих ограничениях:

1. **Границы прочности материала:** При формовке металла (например, алюминия) радиус скругления вершин и граней подбирается строго под толщину и пластичность конкретного сплава. Игнорирование этого правила приведет к растрескиванию и разрыву заготовки по линиям концентрации напряжений.
2. **Гидродинамическое давление:** Вариант текстильного фильтра (парусина/нейлон) на стропах работает ТОЛЬКО в условиях расчетного натяжения внутренним потоком. При ошибке в длине строп или резком гидроударе геометрия будет разрушена давлением.
3. **Не готовый продукт:** Файл `pentohelix.stl` — это незамкнутый фрагмент поверхности (инвариант), а не готовая твердотельная модель для мгновенной 3D-печати. Оснастку, утолщение стенок и допуски вы рассчитываете самостоятельно под ваши задачи и материалы.

---

### EN: Engineering Disclaimer
This repository provides a fundamental geometric invariant (open surface mesh). Naive replication without careful calculations of structural mechanics and fluid dynamics will result in failure. Note the following design constraints:
1. **Material Fatigue:** Sharp low-poly vertices create high stress concentration. When forming sheet metal, ensure the bending radius complies with your specific material's elongation limits.
2. **Pressure Tolerances:** Textile canvas configurations rely entirely on perfect tension-to-flow balance. Incorrect strut length or sudden hydraulic shock waves will warp or destroy the profile.


## 📜 License / Лицензия
This hardware design is open-source and distributed under the **CERN Open Hardware Licence (CERN-OHL-W-2.0+)** and **GPL v3.0**. You are free to manufacture, modify, and improve this geometry, provided you maintain attribution and keep all derivative works open-source.

*Данная геометрия является открытой. Вы можете свободно производить и улучшать её, при условии сохранения авторства и обязательной публикации ваших модификаций под этой же открытой лицензией.*
