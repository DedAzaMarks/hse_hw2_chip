# hse_hw2_chip
## Бордюгов Максим, группа 1
Colab: https://colab.research.google.com/drive/1nMRbmbMQ0rnkL9z_vVosOAB414bvtecG?usp=sharing
- Клеточная линия: A549
- Гистоновая метка: H3K4me1
- Эксперимент: https://www.encodeproject.org/experiments/ENCSR000AVH/

|                                         | ENCFF000AIT                            | ENCFF000AIS                            | ENCFF000AHJ                            |
| :-------------------------------------: | -------------------------------------: | -------------------------------------: | -------------------------------------: |
| Per base sequence quality               | ![AIT1](img/AIT/1.png "img/AIT/1.png") | ![AIS1](img/AIS/1.png "img/AIS/1.png") | ![AHJ1](img/AHJ/1.png "img/AHJ/1.png") |
| Per tile sequence quality               | ![AIT2](img/AIT/2.png "img/AIT/2.png") | ![AIS2](img/AIS/2.png "img/AIS/2.png") | ![AHJ2](img/AHJ/2.png "img/AHJ/2.png") |
| Per sequence quality scores             | ![AIT3](img/AIT/3.png "img/AIT/3.png") | ![AIS3](img/AIS/3.png "img/AIS/3.png") | ![AHJ3](img/AHJ/3.png "img/AHJ/3.png") |
| Per base sequence content               | ![AIT4](img/AIT/4.png "img/AIT/4.png") | ![AIS4](img/AIS/4.png "img/AIS/4.png") | ![AHJ4](img/AHJ/4.png "img/AHJ/4.png") |
| Per sequence GC content                 | ![AIT5](img/AIT/5.png "img/AIT/5.png") | ![AIS5](img/AIS/5.png "img/AIS/5.png") | ![AHJ5](img/AHJ/5.png "img/AHJ/5.png") |
| Per base N content                      | ![AIT6](img/AIT/6.png "img/AIT/6.png") | ![AIS6](img/AIS/6.png "img/AIS/6.png") | ![AHJ6](img/AHJ/6.png "img/AHJ/6.png") |
| Sequence Duplication Levels             | ![AIT7](img/AIT/7.png "img/AIT/7.png") | ![AIS7](img/AIS/7.png "img/AIS/7.png") | ![AHJ7](img/AHJ/7.png "img/AHJ/7.png") |
| Adapter Content                         | ![AIT8](img/AIT/8.png "img/AIT/8.png") | ![AIS8](img/AIS/8.png "img/AIS/8.png") | ![AHJ8](img/AHJ/8.png "img/AHJ/8.png") |
| __Общее количество ридов__              | 40417850                               | 35671032                               | 38269770                               |
| __Не выровнилось__                      | 33802975                               | 29703964                               | 31293422                               |
| Не выровнилось (в процентах)            | 83.63%                                 | 83.27%                                 | 81.77%                                 |
| __Выровнилось уникально__               | 2273997                                | 1750514                                | 1874146                                |
| Выровнилось уникально (в процентах)     | 5.63%                                  | 4.91%                                  | 4.90%                                  |
| __Выровнилось больше 1 раза__           | 4340878                                | 4216554                                | 5102202                                |
| Выровнилось больше 1 раза (в процентах) | 10.74%                                 | 11.82$                                 | 13.33%                                 |

![venn1](img/venn1.png "img/venn1.png")

![venn2](img/venn2.png "img/venn2.png")

![venn3](img/venn3.png "img/venn3.png")

![venn4](img/venn4.png "img/venn4.png")

Дополнительное считается в colab

__Ответы на вопросы__:
- _Почему процент выравниваний получился именно таким?_  
Процент выравнивания получился низний из-за того что выравнивание проводилось только на одну хромосому.
- _Проанализируйте полученные результаты. Как можно объяснить различия в количестве пересечений?_  
Из-за выравнивания на одну хромосому число пиков довольно маленькое. Поэтому пересекающихся участков тоже мало. Количество пересечений считается как число пиков в одном файле, которые встретились в другом ( и наоборот). Из-за этого и получаются разные значения.