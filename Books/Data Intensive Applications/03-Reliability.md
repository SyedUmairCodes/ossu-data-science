Reliable software, performs the required function, can handle most common user mistakes, and has safe-guards built-in to make sure that no unwanted access can be granted.

Faults appear when the application doesn't work as expected. When designing systems for data-intensive applications we must build the system in such a way that it's resilient to most common faults that may come up when the system is in use.

Any system cannot be 100% fault proof, we cannot design such a system that doesn't have any kind of fault in it since we don't know how the user is going to interact with the system. 

> Faults can also be caused by natural disasters and other things that aren't in our control.

A failure is different from a fault. A failure is caused by multiple components of the system failing to work properly which leads to the whole system stopping and a fault is simply one component that isn't working or has stopped working.

Engineers deliberately induce faults in their systems while they're being tested to make them more fault-proof and find any other faults that can happen during the lifetime of the application.

> Fault prevention is better than fault tolerance.

