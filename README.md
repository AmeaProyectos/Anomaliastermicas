# Thermal Anomalies _Anomalías térmicas_

This data science project focuses on the detection and analysis of thermal anomalies in Antarctica, a crucial region for understanding global climate changes. By using advanced data analysis techniques and machine learning algorithms, our goal is to identify patterns and unusual variations in the temperatures of this sensitive area

This project is deployed on [streamlit](https://streamlit.io/) , check the [unnoficial deployment](https://anomaliastermicas-nasa-78qz783ztianqksa2zagpy.streamlit.app/)

To run the local streamlit, clone the repo then run:

`pip install -r requirements.txt`
`streamlit run app.py`

Then a new tab should open on the localhost project.

This dashboard is based on this [Collab notebook](https://colab.research.google.com/drive/1C1NwTP7Mx9uU03MzuIMs1nU_cOSei7hr?usp=sharing#scrollTo=JkoFueVH0Dfr)

The code for such notebook is also on this repo under the **notebooks** folder

It downloads [Nasa](https://power.larc.nasa.gov) data from the following cities and corresponding global coordinates:

| City                | Coordinates        |
| ------------------- | ------------------ |
| Acapulco, Mex       | 16.793542,-99.8349 |
| San Jose, Gua       | 13.9234, -91.1628  |
| Acajutla, Sal       | 13.5242, -89.7991  |
| San Rafael Sur, Nic | 11.8274, -86.5377  |
| Parrita, Cos        | 9.4839, -84.2999   |
| Pedasi, Pan         | 7.4261, -80.0924   |
| Buenaventura , Col  | 3.8461, -77.3266   |
| Perdernales, Ecu    | 0.0876, -80.0691   |
| Colán, Per          | -5.0078, -81.0684  |
| Lima, Per           | -12.1085, -77.0831 |
| Antofagasta, Chi    | -23.6333, -70.4103 |

The data is from the following periods:

| Start    | End      |
| -------- | -------- |
| 19810101 | 19911231 |
| 19920101 | 20021231 |
| 20030101 | 20131231 |
| 20140101 | 20230810 |

Then anomalies are computed by substracting the **Average temperature** to the **Temperature**

Then there are two plots one for the line for the temperature and a scatter for the anomlies
