# ITMO_Plate_number_recognition

Описание файлов репозитория:
train_yolo5.ipynb                Код дообучения yolo5 на дастасете с гос. номерами.
detecto_train.ipynb              Код дообучения Resnet из библиотеки Detecto.
detecto_inference.ipynb          Код запуска модели дообученной в detecto и тест на картинке с номером.
inference_yolo5+detecto.ipynb    Пайплайн yolo5+ Detecto запускается на видео с гос номером.
seformer_train.ipynb             Процесс обучения segformer на базе библиотеки transformers от huggingface.
                                 Получение датасета из сервиса разметки segments. Преобразование датасета в hf.Datasets.
                                 Инициализация парамемтров обучения и обучение модели.
                                 Инференс на примере картинок из интернета.


https://youtu.be/gGTMRvCN_zI     Ссылка на видиео с демонстрацией работы дообученной yolo5.  
