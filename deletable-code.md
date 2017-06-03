# Notes and misc
Adopting a "write deletable" code means code will start to seem less precious.
Might also guard against over-engineering, or the urge to write a
"once-and-for-all" solution.
It acknowledges that information and/or business demands change often, and
sometimes unpredictably.
Like with composition over inheritance, the benefits of coding this way maybe
affect 20% of the code but 80% of 

Making code easy to read & reason about should be a primary goal when writing
code. Removing unnecessary/old code reduces the cognitive load a developer has
to digest when encountering a new (or forgotten) body of code.


## further reading:
    * [Life-changing magic of deleting code](https://medium.engineering/the-life-changing-magic-of-deleting-code-be5cb3ffb391)
    Take time after a release or completing a project to remove unused code and
    clean up. Use the `// TODO: ` comment and tag someone's name there. Remove
    it after the release.
    * [Deleting Code](https://nedbatchelder.com/text/deleting-code.html)
    Dos and Don'ts on deleting code.
    dont commit commented out code; or at least leave a comment as to WHY the code is commented out (instead of being removed)
    leave a comment block in place of where a chunk of code was removed.
    Explain in a comment why it was removed and include a place to find it.
    * [Write code that is easy to delete, not to
    extend](http://programmingisterrible.com/post/139222674273/write-code-that-is-easy-to-delete-not-easy-to)
    Koan-like, several ideas that are good springboards toward fleshing out
    and applying to one's own daily work.
    * [On the Criteria to be used for Decomposing Systems into
    Modules](https://www.cs.umd.edu/class/spring2003/cmsc838p/Design/criteria.pdf)
    OG blueprint for modular system. Instead of dividing program into modules along lines of
    process flow (ie Process A ==> Process B ==> Process C = Module A ==> B ==>
    C) consider how the processes share/exchange information. Focus on
    decomposing along the
    input/output of a module, hiding the internal functionality.

## Toward a definition of "deletable code"
what makes code deletable?
1. minimal interface
    * fewer arguments of a defined type (probably?)
    * clearly defined & predictable return
2. minimal dependencies/dependents?
3. modular/contained/portable (see above)

* whats the relationship between practicing code reuse and writing
  deletable code?

