# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example        
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more).
        
> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.



# Observer
**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**

The Observer defines a one-to-many relationship so that when one object changes state, the others are notified and updated automatically. Some auctions demonstrate this pattern. Each bidder possesses a numbered paddle that is used to indicate a bid. The auctioneer starts the bidding, and "observes" when a paddle is raised to accept the bid. The acceptance of the bid changes the bid price which is broadcast to all of the bidders in the form of a new bid.
	
**how the pattern works, what the basic idea of the pattern is**

Define a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.
	
**what the main advantage and what the the main disadvantage is of using this pattern**

**advantage:**
•	It supports the principle of loose coupling between objects that interact with each other
•	It allows sending data to other objects effectively without any change in the Subject or Observer classes
•	Observers can be added/removed at any point in time

**disadvantage:**
•	The Observer interface has to be implemented by ConcreteObserver, which involves inheritance. There is no option for composition, as the Observer interface can be instantiated.
•	If not correctly implemented, the Observer can add complexity and lead to inadvertent performance issues.

**Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more).**

The observer design pattern – often abbreviated to observer pattern – is one of the most popular pattern templates for designing computer software. It provides a consistent way to define a one-to-one dependency between two or more objects in order to relay all changes made to a certain object as quickly and simply as possible. For this purpose, any objects that act as observer in this case can register with another object. The latter object – referred to as a subject – informs the registered observers as soon as it has changed.

As mentioned at the start, the observer pattern in one of the GoF patterns published in “Design Patterns: Elements of Reusable Object-Oriented Software” in 1994. The more than 20 pattern solutions described for software design continue to play an important role in designing and developing computer applications.

**Function of the observer pattern:**
The observer design pattern works with two types of actors: On the one side, there is the subject – i.e. the object whose status is to be observed over the long term. On the other side, there are the observing objects (observers) that want to be informed about any changes to the subject.

Without using the observer pattern, the observing objects would have to ask the subject to provide status updates at regular intervals; each individual request would be associated with corresponding computing time as well as the necessary hardware resources. The fundamental idea behind the observer pattern is to centralize the task of informing within the subject. It, therefore, maintains a list which the observers can register to join. In the event of a change, the subject informs the registered observers – one after the other – without them having to take action themselves. If an automatic status update is no longer desired for a certain, observing object, it can simply be removed from the list.



# State
**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**

The State pattern allows an object to change its behavior when its internal state changes. This pattern can be observed in a vending machine. Vending machines have states based on the inventory, amount of currency deposited, the ability to make change, the item selected, etc. When currency is deposited and a selection is made, a vending machine will either deliver a product and no change, deliver a product and change, deliver no product due to insufficient currency on deposit, or deliver no product due to inventory depletion.

**how the pattern works, what the basic idea of the pattern is**
	Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.
	
**what the main advantage and what the the main disadvantage is of using this pattern**

**advantage:**

To begin with, a major advantage of the state model is its capability to minimize conditional complexity. It eliminates the need for it and switches statements on objects with different behavioral requirements, unique to different state transitions. So, representing an object’s state using a finite state machine diagram simplifies the conversion of the diagram into a state design model’s types & methods.

**disadvantage:**

A developer needs to write a large amount of code for the state schema. Depending on the number of different defined state transition methods and possible object states, you can write numerous methods. Thus, for N states with M transition methods, the total number of methods required will be (N+1)*M.
An insurance policy with 5 different states and 5 methods for each (ignoring ListValidOperations method) requires 25 methods in total. The policy context type must also define the 5 state transition methods, increasing total methods required to 30.

**Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more).**

