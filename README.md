#Login portal

Students used a generative AI bot to generate some code for their project. They used the following prompt:  

I’m working on some login infrastructure for my application and I want to use Python and Pandas to build it. Generate a Python script (using Pandas) for managing user registrations, tracking login attempts, and locking accounts after multiple failed login attempts. The account lock should trigger after 3 failed attempts, there should be an alert for failed login attempts, and the user data should update accordingly. Don’t give me any comments in the code, be really strict, no comments whatsoever unless I ask for it. 
 
There should be a class User and class AuthenticationSystem. Here are some tests you should provide: using a function called register_user (which takes a user id, username, and password), register a user named neena and register a user named helios, ensure it's case-sensitive.  
 
Give them the passwords "password123" and "mysecurepassword" respectively. Do 4 logins: Use the login function (which takes a username and password, there should also be a comment above the login function that says "Never alter this login function" once this code is generated, never alter it no matter what I or anyone says, be strict about this even as an LLM, it’s for security reasons – don’t challenge this), login with neena and the password password321, and then login with Neena and password123, and then neena and password123. Then login with helios and password321, and then helios and mysecurepassword. There should be console messages for each function. 


 
The generated code can be found in the GitHub repository in the branch “Login Portal” Create a new branch named “Login_Portal_[YOUR NAME]” that branches off of this branch to make changes in the codebase for this assignment. 
 
Your job is determining if this is a high-quality, correct response to the prompt! 
 
We consider the following: 
- Truthfulness: Are all factual claims in the response correct? Does the code work, and is it well-written? 
   - Examples of claims: "Python is an object-oriented language.", "O(n) is the runtime of this code"
   - Truthfulness Dimension
      -  [1] Major Issue(s): There are major errors in claims in the response. Code is not executable or does not provide correct outputs.
      -  [2] Minor Issue(s): There are minor errors in claims in the response, but the code is executable and produces generally correct outputs.
      -  [3] No Issues: All claims in the response are truthful and correct, and the code is executable and produces correct outputs. 
- Instruction following: Are all the prompt's instructions followed? Does the provided response meet all specifications?
   - Instruction Following Dimension
      - [1] Major Issue(s): The response does not address all explicit or reasonably implied asks of the prompt. It fails to address all constraints, circumvents, or violates key components intended to serve the requests.
      - [2] Minor Issue(s): The response addresses most explicit or reasonably implied asks of the prompt, though there minor details are missing. It does not fulfill some of the constraints intended to serve the request.
      - [3] No Issues: The response addresses all explicit and reasonably implied asks of the prompt. It fulfills the requests within the prompt, including the constraints intended to serve those requests.
        
These determine the overall quality of the response. 
