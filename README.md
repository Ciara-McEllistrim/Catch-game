//The aim of this simple JavaScript game is to catch the dog that is running around.

<html>
    <meta charset="UTF-8"> 
<head>
<style>
tr { width: 300px; height: 100px }
td { width: 100px; height: 100px }
img { width: 100px; height: 100px }
</style>
<script> 
  
   var interval = setInterval(moveImgRandomly, 300); //refreshes the function every 200 milliseconds 
    function moveImgRandomly(){
         
    var image_ape = document.getElementById("mole"); //set image as a variable
//    image_ape.parentNode.removeChild(image_ape);
      
        var choosenCell = Math.floor(Math.random() * 10); // generate number between 1 and 9
                       
                            
        //the append childs set the contents of the cell to the image if their table cell id was what was the result of math.random
        
        if (choosenCell==1){
            document.getElementById("1").appendChild(image_ape); 
                
        }
            else
          
        if (choosenCell==2){
               document.getElementById("2").appendChild(image_ape);            
                
        }
            else
          if (choosenCell==3){
          document.getElementById("3").appendChild(image_ape);
                            
        }
            else
          if (choosenCell==4){
             document.getElementById("4").appendChild(image_ape);
                }
            else
          if (choosenCell==5){
            document.getElementById("5").appendChild(image_ape);
                            
        }
            else if (choosenCell==6){
           document.getElementById("6").appendChild(image_ape);
                    }
                else if (choosenCell==7){
         document.getElementById("7").appendChild(image_ape);
                                
        }
            else if (choosenCell==8){
             document.getElementById("8").appendChild(image_ape);
                                
        }
            else if (choosenCell==9){
            document.getElementById("9").appendChild(image_ape);
                
                
        }
    
        
        
    }
    
    function message(){  //if the image is clicked on this message appears.
        alert("Caught");
    }
   
    
    </script>
</head>
<body>
<table>
 <tr>
<td id="1"></td>
<td id="2"></td>
<td id="3"><img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSAhBCKD5nk9v_gTtXRch18Ej7kX6FdyEonalep-qGEcB9s6pTJ"id="mole" onclick="message()">
     </td>
 </tr>
 <tr>
<td id="4"></td>
<td id="5"></td>
<td id="6"></td>
 </tr>
 <tr>
<td id="7"></td>
<td id="8"></td>
<td id="9"></td>
 </tr>
</table>
</body>
</html>
