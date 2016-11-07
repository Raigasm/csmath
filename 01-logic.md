# Logic

When people talk about logic they often mean propositional or
first-order predicate logic

- A logic usually has a well defined syntax, semantics and proof theory.
- The _syntax_ of a logic defines the syntactically acceptable objects of
the logic, or well-formed formulae.
- The _semantics_ of a logic associate each formula with a meaning.
- The _proof theory_ is concerned with manipulating formulae according
to certain rules

## Propositions
A proposition is a declarative sentence, or a statement, that is either
true (T) or false (F)

True or False are *Truth Values*

Propositions are often abbreviated using propositional variables, e.g.
p, q,r,s etc.

Propositions can be combined with other propositions to form *compound propositions*

### Connectives
|Symbol|   |description|alt|
|---|---|---|---|
| ∧ | and | conjunction | (& or .)
| ∨ | or | (inclusive) disjunction, inclusive-or | (\| or +)
| ⊕ | xor | (exclusive) disjunction, exclusive-or | |
| ¬ | not | negation, complement | (∼)
| ⇒ | if . . . then | implication, implies | (→)
| ⇔ | if and only if | equivalence, iff | (↔)

## Truth Tables

Example truth table:
![Truth Table](https://dl.dropbox.com/s/1274ddbbsttt19o/Introduction_to_Mathematical_Logic_2016-10-30_20-20-11.png?dl=0)


Alternative version of a truth table:

| p | &or; | q |
|---|---|---|
| T | T | T |
| T | T | F |
| F | T | T |
| F | F | F |


## Well Formed Formulae

The language of propositional logic is based on two components, an
`alphabet` and a `grammar`

### Alphabet

The alphabet of Propositional Logic consists of the following sets:

- a set of propositional variables `PROP = {p,q,r,s,...}`
- a set of propositional connectives {true, false, &not;, &and;, &or;, &oplus;, &rArr;, &hArr;}
- a set of punctuation symbols `{(,)}`


### The Grammar
Defines what constitutes a well-formed formua (wff)

- Each of the elements in `PROP` is a `wff`
- Each of true and false is a wff.
- If `p` and `q` are wffs, then so are (p &and; q), (p &and; q), (p &oplus; q), (p &rArr; q), (p &hArr; q).

This is an inductive definition.


## Determining Truth Tables for Compound Propositions

If:
- `p` (my breakfast is) toast
- `q` (my breakfast is) cereal
- `r` (my breakfast is juice)

The statement “my breakfast is either toast or cereal, and juice” may be
written in symbolic form as (p &or; q) &and; r


Truth tables may be used to show value assignments (also called
interpretations) of compound propositions

If we have 3 propositions, p, q,r, then we need 23 = 8 rows.

Next, construct a column for each connective, the most deeply nested
first.

## Brackets

Brackets ensure unique readability: ((p &and; q) &or; r) is different from (p &and; (q &or; r))

### Conventions

1. Omit outer brackets
2. Binding power (order) of connectives: ¬, ∧, ∨, ⊕, ⇒, ⇔
3. ¬ applies to smallest formula following it.
4. ∧ applies to smallest formula following it.
5. ∨ applies to smallest formula following it.
6. ⊕ applies to smallest formula following it.
7. ⇒ applies to smallest formula following it.
8. ⇔ applies to smallest formula following it.

## How do we read p ⇔ ¬q ∨ r ⇒ p?

(p ⇔ ((¬q) ∨ r) ⇒ p)
