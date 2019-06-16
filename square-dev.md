# I highly recommend that you solve this yourself! 
#  Curl squ.re/hunt to get started!

### The contest is over (and the final POST will say so), so I feel comfortable posting the whole solution.

### Move along if you've finished the challenge and want to compare approaches or if you just dislike the satisfaction of solving something yourself!

## .
## .
## .
## .
## .
## .
## .
## .
## .
## .
## .
## .
## .
## .

# Step 0: For the love - help the dev!!!
![stepZero][stepZero]

# Step 1: curl in your terminal to receive and (reluctantly) copy the next curl command
![stepOne][stepOne]

# Step 2: Seems like a dead-end, but they have given us a lot of clues...
![stepTwo][stepTwo]

# Step 3: What does the binary from step 1 say in ASCII? ...Ah!
![stepThree][stepThree]

# Step 4: Let's HS256 decode the authorization header from step 2.
![stepFour][stepFour]

## Looks like we got an informative payload back!
## Let's try those routes in Postman!

# Step 5: /labor
## PS. Remember back to step 2 where it told us to use "https://squavenger-hunt.glitch.me" as the main URL and reminded us to include the Authorization header in all requests.
![stepFive][stepFive]

## "Inside your token you must closely inspect, combine the keys for a path that you must use to connect"

# Step 6: /employees
![stepSix][stepSix]

## "On this new path you cannot use GET, using a POST might be your best bet.

# Step 7
![stepSeven][stepSeven]

## "Hidden amongst these clues is the path, that surely lead to a prize to hath. 🏆

# Step 8
![stepEight][stepEight]

## "If you're [sic] are stumped and simply don't know what to do, just ask on the platform with the bird that is blue.

## Thanks, but no thanks! I think there's enough information here!

# Step 9: The /labor route said to inspect the keys of our token, which you can see in step 4, vertically from top to bottom spell out "l e g o"

## With that information, let's make a request to that route. Remember that the /employee route said to use a POST request! 📬
![stepNine][stepNine]

## "Congrats! You figured it out and saved me! Here's your final token:"

# Step 10: go to http://square.com/go/hunt and enter your token in!
![stepTen][stepTen]

# Who saved whom <3

[stepZero]: ./img/square/step0.png "Square Dev - Step Zero"
[stepOne]: ./img/square/step1.png "Square Dev - Step One"
[stepTwo]: ./img/square/step2.png "Square Dev - Step Two"
[stepThree]: ./img/square/step3.png "Square Dev - Step Three"
[stepFour]: ./img/square/step4.png "Square Dev - Step Four"
[stepFive]: ./img/square/step5.png "Square Dev - Step Five"
[stepSix]: ./img/square/step6.png "Square Dev - Step Six"
[stepSeven]: ./img/square/step7.png "Square Dev - Step Seven"
[stepEight]: ./img/square/step8.png "Square Dev - Step Eight"
[stepNine]: ./img/square/step9.png "Square Dev - Step Nine"
[stepTen]: ./img/square/step10.png "Square Dev - Step Ten"