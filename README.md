# Articoli-Scientifici


<p align="left">
    <a href="https://circleci.com/gh/huggingface/transformers">
        <img alt="Unisalento" src="https://upload.wikimedia.org/wikipedia/it/8/87/Universit%C3%A0_del_Salento_logo.png">
    </a>
    </br>
    <a href="https://circleci.com/gh/huggingface/transformers">
       <img alt="Pytorch" src="https://img.shields.io/badge/Books-red.svg">
    </a>
   <a href="https://circleci.com/gh/huggingface/transformers">
       <img alt="Pytorch" src="https://img.shields.io/badge/Youtube-playlists-green.svg">
    </a>    
     <a href="https://github.com/ardalcar">
       <img alt="Pytorch" src="https://img.shields.io/github/gist/stars/2a09bc1qk55vk7wjgzg3pmxlh59rv5dlgewd9jem5nrt4w?style=social">
    </a>    
</p>

# Article list

1. [Allworth, J.; Windrim, L.; Bennett, J.; Bryson, M. A transfer learning approach to space debris classification using observational light curve data. Acta Astronaut. (2021)](https://www.sciencedirect.com/science/article/pii/S0094576521000588)

Correlato all'articolo (3), in prima battuta spiega come ricavare le curve di luce (LC) da un video di osservazione ottica; in seconda battuta spiega il metodo utilizzato per trasferire l'addestramento da LC fittizie a reali. La rete utilizzate è la 1D-CNN composta da 3 sezioni: Convolutional section; fully connected section e Object classification section.
I due step di trasferimento sono:
* addestramento su LC simulate e salvataggio dei pesi della Convolutional section
* addestramento su LC reali partendo da un preaddestramento sulla prima sezione ed inizializzazione casuale sul fully connected section.

L'ambiente di simulazione Blender è stato utilizzato per generare un set di dati contenente 4500 curve di luce per 13 diversi modelli di satellite.
Per le curve di luce reale si è utilizzato il dataset pubblico del Multichannel Monitoring Telescope (MMT)  da cui sono state estratte 500 LC per ognuna delle 8 classi di satelliti utilizzate.
Lo studio propone un iteressante metodo per correlare curve di luce reali a curve di luce simulate, permettendo di avere risultati rilevanti anche con un dataset di LC realit limitato. Tuttavia resta sempre nell'ambito della classificazione di oggetti.
Attinenza al 75%

2. [S. Mahendran H. Ali R. Vidal: 3D Pose Regression using Convolutional Neural Networks. Proceedings of the IEEE International Conference on Computer Vision Workshops(2017)](https://arxiv.org/abs/1708.05628)

Utilizza una rete composta da 2 reti in successione:
* Feature Network, classification immage in 4 categorie
* Pose Network, regressione lineare per trovare i quaternioni relativi all'orientamento dell'immagine

Lo studio del pose network è sicuramente interessante ed inoltre spiega l'utilizzo di TensorFlow per disegnare la rete. 
Attinenza al 65%

3. [R. Linares, R. Furfaro, V. Reddy: Space objects classification via light-curve measurements using deep convolutional neural networks. The Journal of the Astronautical Sciences, (2020) - Springer](https://doi.org/10.1007/s40295-019-00208-w) 

La ricerca parla di classificazione attraverso la Convolutional Neural Network (CNN)
* Test con 1000 LC simulate per 4 classi di satelliti (frammenti, rocket body, prismi, cuboidi)
* Test con 500 LC vere per 3 classi (Debris, Rocket body, Sat Attivo)

Il dataset è pubblico ma su un sito russo.
Attinenza intorno al 60% 

4. [G. P. Badura, C. R. Valenta, B. Gunter: Convolutional Neural Networkis for Inference of Space Object Attitude Status. The Journal of the Astronautical Sciences, (2022) - Springer](https://doi.org/10.1007/s40295-022-00309-z) 

La ricerca parla di classificazione attraverso la Convolutional Neural Network (CNN)
* Test con 7500 LC simulate per 4 classi di manovre (puro rotolamento, accelerazione in rotazione, stabilizzazione e inattivo)

Attinenza sempre intorno al 60%


---

The book of why <br>
978-0-465-09760-9<br><br>  


[Dive into Deep Learning](https://d2l.ai/)  <br>
(freely available)<br><br>

[Earth Observation Data Cubes](https://www.opendatacube.org/_files/ugd/f9d4ea_9357a7188c64483fbbce9378a23aa1e9.pdf)<br>
(freely available)<br><br>

[My data science notes](https://www.overleaf.com/read/pkqvmdkywmhn)<br>
[Git repository](https://github.com/Lorenzo-Epifani/DataScienceNotes)<br><br>


# Videos
## Lectures

[Deep Learning Lecture - Frank Noe (Berlin University)](https://www.youtube.com/playlist?list=PLqPI2gxxYgMKN5AVcTajQ79BTV4BiFN_0)<br>

## Series
[Statquest - Various statistics and classical learning content](https://www.youtube.com/c/joshstarmer/playlists)

[DigitalSreeni - various python/deep learning playlists](https://www.youtube.com/c/DigitalSreeni/playlists)<br>

## Papers explanations/misc

[AladdinPersson - paper explanations and python tutorials](https://www.youtube.com/c/AladdinPersson/playlists)<br>

[Yannic Kilcher - paper explanations](https://www.youtube.com/c/YannicKilcher/playlists)<br>


# Datasets
[Sentinel-2 Image Time Series for Crop Mapping (68GB)](https://www.kaggle.com/datasets/ignazio/sentinel2-crop-mapping) <br>
[SenseFLy education dataset(s)](https://www.sensefly.com/education/datasets/) <br>
[Agriculture for Vision, dataset 2021](https://www.agriculture-vision.com/agriculture-vision-2021/dataset-2021)<br>
[Agriculture for Vision, dataset 2022](https://www.agriculture-vision.com/agriculture-vision-2022/prize-challenge-2022/agriculture-vision-challenge-2022)<br>
[awesome-public-datasets](https://github.com/awesomedata/awesome-public-datasets)<br>
[COCO dataset](https://cocodataset.org/#home)<br>

# Other Resources

[Vision for agriculture](https://www.agriculture-vision.com/)<br>
[Earth Observation Using Python](https://github.com/resmaili/Earth-Obs-Py)<br>
[SentinelSat API reference](https://sentinelsat.readthedocs.io/en/stable/api_reference.html)

 
