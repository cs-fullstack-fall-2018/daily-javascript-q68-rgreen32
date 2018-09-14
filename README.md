# daily-javascript-q68

You have the following code: 
```html
<script> 
      var count = 0; 

      function main() { 
           try { 
                --count; 
                walkThrough(); 
           } 
           catch (e) { 
                count++; 
           } 
           finally { 
                count++; 
           } 
      } 

      function walkThrough() { 
           try { 
                var obj = {} 
                if (obj) 
                     count++; 
                else { 
                     let test = "This is a testing string"; 
                     if (test.indexOf('is') === 2) 
                          count++; 
                     else { 
                          throw new Error("Error"); 
                     } 
                } 
           } 
           catch (e) { 
                count--; 
           } 
           finally { 
                count++ 
           } 
      } 

      main(); 
      console.log(`Count: ${count}`); 
</script> 
```
What will be the value of count?

Choose the correct answer

1) 1
2) 2
3) 3
4) 4  X
