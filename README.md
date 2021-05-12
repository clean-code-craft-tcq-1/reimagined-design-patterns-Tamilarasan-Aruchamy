# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**1. Observer**
          The Observer defines a one-to-many relationship so that when one object changes state, the others are notified and updated automatically. Some auctions demonstrate this pattern. Each bidder possesses a numbered paddle that is used to indicate a bid. The auctioneer starts the bidding, and "observes" when a paddle is raised to accept the bid. The acceptance of the bid changes the bid price which is broadcast to all of the bidders in the form of a new bid.
          
- how the pattern works, what the basic idea of the pattern is
- **1. Observer**
          One-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.
 
- what the main advantage and what the the main disadvantage is of using this pattern
- **1. Observer**
- **Advantage:**
-1. It supports the principle of loose coupling between objects that interact with each other.
-2. It allows sending data to other objects effectively without any change in the Subject or Observer classes.
-3. Observers can be added/removed at any point in time.
-         
-**Disadvantage:**
-1. The Observer interface has to be implemented by ConcreteObserver, which involves inheritance. There is no option for composition, as the Observer interface                  can be instantiated.
-2. If not correctly implemented, the Observer can add complexity and lead to inadvertent performance issues.

- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more).
**1. Observer**
          
> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.
