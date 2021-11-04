### MAP(Mean Average Precision), Segmentation, UNet, Detection

- Задание [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kirili4ik/iad-deep-learning/blob/master/2021/seminars/sem06/sem_06.ipynb)
- Чистое решение [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kirili4ik/iad-deep-learning/blob/master/2021/seminars/sem06/sem_06_solved.ipynb)
- Видео семинара (TBD)

О свертках с ядром 1х1:
> 1x1 свертка просто уменьшает кол-во каналов (глубину). Колбаска(вектор) 1x1xCH_in переведет в 1x1x1, но мы таких возьмем CH_out штук -> получим из входа NxMxCH_in выход NxMxCh_out.

Часть семинара:

![](https://github.com/Kirili4ik/iad-deep-learning/blob/master/2021/seminars/sem06/FalseNegativeVolk.jpg)

##### Дополнительные материалы:
> [Красивый блогпост про checkerboard effect на distill.pub](https://distill.pub/2016/deconv-checkerboard/)
>
> [Блогпост про R-CNN (и следующие) на habr](https://habr.com/ru/company/jetinfosystems/blog/498294/)
