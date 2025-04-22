DROP database multilevel_company;
create DATABASE TASK_2;
USE TASK_2;

CREATE TABLE student (
    username VARCHAR(50) PRIMARY KEY
);

describe student;
CREATE TABLE assignment (
    shortname VARCHAR(50) PRIMARY KEY,
    due_date DATE NOT NULL,
    url VARCHAR(255)
);

describe assignment;

CREATE TABLE submission (
    username VARCHAR(50),
    shortname VARCHAR(50),
    version INT,
    submit_date DATE NOT NULL,
    data TEXT,
    PRIMARY KEY (username, shortname, version),
    FOREIGN KEY (username) REFERENCES student(username) ON DELETE CASCADE,
    FOREIGN KEY (shortname) REFERENCES assignment(shortname) ON DELETE CASCADE
);
describe submission;

show databases;
