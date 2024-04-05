# Lawz-Tables

# DB Design 
![Screenshot 2024-03-13 231111](https://github.com/fairouzAlateeq/Lawz-Tables/assets/37877628/d383c823-a8f3-4531-98db-569f6106915f)


# DB SQL
CREATE DATABASE LAWZ;

CREATE TABLE PLANT (
PLANTID PK INT,
PLANTNAME FK VARCHAR(200),
SUNLIGHT BOOL,
/*  No. of days the plant needs water per week */
IRR-NO CHAR(7),
/* No. of ML of water the plant needs per day*/
ML VARCHAR(500),
); 

CREATE TABLE USER (
USERID PK INT,
PASSWORD VARCHAR(200),
DISPLAYNAME VARCHAR(200),
);

INSERT INTO plant (plantID, plantname, sunlight, irrigation, ML) 
VALUES
    (21, 'Cucumber', 1, 7, 200),
    (22, 'Tomatoe', 0, 5, 150),
    (23, 'Corn', 1, 3, 100),
    (24, 'Carrots', 0, 6, 180),
    (25, 'Mint', 1, 4, 120);
ALTER TABLE USER 
ADD USERNAME UNIQUE VARCHAR(200);

ALTER TABLE user
ADD CONSTRAINT fk_plantname
FOREIGN KEY (plantname)
REFERENCES plant(plantname);

## Info code examples:
INSERT INTO user (userID, password, display_name, username)
VALUES 
    (11, 'password1', 'John Doe', 'john_doe'),
    (12, 'password2', 'Jane Smith', 'jane_smith'),
    (13, 'password3', 'Alice Johnson', 'alice_johnson'),
    (14, 'password4', 'Bob Brown', 'bob_brown'),
    (15, 'password5', 'Emily Davis', 'emily_davis');

UPDATE user 
SET plantID = 24
SET PlantName.user = Plantname.plant
WHERE userID = 11;

## 🤝 Contributing
This code contributes in the making of our app LAWZ which encourages sustainability.

### Clone the repo
All pull requests should be submitted to the main branch.
