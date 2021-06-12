# Projeto_Amor_de_Mae
Esse projeto contém as análises de dados do SUS e IBGE a respeito da vacinação em gestantes e óbitos fetais no Brasil e no Nordeste 
[<img src="https://img.shields.io/badge/author-Glaudemias-yellow?style=flat-square"/>](https://github.com/Glaudemias)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZcJLDEQBu6MBYJy_MRp0Ez6EmpDNLuKr?usp=sharing)
![Dengue - Glaudemais_JPG](https://user-images.githubusercontent.com/84024639/120666112-b8ba7a80-c462-11eb-985a-10d5a483fa93.jpg)

                                                                            [INCOMPLETE]

# Contents
* Introduction
* Data
* Methodology
* Tooling
* Concluisions
* Acknowledgments
* References

# Introduction

This project is the result of module 2, of the Bootcamp in Data Science applied (second edition) proposed by Alura and apoint to some analisys about the numbers of vaccines in pregnant women and fetal deaths from 1994 to 2019 in Brazil and the northeastern states of the country. These [data](#dt) are available in two official website of brazilian gorvenment: 
* Data about vaccine, were found in the official website of brazilian Bealthcare System: [DATASUS](https://www.gov.br/saude/pt-br/assuntos/saude-de-a-a-z-1/s/sistema-unico-de-saude-sus-estrutura-principios-e-como-funciona) 
* Data about fetal death, were found in the official website of Brazilian Institute of Geography and Statistics: [IBGE](https://sidra.ibge.gov.br/tabela/2992) 

Based on this I'll analyse the vaccine curve in  Brazil and in the states(with a focus on the northeastern states), seeking to answers and trying to understand the dynamics of the relationship between vaccines and  fetal deaths in Braazil.

## Vaccines x Fetal Death
  The Vacination of pregnant women its priority to World Health Organization (WHO), and represents the first love act betwen a mother and your baby. The vaccines prevant some complicantion in the birth moment and the diseases development during the child's growth. The maternal antibodies are very important to the baby health in the first 12 months of the pregnancy, when it still in the mother womb. The antibodies provided by the mother, protect the baby, until it can be vaccinated and develops his own immune defenses. 
  
 According to the Brazil Ministry Health , the vaccination of women pregnant reduces the numbers of fetal deaths, wich can be definide as the baby's deaths due to complications during the childbirth or the pragnancy. Besides to influence in the bith rate, the fetal death can be an indicator that help a visualization of spatial distribution, and the quality of woman health assistance. So the vaccination is responsable for avoiding problemns like:     
 
* Congenital malformations and pregnancy damage (abortion, premature birth...);

* Pregnant women and babies, constitue a high risk group for the influenza virus, and vacination can avoid the hospitalization and severe respiratory conditions caused by the virus;

* Whitout Knowing it, woman can transmit the Hepatitis B virus, to your baby;

![vacina](https://user-images.githubusercontent.com/84024639/121777943-f0b07480-cb6a-11eb-8831-cf33d4919c0d.jpeg)

## Vaccines analyzed

  In this project there was four vaccines it was analyzed:
  * **Hepatitis-B:**
    * The vaccination protects against the contamination for hepatitis virus, and avoid problemns such as liver inflamation, that can cronify and cause cancer and cirrhosis.
  * **DT:**
    * The Vaccination protect against the diphtheria and tetanus.  
  * **DTPA:**
    * The Vaccination protect against the diphtheria, tetanus and whooping cough.
  * **Yellow Fever:**
    * The Yellow Fever vaccination in pregnant women its a particular case, since the immunizing against the yellow fever, its made by the live virus. But acoording to the Center of Imunization for the Hospital and Maternity Santa Joana (São Paulo), and the website Vacinas para Gravidas (Vaccines for Pregnant woman, in literal traduction) such as the old people, pregnant woman hardly can develop the complication by the vaccines, and this particular vaccine it's used in special localities, when was developed many cases of yellow fever.
 
<a name="dt"></a>
# Data

The data used in this analysis was obtained from the DATASUS aplication TABNET, and the IBGE aplication SIDRA on Jun 06, 2021, and you can find them, [here](https://github.com/Glaudemias/PROJETO_FINAL_MOD1-DS_2-Bootcamp_Alura/tree/main/Dados) on my repositorie. The datasets chosen have an incompatibility of the dates, and for that I decided divide them in 2 groups of the vaccines curves, wich is:

* **Group 1**
  * The vacines curves from 1994 to March 2021:
    * Hepatitis-B and Yellow Fever  
* **Group 2**
  * The vacines curves from 2013 to March 2021:
    * DTPA and DT  
And this information is used to:
  * To compare the progression of each vacine curve in Brasil;
  * To demonstrate the mosts affecteds states, with a focous on the Northeastern states.
The Five dataset analysed here, was the numbers cases of fetal deaths ranges from 2003 to 2019, in Brasil 
* Number of Deaths for Dengue Cases ranges from January 2008 to March 2021:
And this information is used to:
  * To make the comparative studies above;
  * And was used to make a statiscal aproximation, of the percentage of vaccines numbers/fetal deaths, by the year.
  
A detailed description of each vaccine curve dataset and its meaning is also provided in the DATASUS website, you can find [here](http://tabnet.datasus.gov.br/cgi/pni/Imun_doses_aplic_desde_1994.pdf)

# Methodology
The datasets are analysed following the logic of approximation of the scale, when the first moment I looking for the distribution of the vaccine curve and fetal deaths per year, in the country. The Second part I'll analyse the same datasets across the brazilian states, trying to find some correlation, and understanding the distribution of vaccine and fetal deaths in the northeastern states. Finally I'will analysed the distibution the same datasets but, in this last part the data will spatialized in a map, considering the most critical year's and all brazilian states.

With this we were able to made some conclusions about the variables observerd, you cand find them in the [Conclusion](#concl)

# Tooling (Libraries and Technology)
This project are made in the python 3.8.5, used the Collab the cloud storage services of google, Google Collaboratory.The libraries used here, were:

* Pandas, the main librarie of data analysis in Python, used to manipulate and help in statiscal conclusion about the datasets;
* Numpy, using to heandle missing data;
* date, to transform columns in date type;
* Seabornd,Matplotlib.pyplot, for plotting of the charts;
* Geopandas, for plotting the map.


<a name="concl"></a>
# Conclusion

# Acknowledgments
This project as said before, was proposed as a second project in the Alura's Bootcamp, as an introduction to the Data Science world. So I'm gonna say thank you one more time, to Guilherme and Thiago, for the knowledge passed on to the students, to scuba team and all the comunity it was created on the discord, you guys help so many time. THANKYOU :)

# References
**1. Papers:**

1.1. 
[Paper1](https://www.scielo.br/pdf/rsbmt/v40n2/a09v40n2.pdf) - Estudo retrospectivo (histórico) da dengue no Brasil: caracteristicas regionais e dinâmicas 

1.2. 
[Paper2](http://scielo.iec.gov.br/scielo.php?script=sci_arttext&pid=S1679-49742007000200006) - Aedes aegypti: histórico do controle no Brasil

1.3. 
[Paper3](https://www.scielo.br/j/rsp/a/zCKRhC7DZX9XZmJhYy9cTgx/?lang=pt) - Dengue em localidade urbana da região sudeste do Brasil: aspectos epidemiológicos

1.4.
[Paper4](https://www.scielo.br/j/rsp/a/wvzJGdfCKHSQSzG5WYg8wYR/?lang=pt) - Distribuição espacial da dengue e determinantes socioeconômicos em localidade urbana no Sudeste do Brasil


**2. Articels and specialized health sites**

2.1.  [Artcle1](https://g1.globo.com/ciencia-e-saude/noticia/2020/01/15/ministerio-da-saude-diz-que-11-estados-poderao-ter-surto-de-dengue-em-2020.ghtml) - Ministério da Saúde diz que 11 estados poderão ter surto de dengue em 2020


2.2. [Article2](http://www.ioc.fiocruz.br/dengue/textos/longatraje.html) - O mosquito Aedes aegypti faz parte da história e vem se espalhando pelo mundo desde o período das colonizações


2.3. [Article3](http://www.saude.ba.gov.br/suvisa/vigilancia-epidemiologica/doencas-de-transmissao-vetorial/arboviroses-dengue-chikungunya-zika-e-febre-amarela/) - Arboviroses – Dengue, Chikungunya, Zika e Febre Amarela

# Contact
If you have any tips or suggestions, feel free to contact me here:

[![Linkedin Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/glaudemias-grangeiro-junior-940a951a1/)](https://www.linkedin.com/in/glaudemias-grangeiro-junior-940a951a1/)

[<img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=Gmail&logoColor=white" />](mailto:glaudemias.arqurb@gmail.com)



