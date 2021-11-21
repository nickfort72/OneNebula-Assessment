# OneNebula-Assessment

<h1>Database Challenges</h1>

<h2>Question 1</h2>

The two main areas for improvement are partial dependencies and redundancy.
The ERD appears to be in 1NF as all rows are unique and atomic, however there are partial dependencies. A potential solution could be to Create Cellphone detail and Employee address tables to remove partial dependencies so the ERD is now in 2NF. I then removed vendor from employee and Event Detail as there was redundancy and put it in the new Cellphone Detail table where it was best suited. Tables are now also in 3NF as there are no transitive dependencies. Redundancy is avoided to a large extent and the tables now follow normalization rules.

 ![ERD Diagram](https://github.com/nickfort72/OneNebula-Assessment/blob/main/ERD%20diagram.png)


<h2>Question 2</h2>

SELECT Movies.Genre, SUM(Tickets.TicketID) AS 'Tickets sold in December'   
FROM Tickets  
INNER JOIN Movies  
ON Tickets.MovieID = Movies.MovieID  
WHERE Tickets.Month='December' AND Tickets.Year='2020'  
GROUP BY Genre;  

<h1>Back-end Code Challenges</h1>
<h2>Question 1</h2>

    static void PrintIfMultiple(string input)
    {
	if (input.Length % 2 == 0 && input.Length % 4 == 0)
        {
            Console.WriteLine("Stack Overflow!");
        }
        else if ( input.Length % 2 == 0)
        {
            Console.WriteLine(" Stack");
        }
        else if ( input.Length % 4 == 0)
        {
            Console.WriteLine("Overflow");
        }
	}


<h2>Question 2</h2>

        public class Animal
    {
        public string Eat()
        {
            return "Yummy";
        }

        public virtual string MakeNoise()
        {
            return "Durrr";
        }
    }
    
    class Horse : Animal
    {
       
       public override string MakeNoise()
        {
            return "Neigh";
        }
    }
    
    class Sheep : Animal
    {
     
       public override string MakeNoise()
        {
            return "Baaah";
        }
    }



<h1>Front end code challenges</h1>
 <h2>question 1</h2>
1)
The firstDiv would be red, the secondDiv would be orange. 

2) 
<script>
var firstDiv = document.getElementById("firstDiv");
firstDiv.style.backgroundColor = 'pink';
</script>

3)
 <script>
var secondDiv = document.getElementById("secondDiv");
secondDiv.classList.add("yellow-card");
</script>

<h2>Question 2</h2>

1 )
The function will be parsed correctly because javascript supports method overriding. The value of x will remain the same.
<br>
2 )
You could use a different variable name and make it equal to x, for example: var legalValue = x; or you could use: this.x = x; and colsole.log(this); 
You could also log the value of x at the end of the function to prevent confusion if the value of x changes after logging.  

<h1>Personality test</h1> 

![Personality test](https://github.com/nickfort72/OneNebula-Assessment/blob/main/Personality%20assessment.png)




 






