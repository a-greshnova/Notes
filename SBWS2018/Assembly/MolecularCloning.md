
# Молекулярное клонирование

### Высокопроизводительное клонирование
Позволяет осуществлять:
* комбинаторную сборку
* сборку многокомпонентных конструкций

Источник: [Высокопроизводительное клонирование](https://stepik.org/lesson/11339/step/1?unit=2449)

## Golden Gate

![Golden-Gate](https://github.com/a-greshnova/Notes/blob/master/GoldenGate.png)

В основе Golden Gate реакции рестирикции и лигирования, но используется рестриктаза типа IIs. Рестриктазы этого типа делают разрезы 
вне сайта узнавания. 
Рестриктаза BsaI, используемая в Golden Gate
* имеет сайт узнавания "GGTCTC" (не палиндромный и имеет направление);
* делает разрез на один нуклеотид ниже сайта узнавания.

Таким образом, рестриктазы могут создавать разные липкие концы в зависимости от того, в каком контексте находятся сайты узнавания 
рестриктазы. На 5' концы ПЦР праймеров для вставки добавляются адаптеры, содержащие сайт узнавания рестриктазы BsaI и последовательность, 
которая будет разрезана. Сайты узнавания расположены в такой ориентации (стрелки направлены "внутрь"), чтобы после обработки ферментами 
рестрикции сайты узнавания отрезались и остались только липкие концы. В векторе, в который будет производится вставка, сайты узнавания BsaI
расположены так (стрелки направлены "наружу"), чтобы при обработке ферментами рестрикции сайты узнавания рестриктазы и последовательность 
между ними была вырезана, и остались липкие концы. Т.к. мы сами добавляли ко вставке последовательность, которая будет разрезана, 
получившиеся липкие концы будут совместимыми с теми липкими концами, которыми мы захотим (возможно осуществить последовательную сборку нескольких фрагментов).

**Преимущества:**
* можно осуществить многокомпонентную сборку
* нет неоднозначности с направлением встраивания фрагмента

**Ограничения:**
* все липкие концы должны различаться между собой и не быть палиндромами

*Похожие способы:*
* MoClo
* Golden Braid

Источник:
* [The Golden Gate assembly method (and MoClo and GoldenBraid)](https://j5.jbei.org/j5manual/pages/23.html)
* [Рестриктазы IIS, GoldenGate и GoldenBraid клонирование](https://stepik.org/lesson/11342/step/1?unit=2452)

## Gibson

![Gibson](https://github.com/a-greshnova/Notes/blob/master/Gibson.png)

Реакция в одной пробирке при температуре 50°C. Вектор, в который будет производиться вставка, и сама вставка должны иметь перекрывающиеся области (можно добавить адаптеры на 5' к праймерам вставки). Вектор и вставка смешиваются вместе, добавляется 5' экзонуклеаза. При 50°C она очень нестабильная и до того как выйдет из строя успевает убрать около 25 нуклеотидов, создавая совместимые липкие концы на концах вектора и вставки. После липкие концы отжигаются друг на друга, бреши застраиваются термостабильной высокоточной полимеразой И затем сшиваются лигазой.

**Преимущества:**
* не оставляет шрамов
* не зависит от последовательности (не нужно добавлять сайты рестрикции)
* позволяет собрать сразу несколько фрагментов ДНК

**Ограничения:**
* получающиеся после обработки рестриктазами однонитевые фрагменты не должны образовывать шпилек

*Похожие способы:*
* SLIC
* CPEC
* SLiCE

Источник: 
* [Клонирование за счет создания однонитевых концов](https://stepik.org/lesson/11343/step/1?unit=2453)
* [The SLIC, Gibson, CPEC and SLiCE assembly methods (and GeneArt® Seamless, In-Fusion® Cloning)](https://j5.jbei.org/j5manual/pages/22.html#2)