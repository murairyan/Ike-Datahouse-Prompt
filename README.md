# Ike-Datahouse-Prompt
My answer to the prompt given by Ike Datahouse.

// Building the Solution:
I decided to use C++ as my choice of language for this prompt. The main issue, however, of using C++ was that I could not create and use an array that would accept both int and string values as suggested in the JSON input and output from the prompt. So, as a countermeasure to go around this issue I decided to use a 2-D array. Reason for this is because I know that there are three team members and three applicants, and each of these "objects" contain 3 int values (originally four, but for simplicity I decided to do three). Therefore a 2-D array with three rows and columns works accordingly to the input given. The biggest flaw to this design was that it would be difficult to assess who was who according to the score, but since this is almost like pseudo code I just designed it as a developer would in C++. I would imagine that there would be another array to store the names of the team members and applicants to correspond to their respective scores. After delving into working around the string and int array issue, I decided to go with several functions that would help dictate the scoring of the team members and applicants. At first I tried to understand how the scoring system worked based on the input and output given to me by the prompt, but to no avail. So, I went for a simple solution of adding the values of all these scores of the team and then taking the average of it. That's what one of the function does, the other is to just gather the scores of the applicants one by one, so it is just a summation of each row. Although it was not directed, I chose to use functions for the prompt because to my knowledge, functions allow for more simplicity for the main function as well as flexibility in the event that something does not work, it makes it easier to deduce what the leading cause of the problem may be. Inside the main function, I had also created an empty array, this array would take and hold the returned array from the function, which is the sums of the scores of each applicant. This now filled array would then be used to store the scores of the applicants by taking the sums of each applicant and dividing that score with the average score of the team members. I found this to be the most logical solution to scoring the applicants as it would show compatibility. I was also thinking of adding the scores of each respective attribute and then averaging that to compare with the score of the applicants, but I did not want to go overboard with the function. I just wanted to show a general concept and explain the overall purpose of it. The output was also in JSON as told by the prompt. Even though, the array that is storing the scores of the applicants is only for int values, here we assume that the array has both the names and scores as shown in the JSON output. At the end, I returned 0 to tell the program that it is done executing and can stop, although this step is not necessary, I just have a habit of doing it (I believe it is neither a good or bad practice). And since I am technically coding in C++, the program already has “return 0” implemented within it, but I wanted to just type it out. 

// Potential Issues:
Now I do understand that I used Github to create this program and that it is mostly comprised of almost pseudo code as I never got the chance to really test this approach, so there could be some parameter or even data type errors. As mentioned earlier, there is no way of having an array hold both string and int values, so I believe that my approach is a severe limitation of what the input and output is, so just creating an assumption that the user knows what name belongs to what row in the 2-D array. Another issue that could be a problem is the data types. I do know that the output values should be double or float as it is in the decimal values, so I did make the empty array that holds the applicants score as a double datatype, but the other variables all have int. This will most likely output an error as int and double data types may not have a conversion type and therefore the main function will return nothing but an error. The parameters of the functions are also very inflexible as I made it like “int arr[3][3]”, but in the event that the input is more or less than that then the function will be unable to work. A potential solution to this would be to make the parameters the same as the constant int values for “rows” and “columns” as I did for the main program. Lastly, I made it so that the average score of the "team" will be greater than the overall score of each "applicant", but in the event that condition is not met (keeping the compatability score between [0,1]), a different scoring method would be better like the one mentioned beforehand. The biggest struggle I had making this was how to get the names to correspond to their respective scores for both “team” and “applicants”, the only solution I could think of would be to create two arrays that would store the scores and the names and then output each name with their respective scores, but I found the 2-D array solution more fun to do, so I stuck with it. 

// Overall:
As there are most likely plenty of errors within this code, I did the best I could to properly utilize the input and output given to me by the prompt. I really enjoyed the overall process and thinking outside the box to work around the JSON sample to utilize C++. What I show in the code is how I usually go about coding, I try to space out lines of code the best I can so it is easy to follow along, provide inline comments to elaborate into detail for myself and others, and the use of functions to create a simpler main program. Hope this is easy to follow along and please let me know if there are more details that need to be further elaborated on. I did this within the 3 hour time frame given, hence the potential errors, but hope this reflects well on my analytical skills and experience. 
