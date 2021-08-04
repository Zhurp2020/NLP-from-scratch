# The Handbook of Linguistics
## Part 3 Core Fields
### 14 Formal Semantics
#### 1 Introduction
+ understand  linguistic meaning by constructing precise mathematical models of the principles that speakers use to define those relations between expressions in a natural language and the world which support meaningful discourse.
+ explain our capacity to assign interpretations to an unbounded number of grammatical sentences
#### 2 Meanings and Denotations
+ if it is possible to construct a successful account of the meaning of declarative sentences used to make statements, then this account can be generalized to nondeclarative sentences
+ Frege, first-order logic.
  + individual terms 
  + predicates  
  + connectives 
  + quantifiers
  + for each logical type an expression of that type can take a certain sort of entity as its denotation
    + the function $f$ which a one-place predicate denotes can be represented as the set of objects in $f$’s domain for which $f$ yields the value true
    + Two-place connectives denote functions from pairs of truth-values to a truth-value
    + quantifiers are second-order functions, in quantified sentences, a term that corresponds to a property of a set applies to a predicate 
  + the sense of an expression is the principle for determining its denotation
+ Carnap
  + the extension of an expression $E$ is the entity which it denotes
  + intensions as functions from possible worlds to denotations
  + a possible world can be thought of as the result of specifying the properties and relations which hold for the objects of a domain in a way that defines a complete state of affairs for the entities of the domain
  + intension of an expression takes a possible world as an argument and yields the extension of the expression in that world as its value
+ compositionality: the meaning of any well-formed phrase in a language be a function of the meanings of its syntactic components
  + the extension of a phrase is a function of the extensions of its parts
  + the intension of a phrase is a function of the intensions of its parts
+ Tarski, true-in-L
  + . The definition proceeds stepwise first to elementary sentences constructed from individual terms and predicates, next to compound sentences formed by applying truth functions to other sentences, and finally to quantified sentences. 
  + For each sentence S of type T in language L, it specifies the truth conditions for S in terms of the relations which must hold among the denotations of the constituents of S. 
  + generates appropriate truth conditions for the full set of well-formed sentences of L. 
+ Davidson
  + associate the sentences of a natural language with first-order logical forms to which a Tarskian truth definition can apply
+ Montague, type system, categorical grammar
  + a small number of syntactic categories are taken as basic
  + All other categories are functions from input expressions of a certain category to output expressions of a given category
  + homomorphism: a mapping that assigns a single semantic type to each syntactic category
+ Difference:
  + modification
    + Davidson: 
      + predicates which apply to individuals
      + assigns a semantic type to modifiers which is quite remote from their syntactic role
      + does not extend to modifiers that produce expressions whose meanings cannot be taken as the conjunction of two predicate extensions
    + Montague: 
      + Syntactically, modifiers are functions from predicates to predicates, and semantically they are functions from predicate intensions to predicate extensions
      + does not express the fact that when an extensional modifier applies to a predicate, it does produce a predicate whose interpretation is equivalent to the conjunction of two predicates
  + NP
    + Davidson:  taking proper names to be terms that denote individuals and appear as arguments of predicates, while analyzing quantified NPs as operators which bind variables in argument positions. 
    + Montague: 
      + functions which take VPs as arguments to produce sentences: 
      + generalized quantifiers: a set of sets of individuals
      + transitive verbs stand for relations between individuals and sets of sets (GQs) rather than relations between individuals. 
#### 3 Dynamic Semantics: Beyond Static Sentence Meanings
+ discourse representation theory (DRT): an indefinite NP is treated not as a quantified NP, but as an expression which introduces a discourse referent that satisfies the content of the indefinite description
+ dynamic binding: retains the traditional view of indefinites as existentially quantified NPs. In addition to the classical logical connectives and quantifiers it introduces dynamic counterpart operators whose scopes can extend beyond single clauses
+  E-type pronoun: locates the mechanism for dynamic anaphora in the interpretation of the pronoun which takes a quantified NP as its antecedent, functions like a pointer to a description that refers back to an entity in the set that is determined by its quantified NP antecedent.
#### 4 Meanings and Situations: Beyond Possible Worlds 
+ A situation is a smaller and more fine-grained object than an entire world
+ Cooper
  +  distinguish between the resource situation in which the restriction set of a GQ is fixed and the situation in which the entire sentence containing the GQ expression is evaluated.
  +  quantificational situation must be distinguished from the individual situations i in which the property expressed by the VP applies to each of the elements of the restriction set
#### 5  Underspecified Representations: Beyond Compositionality
+ noncompositional: allowing the mapping from syntax to semantics to be a relation which assigns more than one meaning to an expression under a single syntactic representation
+ quantified NPs can either be taken as GQs in situ or interpreted through the device of quantifier storage
+ sentences containing scope-taking expressions are assigned schematic semantic representations in which the scopes of these terms are left unspecified.
#### 6 Conclusion