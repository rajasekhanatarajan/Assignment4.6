# Assignment4.6

#A recent national study showed that approximately 44.7% of college students have used Wikipedia as a source in at least one of their term papers. Let X equal the number of students in a random sample of size n = 31 who have used Wikipedia as a source.

#Perform the below functions

#a. Find the probability that X is equal to 17

#b. Find the probability that X is at most 13

#c. Find the probability that X is bigger than 11.

#d. Find the probability that X is at least 15.

#e. Find the probability that X is between 16 and 19, inclusive

#Ans 1a.

dbinom(17, size = 31, prob = θ.447) [1] 0.07532248

#Ans 1b.

pbinom(13, size = 31, prob = θ.447) [1] 0.451357

#Ans 1c.

pbinom(11, size = 31, prob = θ.447, lower.tail = FALSE) [1] 0.8020339

#Ans 1d.

pbinom(14, size = 31, prob = θ.447, lower.tail = FALSE) [1] 0.406024

#Ans 1e.

sum(dbinom(16:19, size = 31, prob = θ.447)) [1] 0.2544758 diff(pbinom(c(19, 15), size = 31, prob = θ.447, lower.tail = FALSE)) [1] 0.2544758
