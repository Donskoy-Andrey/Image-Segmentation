# Задача
Требуется сегментировать изображения новообразований на коже из датасета ADDI Project с помощью одного из предложенных методов (Graph-based segmentation, Normalized cuts, Свёрточные нейронные сети). В качестве решения были использованы сверточные нейронные сети. 

При использовании нейронных сетей выборка разделена на train/test/validation в соотношении 100/50/50.\
Качество модели оценивается с помощью метрики IoU (Intersection over Union).

# Результат
Построены архитектуры SegNet и U-Net с 3 функциями потерь: BCE, Dice, Focal. Суммарно все 6 структур были обучены на 300 эпохах.\
Результаты метрик, а также графики изменения лосса представлены в блоках SegNet (Summary) и U-Net (Summary):

<p align="center">
  <img src="https://github.com/Donskoy-Andrey/Image-Segmentation/blob/master/segnet.png" />
  <img src="https://github.com/Donskoy-Andrey/Image-Segmentation/blob/master/unet.png" />
</p>

# Качество
Лучшая из полученных моделей – SegNet на Focal Loss, результат метрики – **0.792 на 240 эпохе.**
