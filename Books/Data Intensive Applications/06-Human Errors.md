The end-user doesn't use the product the way it was supposed to be used and this the most common human error that can happen other than the user doesn't know how to use the product.

There are different ways to design a system in such a way that it becomes resilient to human errors such as:

- Only give access to the required parts of the applications to the general user.
- The admin or super-user can access other options on their own if they know how to.
- Don't put the options where the user can cause the most error around the parts that are most sensitive and can cause failures.
- Testing is important, unit-test each and every component and then integration testing when the system has been built. 
- Allow the user to undo any actions that he makes and if it's an important decision ask them twice before actually performing the operation.
- Monitoring, metrics, and telemetry should be added to keep track of the features most used by users and how they use it.
- Add tutorials and popups guiding the user what the correct way of using each option is.