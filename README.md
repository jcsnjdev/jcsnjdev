CREATE TABLE me (
    name      VARCHAR(255) NOT NULL,
    github    VARCHAR(255),
    age       INT(2) NOT NULL,
    country   VARCHAR(255),
    languages VARCHAR(255),
    doing     VARCHAR(255) CHECK (doing = "Studying" OR doing = "Sleeping"),
    
    PRIMARY KEY(github)
);
   
INSERT INTO me (name, github, age, country, languages, doing)
VALUES (
    	"Isaque", 
	"github.com/jcsnjdev",
        17, 
        "Brazil",
        "Python, Java, HTML, CSS, JavaScript,TypeScript and SQL",
	"Sleeping"
);
	
SELECT * 
FROM me
WHERE github = "github.com/jcsnjdev";
