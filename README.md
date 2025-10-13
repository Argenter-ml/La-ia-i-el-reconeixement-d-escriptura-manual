# La IA i el reconeixement d'escriptura manual

Aquest projecte explora diferents **models i xarxes neuronals** per al **reconeixement de caràcters escrits a mà**, incloent-hi tant **lletres com dígits**.  
A més d’entrenar i comparar diversos models, també s’han desenvolupat **interfícies gràfiques** que permeten **dibuixar els caràcters manualment** i veure com el model els reconeix en temps real.

---

## Objectiu del projecte

L’objectiu principal és **avaluar l’eficàcia de diferents arquitectures de xarxes neuronals** (MLP i CNN) en la tasca de classificació de caràcters manuscrits.  
Per fer-ho, s’han entrenat cinc models diferents utilitzant la base de dades **EMNIST**, que conté mostres d’escriptura manual de lletres i dígits.

---

## Estructura del repositori

```bash
.
├── README.md
├── LICENSE
│
├── notebooks/
│   ├── model_mlp1.ipynb
│   ├── model_mlp2.ipynb
│   ├── model_CNN3.ipynb
│   ├── model_CNN4.ipynb
│   └── model_CNN5.ipynb
│
├── data/
│   └── (fitxers EMNIST o scripts per importar-los)
│
├── results/
│   └── (imatges, gràfics i resultats)
│
└── src/
    └── (funcions auxiliars o interfícies gràfiques)
```
## Models inclosos

| Nº | Nom del model | Descripció | Resultats | Fitxer |
|----|----------------|-------------|------------|---------|
| 1 | **Model_MLP_1** | Xarxa MLP bàsica que assenta les bases del projecte. | 🎯 90% taxa d'encert | [`model_mlp1.ipynb`](notebooks/model_mlp1.ipynb) |
| 2 | **Model_MLP_2** | Xarxa MLP millorada que augmenta la precisió respecte al model anterior. | 🎯 91.3% taxa d'encert | [`model_mlp2.ipynb`](notebooks/model_mlp2.ipynb) |
| 3 | **Model_CNN_Lletres_Dígits** | CNN capaç d’identificar tant lletres com dígits amb més precisió. | 🎯 93% taxa d'encert | [`model_CNN3.ipynb`](notebooks/model_CNN3.ipynb) |
| 4 | **Model_CNN_Lletres** | CNN centrada exclusivament en la detecció de lletres amb alta precisió. | 🎯 93.26% taxa d'encert | [`model_CNN4.ipynb`](notebooks/model_CNN4.ipynb) |
| 5 | **Model_CNN_Dígits** | CNN especialitzada en el reconeixement de dígits amb resultats excel·lents. | 🎯 99.38% taxa d'encert | [`model_CNN5.ipynb`](notebooks/model_CNN5.ipynb) |

---

## Dataset utilitzat

S’ha fet servir la base de dades **[EMNIST (Extended MNIST)](https://www.nist.gov/itl/products-and-services/emnist-dataset)**, que conté mostres d’escriptura manual de caràcters en format d’imatges de 28x28 píxels.  
Els fitxers s’han descarregat i importat localment per entrenar els models.

---

## Llibreries i entorn

El projecte utilitza **Python** amb les següents dependències principals:

```text
numpy
pandas
matplotlib
scikit-learn
tensorflow
opencv-python
tkinter
