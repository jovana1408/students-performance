# Analiza uspeha učenika (Students Performance Analytics)

Ovaj projekat se bavi analizom i OLAP modeliranjem uspeha učenika na osnovu demografskih i socio-ekonomskih faktora. Projekat obuhvata rad sa Kaggle skupom podataka, njegovo skladištenje i upite u SQL Serveru (SSMS), kao i kreiranje višekratnih kocke/tabularnih modela u SQL Server Analysis Services (SSAS).

---

## 📊 O skupu podataka (Dataset)

Izvorni skup podataka preuzet je sa Kaggle platforme (**Students Performance in Exams**) i sadrži sledeće atribute:

- **Gender:** Pol učenika (*female / male*)
- **Race/Ethnicity:** Etnika/Grupa (*Group A, B, C, D, E*)
- **Parental Level of Education:** Stepen obrazovanja roditelja
- **Lunch:** Tip školske ishrane (*standard / free or reduced*)
- **Test Preparation Course:** Status pripremnog kursa (*none / completed*)
- **Math Score / Reading Score / Writing Score:** Rezultati na testovima (0–100)

---

## 🛠️ Korišćene tehnologije i alati

- **Kaggle** – Izvor skupa podataka i inicijalna istraživačka analiza (EDA)
- **Microsoft SQL Server Management Studio (SSMS)** – Upravljanje bazom podataka, čišćenje podataka i SQL upiti
- **SQL Server Analysis Services (SSAS)** – Izrada analitičkih modela, dimenzija, mera (Measures) i OLAP kocki za višedimenzionalnu analizu
- **MDX / DAX** – Analitički upiti za generisanje izveštaja i agregacija

---

## 🏗️ Arhitektura projekta i koraci

1. **Preuzimanje i priprema podataka (Kaggle):**
   - Preuzimanje `.csv` fajla sa Kaggle-a i analiza strukture podataka.
   
2. **Relaciona baza podataka (SSMS):**
   - Importovanje sirovih podataka u SQL Server bazu.
   - Normalizacija/priprema tabela i definisanje relacija (dimenzije i tabela činjenica / Star Schema).

3. **Višedimenzionalno modeliranje (SSAS):**
   - Definisanje dimenzija (npr. *DimStudent*, *DimCourse*, *DimDemographics*).
   - Kreiranje tabele činjenica (*FactStudentPerformance*) sa merama poput prosečnih bodova i prolaznosti.
   - Izgradnja OLAP kocke


---

## 📈 Primeri analiza i mera

Neke od definisanih mera i analiza u projektu uključuju:
- **Prosečni bodovi po predmetima:** Poređenje rezultata u zavisnosti od pripremnog kursa.
- **Uticaj obrazovanja roditelja:** Analiza korelacije između nivoa obrazovanja roditelja i uspeha učenika.
- **Distribucija uspeha po tipu ishrane:** Analiza socijalnih faktora na krajnji uspeh.

---

## 👩‍💻 Autor

- **Jovana** – [@jovana1408](https://github.com/jovana1408)
