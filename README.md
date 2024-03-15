# Lawz-Tables

# DB Design 
![Screenshot 2024-03-13 231111](https://github.com/fairouzAlateeq/Lawz-Tables/assets/37877628/d383c823-a8f3-4531-98db-569f6106915f)


# DB SQL
CREATE DATABASE LAWZ;

CREATE TABLE PLANT (
PLANTID PK INT,
PLANTNAME FK VARCHAR(200),
SUNLIGHT BOOL,
IRR-NO CHAR(7),
ML VARCHAR(500),
); 

CREATE TABLE USER (
USERID PK INT,
PASSWORD VARCHAR(200),
DISPLAYNAME VARCHAR(200),
);

ALTER TABLE USER 
ADD USERNAME UNIQUE VARCHAR(200);

## 🤝 Contributing
This code contributes in the making of our app LAWZ which encourages sustainability.

### Clone the repo
All pull requests should be submitted to the main branch.
