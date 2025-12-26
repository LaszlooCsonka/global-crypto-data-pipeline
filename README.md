# global-crypto-data-pipeline
End-to-End Big Data Pipeline for Crypto Markets. Built with Python, PySpark, Airflow, and Docker. Architected for GCP (BigQuery, Dataproc, GKE) using Data Vault 2.0 modeling.


# Global Crypto Data Platform (Enterprise Edition)

## 📌 Project Overview
Ez a projekt egy professzionális, végponttól-végpontig tartó (End-to-End) Big Data platform, amely kriptovaluta piaci adatokat gyűjt, tisztít és elemez. A rendszer célja egy skálázható architektúra bemutatása, amely a lokális adatgyűjtéstől a felhőalapú (GCP) Big Data feldolgozásig terjed.

A projekt fejlesztése során a szoftverfejlesztési életciklust (SDLC) **Jira**-ban dokumentálom, a folyamatokat pedig **BPMN 2.0** és **UML** ábrákkal tervezem.

## 🛠 Tech Stack
- **Orchestration:** Apache Airflow
- **Containerization:** Docker, Kubernetes (GKE)
- **Data Processing:** Python, PySpark (Google Cloud Dataproc)
- **Cloud Platform:** Google Cloud Platform (GCP)
- **Storage & Warehouse:** Google Cloud Storage (Data Lake), BigQuery (DWH)
- **Data Modeling:** Data Vault 2.0, Apache Iceberg
- **Databases:** RDBMS (SQL) & NoSQL elvek
- **Documentation:** Jira, BPMN, UML

## 🏗 Architecture & Roadmap

A projekt négy fő fázisra oszlik:

### Phase 1: Ingestion & Local Automation
- Binance REST API integráció Pythonban.
- Helyi ütemezés és hibakezelés implementálása.
- BPMN folyamattervezés a logikai útvonalhoz.

### Phase 2: Cloud Infrastructure & Data Modeling
- Áttérés **Google Cloud Storage** alapú Data Lake-re.
- **Data Vault 2.0** modellezés (Hubs, Satellites, Links) alkalmazása a historikus adatok integritásáért.
- **RDBMS** metaadat-kezelés és **NoSQL** log-tárolás.

### Phase 3: Big Data Processing
- **PySpark** ETL folyamatok fejlesztése nagy tömegű adatok tisztítására.
- **Apache Iceberg** táblaformátum használata (ACID tranzakciók és Time Travel).
- Erőforrás-kezelés **Google Cloud Dataproc** használatával.

### Phase 4: Enterprise Analytics & Orchestration
- Adattárház (DWH) építés **BigQuery**-ben.
- Munkafolyamatok vezérlése **Apache Airflow** segítségével.
- A teljes rendszer skálázása **Kubernetes (GKE)** környezetbe.

## 📈 Data Vault 2.0 Model
A projekt során **Data Vault 2.0** módszertant használok, amely lehetővé teszi a rendkívül rugalmas és skálázható adattárolást. 
- **Hubs:** Üzleti kulcsok (pl. Coin symbols).
- **Satellites:** Időfüggő adatok (pl. Árfolyam, volumen).
- **Links:** Kapcsolatok (pl. Exchange-to-Pair relációk).

## 🚀 How to Run (Local Setup)
*(Feltöltés alatt - hamarosan Docker Compose állományokkal)*

## 📄 Documentation
A projekt részletes technikai tervei és Jira jegyei a `/docs` mappában találhatóak.
