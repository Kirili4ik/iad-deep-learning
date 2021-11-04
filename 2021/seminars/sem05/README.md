### ResNet, Transfer learning и Adversarial exaples 

- Шапргалка по теории: <a href="https://kirili4ik.notion.site/5-ResNet-Transfer-learning-FGSM-b0fd062aaf0247dc9d1f949af76de445">
      <img align="center" src="https://img.shields.io/badge/Notion-000000?logo=notion&logoColor=white"/>
  </a>

- Задание [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kirili4ik/iad-deep-learning/blob/master/2021/seminars/sem05/sem05_task.ipynb)
- Чистое решение [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kirili4ik/iad-deep-learning/blob/master/2021/seminars/sem05/sem05_solution.ipynb)
- Видео семинара (TBD)



Исправлений в ноутбуке было не очень много, зато можно дать небольшое объяснение к самому концу ноутбука:

Почему в итоге мы получили при отрисовке разные цвета, а не черный/белый? Мы же берем знак, то есть +1/-1? Дело в том, как мы рисуем картинку. На самом деле у картинки 3 канала - RGB. Когда мы сделали torch.sign(image.grad) каждый пиксель это RGB и выходит, например, [+1, -1, -1], а при отрисовке получается 1\*Red-1\*Blue-1*Green. Таким образом и получаются отрисованные цвета типа magenta или yellow=green+blue

Скажем, изначально в картинке пиксель RGB [0.3, -0.3, 0.7], а мы во время атаки добавляем +0.007*[-1, -1, +1].


##### Дополнительные материалы:
> [Немного о Transfer Learning @ FullStackDeepLearning.com](https://fullstackdeeplearning.com/spring2021/lecture-4/)
>
> [Paper on ResNet @ arxiv](https://arxiv.org/abs/1512.03385)
>
> [Моя презентация про Adversarial examples](https://github.com/Kirili4ik/pres-n-articles/blob/master/Adversarial_examples.pdf) (в конце есть ссылки на хорошие материалы по теме)
