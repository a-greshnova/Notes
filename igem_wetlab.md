# dCas9 -> GFP

## План работы

Задача | Время выполнения | Результат
-------|------------------|-----
Подготовка компетентных клеток E.coli | 12.06 - 15.06 | Готово
Наработка dCas9 **P6 11J** 2019| 15.06 - 20.06 | Проверка сиквенса - ?
ПЦР амплификация и добавление сайтов рестрикции и линкера к гену dCas9 | 1 день (? праймеры) | -
Наработка плазмиды GFP | 19.06 - 20.06 | Готово
Наработка плазмид с Addgene | 3.07.19 - ? | -
Сборка dCas9 и GFP | 2 дня | -
Отбор клонов | 1 день | - 
Экспрессия гибридного белка в E.coli | август | -
Проверка (антитела?..) | август | -

[Benchling](https://benchling.com/greshnova/f_/TeZKADfR-summer-practice-2019/?filter=section%3Ainventory%3Btypes%3AIS_ONE_OF%3Afolder%2Cbasic_folder_item%2Cprotein%2Csequence%2Coligo%3Bfolder%3Alib_TeZKADfR%3BarchivePurposes%3AIS_ONE_OF%3ANOT_ARCHIVED&offset=0&limit=100&sort=name&reverse=0&q=)

### dCas9

[BBa_K1150000](http://parts.igem.org/wiki/index.php?title=Part:BBa_K1150000)
Inconsistent

Можно охарактеризовать этот биобрик
[Check](https://www.genscript.com/tools/rare-codon-analysis) codon optomisation index (CAI) 

Добавим информацию о биобрике, в работе будем использовать плазмиду от Дмитрия.

### GFP

[pet28a GFP](https://benchling.com/greshnova/f/TeZKADfR-summer-practice-2019/seq-2hUdmAbT-pet28a_gfp-2/edit)

На addgene есть плазмида с гибридным белком [dCas9-GFP](https://www.addgene.org/64104/)

### Линкер

Можно взять из плазмиды на addgene: ggctctactagtggctctcccaagaagaagaggaaggtaggatccggaagt (GSTSGSPKKKRKVGSGS)
Коллекция линкеров на [igem](http://parts.igem.org/Protein_domains/Linker)

[Статья](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3726540/pdf/nihms-411484.pdf) про гибридные белки

Возможные варианты линкеров:
- (GGGGS)n (n=3 [canditest](http://2018.igem.org/Team:UiOslo_Norway/Design), igem 2018)
- (G)8
- GSAGSAAGSGEF
  - GFP -> protein
  - меньше аггрегации и неправильного сворачивания

### Праймеры для ПЦР dCas9

Forward: TCTAGAGACAAGAAGTACA

- добавляем сайт XbaI

Reverse: GAATTCACTTCCGGATCCTACCTTCCTCTTCTTCTTGGGAGAGCCACTAGTAGAGCCGTCGCCTCCCAGC

- добавляем линкер (GSAGSAAGSGEF или GSTSGSPKKKRKVGSGS)
- добавляем сайт EcoRI

### Подготовка ультракомпетентных клеток *E.coli*

The Inoue Method for Preparation and Transformation of Competent E. coli: Ultracompetent Cells

## Разнообразие систем CRISPR

[Презентация](https://github.com/a-greshnova/2019_igem/blob/master/Diversity%20and%20evolution%20of%20class%202%20CRISPR%E2%80%93Cas%20systems.pdf) по [обзору](https://www.nature.com/articles/nrmicro.2016.184)

### Трансформация ультракомпетентных клеток *E.coli*

- PET28a GFP (Kan) - 5 мкл + 100 мкл *E.coli*
- pSB1C3 dCas9 (Cm) - 3 мкл + 100 мкл *E.coli*

### Выделение плазмид

### Пороверка dCas9

**ПЦР dCas9**

**Праймеры** VR VF2

![PCR_gel](https://github.com/intbio/2019_igem/blob/master/dCas9_PCR.png)
![SM0311](https://github.com/intbio/2019_igem/blob/master/SM0311.jpg)

Размер ПЦР фрагмента около 2500

**Праймеры** 
- Suffix-f: ACTAGTAGCGGCCGCTGCAG
- Prefix-r2: CTCTAGAAGCGGCCGCGAATTC

![dCas9_PSCR](https://github.com/intbio/2019_igem/blob/master/dCas9_PCR_prefix_suffix.jpg)
![SM0311](https://github.com/intbio/2019_igem/blob/master/SM0311.jpg)

Размер около 4000

**Секвенирование dCas9**

[VR](https://benchling.com/kosarimn97/f/nW0uzvMM-sequnces/seq-NXhU28Sp-p6_11j_vr_h9/edit) [VF2](https://benchling.com/kosarimn97/f/nW0uzvMM-sequnces/seq-9vPXULxG-p6_11j_vf2_g9/edit)
