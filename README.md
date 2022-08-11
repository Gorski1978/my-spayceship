# my-spayceship
function my_spaceship(letter_string) {
    var x=0;
    var y=0;
    var direction = "up";
    
    for(var index = 0; index < letter_string.length; index ++) {
        if(letter_string[index]== "A") {
        if(direction == "up") {
           y--;
        }
        else if(direction == "down") {
           y++;
        }		
        else if(direction == "left") {
           x--;	
        }	
        else if(direction == "right") {
           x++;	
        }		
      }	
           
      else if(letter_string[index]== "L") {
        if(direction == "up") {
            direction = "left";
      }
      else if(direction == "left") {
         direction = "down";
      }		
      else if(direction == "down") {
         direction = "right";	
      }	
      else if(direction == "right") {
        direction = "up";	
        }		
      }	
           
           
      else if(letter_string[index]== "R") {
        if(direction == "up") {
            direction = "right";
      }
      else if(direction == "right") {
         direction = "down";
      }		
      else if(direction == "down") {
         direction = "left";	
      }	
      else if(direction == "left") {
        direction = "up";	
        }		
      }			
    }
      return `{x: ${x}, y: ${y}, direction: '${direction}'}`;	 
           
   }
