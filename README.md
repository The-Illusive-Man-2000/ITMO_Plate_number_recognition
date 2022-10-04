## ITMO_Plate_number_recognition



__Описание файлов репозитория:__

train_yolo5.ipynb                код дообучения yolo5 на дастасете с гос. номерами.

detecto_train.ipynb              код дообучения Resnet из библиотеки Detecto.

detecto_inference.ipynb          код запуска модели дообученной в Detecto и тест на картинке с номером.

inference_yolo5+detecto.ipynb    пайплайн yolo5+ Detecto запускается на видео с гос номером.

data.yaml                        Конфигурационный файл для дообучения yolo5.

test_plate.png                   Тестовое фото с номером на котором запускался файл detecto_inference.ipynb

segformer_license_plate          Папка с кодом для segformer. Код обучения segformer на базе библиотеки transformers от huggingface.
                                 Получение датасета из сервиса разметки segments. Преобразование датасета в hf.Datasets.
                                 Инициализация парамемтров обучения и обучение модели.
                                 Инференс на примере картинок из интернета.

EasyOCR_test_on_plates.ipynb     Код тестирования EasyOcr на фотографиях с номерами, замеры скорости и точности. 
detecto_test_on_plates.ipynb     Код тестирования Detecto на фотографиях с номерами, замеры скорости и точности.



Сравнение Detecto и EasyOcr проводилось на 2845 фото с номерами.

Сравнение                    | Detecto | EasyOcr  
:----------------------------|:-------:|---------:
Accuracy                     | 0.745   | 0.182
Обработанных фото в секунду  | 28,45   | 44,45    


***

https://drive.google.com/file/d/1CtwtQBOKxNQbYaRqofxRFJRy63hLurSf/view?usp=sharing    Ссылка на архив с датасетом, на котором дообучали Yolo5.

https://drive.google.com/file/d/1KZ3xQCUj9XKREW2jDrPcl4Zwo-UgOZq9/view?usp=sharing    Ссылка на архив с фотографиями и разметкой, на которых дообучали Detecto.

https://drive.google.com/file/d/1PSemzoMMqLW5OJhw9UUhh5ej3i8PxsGs/view?usp=sharing    Ссылка на веса дообученной Yolo5.

https://drive.google.com/file/d/1x9ylDT3atD_tS7-GYSW6ecm0FnnvcQc_/view?usp=sharing    Ссылка на веса дообученной в Detecto Resnet50.


https://youtu.be/gGTMRvCN_zI     Ссылка на видео с демонстрацией работы дообученной yolo5. 

https://youtu.be/Opa3ss7x7cs     Ссылка на видео с демонстрацией работы дообученнйх yolo5 и Detecto (рамка с номером и распознанные символы отображаются на видео). 

https://youtu.be/qEU8Up3fZ2A     Ссылка на видео с демонстрацией работы дообученнйх yolo5 и Detecto (рамка с номером и распознанные символы отображаются на видео). Вторая машина.

***

За неимением видеокарты Yolo5 и Resnet из Detecto дообучались в google colab. Из-за слухов о сокращении часов в бесплатной версии большое количество экспериментов проводить не рискнул. Для воспроизведения обучения Yolo5 нужно скопировать на свой гугл диск в корневую папку My drive архив с датасетом по ссылке выше, конфигурационный файл и сам файл train_yolo5.ipynb.
Для воспроизведения обучения Resnet в Detecto нужно скопировать на свой гугл диск в корневую папку My drive архив с датасетом по ссылке выше и файл detecto_train.ipynb.
