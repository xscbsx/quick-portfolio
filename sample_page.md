# My projects
## Hospital database management

**Project description:** 
In this project, you can have a wise view of the hospital management.For example, you can track the workers who had contact with patients who were later diagnosed with COVID. With this tool, It's easy to track the people who were at a risk and also prevent the infection.

### 1. Creation of the entity-relationship diagram (ERD)


<img src="images/Hospital.vpd.png?raw=true"/>

### Business scenario description
1. Doctors diagnose any number of Conditions affecting a Patient, and a Diagnosis may apply to many Patients;

2. The involved hospital records the following information: location, doctor and patient's information;

3. Doctors may order and perform any number of  Treatments for a Patient, or may not perform any Treatment.

4. A Treatment  may be performed on any number of Patients, and a Patient may have Treatments performed by any number of Physicians.

_SQL code:_

```
CREATE TABLE DOCTOR(doc_id integer PRIMARY KEY, Name text, Specialization text not null);
CREATE TABLE PATIENT(card_id integer PRIMARY KEY,Name text, Diagnosis text not null,Date_CheckIn datetime not null,Date_CheckOut);
CREATE TABLE HOSPITAL(hosp_id text PRIMARY KEY,Location text)
CREATE TABLE COVID_TEST(test_id integer PRIMARY KEY, doc_id FOREIGN KEY, card_id FOREIGN KEY,Test_date datetime, Test_Time datetime,Result varchar(8)
```
<!-- 
### 2. Assess assumptions on which statistical inference will be based

```javascript
if (isAwesome){
  return true
}
```

### 3. Support the selection of appropriate statistical tools and techniques

<img src="images/dummy_thumbnail.jpg?raw=true"/>

### 4. Provide a basis for further data collection through surveys or experiments

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. -->

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
