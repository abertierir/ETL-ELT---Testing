# What is Data Warehouse?

---

Getting data from diferent heterogenous sources.

It is a process of transforming data into information and making it available to users in a timely manner to make a difference.

> Source systems which supply data to a staging area, what is basically a one to one copy of source data that you receive from your different source systems. This integrated data what we call a data warehouse.
> 

### Datamart

A subset from our data warehouse for each and end users. 

![Captura de Pantalla 2023-01-31 a la(s) 1.33.56 p.m..png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/150ec942-71a5-4f38-8931-0f8977b5d548/Captura_de_Pantalla_2023-01-31_a_la(s)_1.33.56_p.m..png)

# What is ETL/ELT?

---

## ETL

Data Warehouses environments

![Captura de Pantalla 2023-01-31 a la(s) 1.59.24 p.m..png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/febad498-ab86-45a3-bb86-3a6cecd0d612/Captura_de_Pantalla_2023-01-31_a_la(s)_1.59.24_p.m..png)

## ELT

![Captura de Pantalla 2023-01-31 a la(s) 2.02.50 p.m..png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/93faaa8a-43ab-4709-ab30-a25ca0aec373/Captura_de_Pantalla_2023-01-31_a_la(s)_2.02.50_p.m..png)

Load the data without touch it.

# Data Quality

---

We want to know if our data ramains consistent and valid throughout your whole life cycle.

There are different categories of testing:

- Transformation’s mapping: We look at different transformations from our source to our target system and validate each of those transformations.
- Source Target Testing: Data lineage or integrity testing
- Schema testing

# Data Categories and Classifications

---

1. Information → Data serving a certain context and purpose
2. Transactions Data → Describers an event or transaction. Events that occur at a certain time.
3. Master Data → Data that is consitently shared across an entire organization **Ex**: Customer information
4. Reference Data → Structures and standarizes the master data into a pre-defined list of values. **Ex:** Codes defined by and ISO or Currency codes.
5. Metadata → Provides context and information abour the master data. Data that describes your data.

Por ejemplo para Master Data es necesario verificar la consistencia.

Por ejemplo para Reference Data is important to have an unified list throughout all the sources.

# Data Quality Rules and Dimensions

---

DAMA-DMBOK Framework - Data Quality Dimensions:

1. Completeness: The dataset is complete. We don’t want to see any data missing. **Ex** Name is mandatory
2. Uniqueness
3. Timeliness
4. Validity: Data is still valid at certain point of time. **Ex** Age falls between 0 and 120 **or** E-mail address need s to be in the right format
5. Accuracy: Is it still up to date today?
6. Consistency. **Ex** Currency needs to be in the list of allowed ISO values **or** Genders needs to be M or F
    
    ![Captura de Pantalla 2023-01-31 a la(s) 5.51.38 p.m..png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1f0e3fff-45af-4d3d-b246-7ca138bbe291/Captura_de_Pantalla_2023-01-31_a_la(s)_5.51.38_p.m..png)
    

→ Data Quality Rules Repository

→ Data Quality Components

1. **Data Profiling -** Metadata, Descriptive Methods (Count, Mean, Max, Min), Validation Levels (Scheme, entity, attribute)
2. **Data Quality Analysis**  / Validation
3. **Data Cleansing** / Matching - Eliminate errors, duplicates, incisistencies
4. **Data Quality Monitoring** - Reporting and Monitoring

### Data Quality Tools

- Informatica Data Quality - IDQ
- Talent Open Studio for Data Quality
- IBM - InfoSphere Quality Stage and Information Analyzer
- SAS Data Quality
- Oracle
- Others

# Data Requirements and Test Design

---

### Archivos

- Orders
- Products
- Returns
- Region Managers
- Customers

**Data Marts:** DM_CUSTOMER_REGIONAL_SALES
