# Welcome-to-the-Bookstore
The purpose of this project was to practice basic Javascript.  I use JS to calculate the price of purchasing books, using some simple input, output, arithmetic, and conditional statements.
<!DOCTYPE html>
<!-- 
Author: Jennifer Otiono & Rose Marie Flores
Date: 3/11/17
Purpose: Assignment 3
Filename: 
-->

<html lang="en">
  

  <head>
    <meta charset="utf-8">      
    <title>Basic JavaScript</title>
  </head>
  
  <body>
    <h1>Welcome to the Bookstore</h1>
    <p id="results"></p>
    
     <p>
      <a href="http://validator.w3.org/check?uri=referer">
       <img
         src="http://cs.wellesley.edu/~cs110/Icons/valid-html5v2.png"
         alt="Valid HTML 5"
         title="Valid HTML 5"  
         height="31" width="88">
      </a>
    </p>  
    
    <script>
    
      var num_books = parseInt(prompt("How Many Books Do You Want To Order?",100));	
      	 if (num_books < 25 ) {
      	 var book_price =num_books*50;
      	    
      	  }
      	  else  {
      		 var book_price = num_books*40; 
      	  }
      		
      	 var tax = (book_price * 0.07);
         var order_wtax= (book_price + tax);
     	 var ship_fee;
     	 
     	 
         if (order_wtax < parseInt(500))
      	 { 
      	  ship_fee = parseInt(25); 
      	 }
      		else {
      		ship_fee = parseInt(0);			
      	 }
         var tot_order=order_wtax + ship_fee;
        
          alert("RECEIPT\nNumber of Books: "+num_books+".\nBook Price: $"
          +book_price.toFixed(2)+".\nTax: $ "+tax.toFixed(2)+".\nShipping Fee: $"
          +ship_fee.toFixed(2)+".\nTotal Cost: $"+tot_order.toFixed(2));
          
        
          console.log(book_price.toFixed(2));
          console.log(tax.toFixed(2));
          console.log(order_wtax.toFixed(2));
          console.log(ship_fee.toFixed(2));
          console.log(tot_order.toFixed(2));
      
    </script>
  
   
  </body>
</html>
  
