## Prefer reversible decisions

### Summary

Prefer design decisions that will be easy to change. 

### Details

Many of the decisions you make while designing your code will eventually turn out to be wrong. 

If you can make your decisions reversible by containing their consequences and adding abstractions then this future change this will not matter.

As an example - if you introduce a third party library and reference it throughout your code you have made the cost of reversing the decision to use that library high. If you constrain it to a single location and create an interface for it, the cost of reversing the decision is low.

But don't forget KISS and YAGNI - if your abstractions complicate the design better to leave them out.
