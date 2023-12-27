ALGORITHM "Checkpoint ALGO Chapter 1"
VAR
 
 //Instructions
//1- The length of the sentence (the number of characters).
//2- The number of words in the sentence (assuming that the words are separated by a single space).
//3- The number of vowels in the sentence.
 
    sentence = "GoMyCode"
    length: INTEGER
    wordCount: INTEGER
    vowelCount: INTEGER
    vowels = "aeiouAEIOU"
    i: INTEGER
    sum: INTEGER

BEGIN
    // 1. Calculate the length of the sentence
    
    length := 0
   
    FOR i FROM 0 TO sentence.length - 1
       
    length := length + 1
    END_FOR

    // 2. Calculate the number of words in the sentence
    wordCount := 1  // Assuming the sentence is non-empty
    
    FOR i FROM 0 TO sentence.length - 1
      
        IF sentence[i] = ' ' AND sentence[i + 1] != ' '
           
            wordCount := wordCount + 1
    

    // 3. Calculate the number of vowels in the sentence
   
    vowelCount := 0
    
    FOR i FROM 0 TO sentence.length - 1
        
        IF vowels.contains(sentence[i])
            
            vowelCount := vowelCount + 1
   

    // 4. Calculate the sum from 1 to the length of the sentence
    sum := 0
    
    FOR i FROM 1 TO length
       
        sum := sum + i
   
    END_FOR

    WRITE("Length of the sentence is length")
    WRITE("Number of words in the sentence is wordCount")
    WRITE("Number of vowels in the sentence is vowelCount")
    WRITE("Sum from 1 to the length of the sentence is sum")
END
