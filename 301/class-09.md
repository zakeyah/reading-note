## Read: 09 - Refactoring

# What is functional programming?

Functional programming is a programming style of building the structure and elements of computer programs, it treats computation as the evaluation of mathematical function and avoids changing-state and mutable data.

Pure functions are the first concept in functional programming. It returns the results and is also referred a `deterministic`

The benefits of pure functions are that makes code easier to test.

# What is immutability?

Immutability is a state that cannot change after it is created.

# When should you consider software refactoring?
The best time to consider refactoring is before adding any updates or new features to existing code. Going back and cleaning up the current code before adding in new programming will not only improve the quality of the product itself, it will make it easier for future developers to build on the original code.

# When should you consider software refactoring?
The best time to consider refactoring is before adding any updates or new features to existing code. Going back and cleaning up the current code before adding in new programming will not only improve the quality of the product itself, it will make it easier for future developers to build on the original code.
# Techniques
One of the most widely used techniques for code refactoring is the red/green process used in Agile test-driven development. Applying the Red-Green-Refactor method, developers break refactoring down into three distinct steps:
- Stop and consider what needs to be developed. 
- Get the development to pass basic testing. 
- Implement improvements. 
# Refactoring by Abstraction
Branching by abstraction is a method used primarily when there is a large amount of refactoring to be done. Abstraction involves class inheritances, hierarchy, and extraction. The goal of abstraction is to reduce unnecessary duplications in software code.
# Composing Method
Composing involves streamlining the code in order to reduce duplications. This is done through various processes, including extraction and inline methods.
-    Extraction involves breaking down the code into smaller chunks in order to find and "extract" fragmentation. The fragmented code is then moved to a separate method and replaced with a call to this new method. In addition to the method, extraction can involve class, interface, and local variables as well.
-    Inline refactoring is a way to reduce the number of unnecessary methods while simplifying the code. By finding all calls to the method and replacing them with the content of the method, the method can then be deleted.
