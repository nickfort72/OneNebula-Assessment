# OneNebula-Assessment

Database Challenges

Question 1

The two main areas for improvement are partial dependencies and redundancy.
The ERD appears to be in 1NF as all rows are unique and atomic, however there are partial dependencies. A potential solution could be to Create Cellphone detail and Employee address tables to remove partial dependencies so the ERD is now in 2NF. I then removed vendor from employee and Event Detail as there was redundancy and put it in the new Cellphone Detail table where it was best suited. Tables are now also in 3NF as there are no transitive dependencies. Redundancy is avoided to a large extent and the tables now follow normalization rules.

 



 


Back-end Code Challenges
Question 1

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
 
Question 2

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
 
Front end code challenges
 question 1
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

Question 2

1 )
The function will be parsed correctly because javascript supports method overriding. The value of x will remain the same.
2 )
You could use a different variable name and make it equal to x, for example: var legalValue = x; or you could use: this.x = x; and colsole.log(this); 
You could also log the value of x at the end of the function to prevent confusion if the value of x changes after logging.  




 






