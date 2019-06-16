# I highly recommend that you solve this yourself!

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

# Step 0: Go to bandcamp.com/jobs and find this header in the "jobs" network request
![stepZero][stepZero]

# Step 1: At that URL we see the raw content of an POST.
![stepOne][stepOne]

# Step 1a: Let's mock it up in Postman! Remember to send the content at the bottom in the POST body (not in screenshot).
![stepOneA][stepOneA]

# Step 2: At the returned URL, we find this image.
![stepTwo][stepTwo]

# Step 2a: I just ran it through an OCR tool and fixed up whatever was wrong. This gives us the next URL!
![stepTwoA][stepTwoA]

# Step 3: Now we have this cryptic matrix of characters with a message at the bottom...
![stepThree][stepThree]

> .e .m .a~.i .l,   .y .o~.u>.r,   .c~.o~.v .e .r,   .l+.e~.t .t .e~.r,   .a .n .d,   .r~.e+.s~.u .m~.e   .t+.o

# Step 3a: After I tried a few things, I realized that this was probably a CSS Selector. 

#### * dot (.) is a class selector
#### * tilde (~) is a general sibling combinator
#### * greater-than sign (>) is a child combinator
#### * addition symbol (+) is an adjacent sibling combinator

## So maybe this is a big ole CSS selector? Let's try it out in devtools and turn everything with that class red.

## That worked! I won't give anything away, but you can concat all the red letters to solve the puzzle!
![stepThreeA][stepThreeA]



[stepZero]: ./img/bandcamp/step0.png "bandcamp - Step Zero"
[stepOne]: ./img/bandcamp/step1.png "bandcamp - Step One"
[stepOneA]: ./img/bandcamp/step1a.png "bandcamp - Step One A"
[stepTwo]: ./img/bandcamp/step2.png "bandcamp - Step Two"
[stepTwoA]: ./img/bandcamp/step2a.png "bandcamp - Step Two A"
[stepThree]: ./img/bandcamp/step3.png "bandcamp - Step Three"
[stepThreeA]: ./img/bandcamp/step3a.png "bandcamp - Step Three A"