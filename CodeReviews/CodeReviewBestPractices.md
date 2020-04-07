# Best Practices 

 <p align="center">
<img src="Images/cleancodereview.png" alt="Defects Density vs Lines of code per hour" width="400">
</p>

### Communicate clear goals and expectations of reviewers  
 To ensure that reviews are consistent Reviewers should be given a checklist of what to look for during a review. The checklist should contain the following criteria of what they should be looking for as reviewers :

 #### Design 
* When looking at the design of the code the reviewer should be asking themselves these questions :

 * Does the change belong in the code base or in a library.
 * How well does it integrate with the rest of the system.
 * Do interactions of different pieces of code make sense.

 #### Functionality 
 * Does the code carry out it's intended function?
 * Is it not only good for the users but also other developers who will have to work with this area of the code base in the future?
 * What are the edge cases?, Think like a user and make sure there are no bugs or concurrency issues.

 #### Structure
* Are there any structural errors in the code such as dead code, algorithm bugs etc.? (this task can usually be automated)

 #### Style 
* Is the code consistent with the style guide? 
 This is important for maintaining consistency and helps with readability across the project.

 #### Complexity 
* Is the code more complex than it need to be?
* Has functionality that isn't presently needed been added to the system?

 #### Tests 
* Are the current tests in place appropriate?
* Do unit or end-to-end tests need to be updated/created?


### Speed of a code review and how long should be spent on a given review
 
 #### 60-90 minutes max per review
 A code reviewer should take the time to carry out a slow and thorough review. However this should take no more than 60-90 minutes according to study's carried out by IBM and others it has been shown that after 60 minutes reviewers tend to get tired and stop finding additional defects/issues with the code.

 <p align="center">
<img src="Images/image002.gif" alt="Defects Density vs Lines of code per hour" width="400">
</p>

 #### Fast Responses
 Individual responses to code reviews should come as fast as possible but not at the expense of the quality of the review as this could result in the code being below standard. As the whole review process may take time it is important that the developer whose code is being reviewed receives a response asap from the individual reviewers. This eases the frustration that the developer may get from "slow" code reviews. You obviously don't have to carry out the full review straight away if you are too busy to so but responding when you can and letting the developer know you will get to it later when you have time or recommending another reviewer who may be able to respond more quickly. Will let the developer know that the reviewers aren't ignoring them.

### How to write comments for a code review
  
  #### Balance giving directions
  Remember it is not your job to provide a full solution for the developer make sure there is a balance between simply pointing out problems for them to fix and giving explicit instructions on how to fix. This is especially important when mentoring new developers as denying them the opportunity to learn from their mistakes can hinder their development.

  #### Give credit when credit is due
  Make sure not to just critique your colleagues if you found how they've written their code or how they implemented a functionality to be good/clever let them know. This again can be good for mentoring newer developers as it offers encouragement, they can learn from what they did right and not just hear about what they've done wrong.

  #### Encourage Developers to simplify code
  Asking a developer to simplify their code or to add comments to it will usually result in them rewriting their code more clearly making it easier to understand. Which far more beneficial for the health of the project as it will be easier later on if someone else is working with that part of the code base rather than just explaining it to you within the confines of the review.


### Handling Developer push back on a review
A Developer will not always agree with your review which can lead to unnecessary conflict if not handled correctly there are key things you need to take into account to handle this correctly which are :

 #### Consider whether they are correct
  * Does their argument for not making your suggested changes make sense?
  * Does it make sense from code health perspective?
  If that is the case let them know you agree and drop your review.

 #### Ask for further explanation  
 If you are not convinced by their argument for not accepting your review ask them for further explanation on why they believe they're correct. If you are still not convinced by their argument believing your suggestion and the additional work involved is worth the benefit it will provide to the project continue to push for the developer to accept your review and make the changes.

### Include Everyone in the review process
Including everyone in the review process no matter what their seniority as a developer is helps promote collaboration and relationships between the team members enhancing the team's cohesion. Also as mentioned before in code review benefits knowing that every other team member will be looking at your code will encourage you to make sure code is of a higher standard when it's being put up for a review.


 ## Quick Links
  * [Home Page](../README.md)
  * [Code Review Home Page](CodeReviews.md)
  * [Bad Practices](CRBP.md)
  



#### References

[11 proven practices for more effective, efficient peer code review, Jason Cohen](https://www.ibm.com/developerworks/rational/library/11-proven-practices-for-peer-review/)

[Google's Engineering Practices documentation](https://google.github.io/eng-practices/review/)

[9 Best Practices for Code Review, Richard Bellairs](https://www.perforce.com/blog/qac/9-best-practices-for-code-review)
