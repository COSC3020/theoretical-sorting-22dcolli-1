# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

## Plagarism Statement

All exercises must contain the following statement:
“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”

## Note
I did not complete this excersise last semester, so I am attempting this completely from scratch. I did discuss this partially with Lily Brongo and then referenced Ishita Patel's repository from last semester to confirm my logic before submission.

## Answer

I think that the best way to verify the claim is to test the algorithm as extensively as possible. Under the assumption that this is a black-box implementation, in order to test we would simply feed the algorithm many data sets of differing values and sizes in order to try an observe the algorithms behavior. The size of the varying data sets would not matter, as long as there are many possible sets tested, which should include small sets,large sets, and of course many unique cases and edge cases. We include the edge cases to more accuratley observe the algorithm's behavior in them.The algorithm claims to be able to sort in $\Theta(n)$ time, which means that with testing, we should be able to observe a linear increase in sorting time with the size of the data set. In essence, there should be direct coralation between data set size and sort time, with shorter data sets having a proportionaly shorter sort time and larger data sets having a proportionaly longer sort time which to reiterate is just a linear increase in time for the size. With enough testing, eventually we should be able to see the algorithms behavior clearly. There is an issue also however, which comes from the statement that the algorithm is based on the comparisons of two elements at a time. Using slide 45 from the class lectures, theoretically we can see that the complexity of any comparison based sorting algorithm can't be better than $\Theta(nlogn)$, which is contradicted by this algorithm's claim of $\Theta(n)$.
