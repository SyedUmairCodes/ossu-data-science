We all use some type of third-party libraries or frameworks in our code to make our job easier but the developers who make those third-party APIs strive to deliver a product for wide adaptability and that their product can work in almost all types of environments.

While the users of these services want the APIs to be tailored to their specific use-case and these thought processes of both parties can cause a whole lot of problems rather than solving them.

A third-party framework may have a lot of built-in methods and functions that are quite useful but if you only need a few of these functions you would argue that importing the whole framework would just add bloat to your application but coding 
those functions from scratch would take too much time.

Third-party code helps us get more functionality delivered in less time but if we came across any errors we would need to go through the entire documentation of the library or framework that we are using to find to out if the bug is in our code or theirs.

A better approach to prevent this is to not use a new third-party API directly in production but to test it out first using small and simple tests. This way you could focus only on the parts of the third-party API that you actually need.

These tests can be handy to test out newer versions of the third party API to check if there are any breaking changes because the third-party API developers will focus on their needs and might introduce changes that could potentially break your application.

Good software designs accommodate change without huge investments and rework. When we use code that is out of our control, special care must be taken to protect our investment and make sure future change is not too costly.