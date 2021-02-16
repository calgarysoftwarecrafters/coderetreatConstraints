

### Summary:

Design the bigger pieces first, mock what's underneath


### Details:

Start by agreeing on a design. Pick a top-level component from the design and start there, then mock necessary dependencies. With every finished component, you move to the previously mocked collaborators and start with TDD again there, creating actual implementations.


### Example:

TDD the the sandwich, mock everything else

TDD the bread...
