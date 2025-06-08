# Dashboard d'Emigració i Desenvolupament Global (1990-2020)

**Autor:** Sergi Bartra Juan  
**Projecte:** Visualització de Dades (UOC)

### ✨ [VEURE EL DASHBOARD EN VIU](https://sbartrajvdd.shinyapps.io/dashboard_practicaII/) ✨


Aquest repositori conté el codi font d'un dashboard interactiu creat amb **R**, **flexdashboard** i **shiny**. L'objectiu és explorar la relació entre les taxes d'emigració i diversos indicadors de desenvolupament humà i econòmic a nivell mundial entre els anys 1990 i 2020.

## 🎯 Objectiu del Projecte

El dashboard ha estat dissenyat per a ser una eina intuïtiva que permet a usuaris (analistes, estudiants, periodistes o ciutadans curiosos) respondre preguntes clau sobre desenvolupament i migració, com ara:

-   Com han evolucionat indicadors com l'esperança de vida o el PIB per càpita a les diferents regions del món?
-   Quines correlacions existeixen entre el desenvolupament econòmic i la qualitat de vida?
-   Com es posiciona un país específic en comparació amb la mitjana de la seva regió?
-   Quines trajectòries de desenvolupament han seguit diferents nacions al llarg de les últimes tres dècades?

## 🚀 Característiques Principals

El dashboard s'estructura en tres pestanyes principals per facilitar una exploració des del nivell global fins al detall per país:

### 1. Panorama Global
-   **Mapa Mundial Interactiu:** Visualitza qualsevol indicador seleccionat per a un any concret. Els països es coloregen segons el seu valor, permetent una identificació ràpida de patrons geoespacials.
-   **Rànquing Top 10:** Mostra els 10 països amb el millor rendiment per a l'indicador i any seleccionats.
-   **Estadístiques Globals:** Ofereix un resum (mitjana, mediana, màxim, mínim) de l'indicador a nivell mundial.

### 2. Anàlisi per Regió
-   **Distribució Regional:** Un gràfic de caixes (`boxplot`) que compara la distribució de l'indicador entre les diferents regions del món, destacant desigualtats.
-   **Trajectòries Animades:** Un gràfic de dispersió animat que mostra l'evolució de múltiples països al llarg del temps, comparant dos indicadors simultàniament.

### 3. Anàlisi per País
-   **Evolució Temporal:** Un gràfic de línies que mostra l'evolució d'un indicador per a un país seleccionat.
-   **Comparativa Regional:** Compara el valor del país seleccionat amb la mitjana de la seva regió, oferint un context immediat.
-   **Anàlisi de Correlació:** Un gràfic de dispersió que mostra la relació entre dues variables, destacant la posició del país seleccionat.

## 🛠️ Tecnologies i Eines

Aquest projecte s'ha desenvolupat íntegrament en **R** i aprofita un ecosistema de paquets especialitzats en anàlisi i visualització de dades:

-   **Estructura i Interactivitat:** `flexdashboard`, `shiny`
-   **Visualització de Dades:** `ggplot2`, `plotly`, `leaflet`, `DT`
-   **Manipulació de Dades:** `dplyr`, `tidyr`, `countrycode`, `sf`, `rnaturalearth`

## 📊 Font de Dades

El conjunt de dades principal prové de **"Global Emigration and Development"** a Kaggle, que agrega informació de fonts oficials com el Pew Research Center i el World Bank.

-   **Enllaç al Dataset:** [Global Emigration and Development a Kaggle](https://www.kaggle.com/datasets/mahyarentezari/emigration)
-   **Llicència de les dades:** Creative Commons (CC BY-SA 4.0).

## 📝 Compliment amb l'Enunciat de la Pràctica

Aquest projecte ha estat dissenyat per complir tots els requisits de l'enunciat de la pràctica de l'assignatura "Visualització de Dades" de la UOC:

1.  **Preguntes i Objectius:** La pestanya "Sobre el Dashboard" estableix clarament les preguntes que es volen respondre i els objectius de la visualització, servint com a introducció al relat visual.

2.  **Anàlisi Visual i Justificació:** S'han escollit gràfics adequats per a cada propòsit: mapes per a la distribució geogràfica, boxplots per a comparar distribucions, gràfics de línies per a sèries temporals i scatter plots per a analitzar correlacions, complint els criteris d'expressivitat i efectivitat.

3.  **Elements Interactius:** La interactivitat és un pilar fonamental del projecte. L'usuari pot filtrar per any, seleccionar indicadors i països, i explorar les dades directament sobre els gràfics (hover, zoom). Aquestes interaccions fomenten l'exploració lliure i el descobriment de patrons.

4.  **Composició i Disseny Visual:** S'ha implementat una composició coherent amb una estructura de pestanyes lògica. El disseny visual és consistent gràcies a un tema fosc personalitzat, garantint una bona llegibilitat i una experiència d'usuari agradable. Tots els gràfics inclouen títols, llegendes i etiquetes clares per facilitar la seva interpretació.
