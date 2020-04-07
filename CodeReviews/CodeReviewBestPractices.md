# Best Practices

### Communicate clear goals and expectations of reviewers  
 To ensure that reviews are consistent Reviewers should be given a checklist of what to look for during a review. The checklist should contain the following critrea of what they should be looking for as reviewers :

 #### Design 
* When looking at the design of the code the reviewer should be asking themselves these questions :

 * Does the change belong in the code base or in a library.
 * How well does it intergrate with the rest of the system.
 * Do interactions of different pieces of code make sense.

 #### Functionality 
 * Does the code carry out it's intended function?
 * Is it not only good for the users but also other developers who will have to work with this area of the code base in the future?
 * What are the edge cases?, Think like a user and make sure there are no bugs or concurrency issues.


 #### Structure
* Are there any structural errors in the code such as dead code, algorithm bugs etc.? (this task can usually be automated)


 #### Style 
* Is the code consistent with the style guide? 
 This is important for maintaining consistency and helps with readibility across the project.

 #### Complexity 
* Is the code more complex than it need to be?
* Has functionality that isn't presently needed been added to the system?

 #### Tests 
* Are the current tests in place appropriate?
* Do unit or end-to-end tests need to be updated/created?