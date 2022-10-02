# ITMO_Plate_number_recognition

Описание файлов репозитория:

train_yolo5.ipynb                код дообучения yolo5 на дастасете с гос. номерами.

detecto_train.ipynb              код дообучения Resnet из библиотеки Detecto.

detecto_inference.ipynb          код запуска модели дообученной в Detecto и тест на картинке с номером.

inference_yolo5+detecto.ipynb    пайплайн yolo5+ Detecto запускается на видео с гос номером.

seformer_train.ipynb             Процесс обучения segformer на базе библиотеки transformers от huggingface.
                                 Получение датасета из сервиса разметки segments. Преобразование датасета в hf.Datasets.
                                 Инициализация парамемтров обучения и обучение модели.
                                 Инференс на примере картинок из интернета.



https://drive.google.com/file/d/1CtwtQBOKxNQbYaRqofxRFJRy63hLurSf/view?usp=sharing    Ссылка на датасет, на котором дообучали yolo5.


https://youtu.be/gGTMRvCN_zI     Ссылка на видео с демонстрацией работы дообученной yolo5. 

https://youtu.be/Opa3ss7x7cs     Ссылка на видео с демонстрацией работы дообученнйх yolo5 и Detecto (рамка с номером и распознанные символы отображаются на видео). 
