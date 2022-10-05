### ITMO_Plate_number_recognition

$~~~~~~~~~$

__Описание файлов репозитория:__

inference_yolo5+detecto.ipynb $~~~~~~~~~$ _Пайплайн yolo5+ Detecto запускается на видео с гос номером._

requirements.txt  $~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~$ _Список библиотек и их версий._

***
__Папка yolo__

train_yolo5.ipynb    $~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~$   _Код дообучения yolo5 на дастасете с гос. номерами._

data.yaml    $~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~$   _Конфигурационный файл для дообучения yolo5._


***

segformer_license_plate  $~~~~~~~~~~~~~~~~~~~~~$  _Папка с кодом для segformer. Обучение segformer на базе библиотеки transformers от huggingface._


***
__Папка detecto__

detecto_train.ipynb  $~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~$   _Код дообучения Resnet из библиотеки Detecto._

detecto_inference.ipynb $~~~~~~~~~~~~~~~~~~~~~$ _Код запуска модели дообученной в Detecto и тест на картинке с номером._

EasyOCR_test_on_plates.ipynb   $~~~~~~~~~~$  _Код тестирования EasyOcr на фотографиях с номерами, замеры скорости и точности._

detecto_test_on_plates.ipynb  $~~~~~~~~~~~~$   _Код тестирования Detecto на фотографиях с номерами, замеры скорости и точности._

test_plate.png      $~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~$  _Тестовое фото с номером на котором запускался файл detecto_inference.ipynb_



Сравнение Detecto и EasyOcr проводилось на 2845 фото с номерами.

Сравнение                    | Detecto | EasyOcr  
:----------------------------|:-------:|---------:
Accuracy                     | 0.745   | 0.182
Обработанных фото в секунду  | 28,45   | 44,45    


***

https://drive.google.com/file/d/1CtwtQBOKxNQbYaRqofxRFJRy63hLurSf/view?usp=sharing   $~~~~~~~~~~$  _Ссылка на архив с датасетом, на котором дообучали Yolo5._

https://drive.google.com/file/d/1KZ3xQCUj9XKREW2jDrPcl4Zwo-UgOZq9/view?usp=sharing  $~~~~~~~$  _Ссылка на архив с фотографиями и разметкой, на которых дообучали Detecto._

https://drive.google.com/file/d/1PSemzoMMqLW5OJhw9UUhh5ej3i8PxsGs/view?usp=sharing  $~~~~~$  _Ссылка на веса дообученной Yolo5._

https://drive.google.com/file/d/1x9ylDT3atD_tS7-GYSW6ecm0FnnvcQc_/view?usp=sharing  $~~~~~~~~~~$  _Ссылка на веса дообученной в Detecto Resnet50._


https://youtu.be/gGTMRvCN_zI   $~~~~~~~~$  _Ссылка на видео с демонстрацией работы дообученной yolo5._

https://youtu.be/Opa3ss7x7cs   $~~~~~~~~~~$  _Ссылка на видео с демонстрацией работы дообученнйх yolo5 и Detecto (рамка с номером и распознанные символы отображаются на видео)._ 

https://youtu.be/qEU8Up3fZ2A   $~~~~~~~~$  _Ссылка на видео с демонстрацией работы дообученнйх yolo5 и Detecto (рамка с номером и распознанные символы отображаются на видео). Вторая машина._

***

За неимением видеокарты Yolo5 и Resnet из Detecto дообучались в google colab. Из-за слухов о сокращении часов в бесплатной версии большое количество экспериментов проводить не рискнул. Для воспроизведения обучения Yolo5 нужно скопировать на свой гугл диск в корневую папку My drive архив с датасетом по ссылке выше, конфигурационный файл и сам файл train_yolo5.ipynb.
Для воспроизведения обучения Resnet в Detecto нужно скопировать на свой гугл диск в корневую папку My drive архив с датасетом по ссылке выше и файл detecto_train.ipynb.
