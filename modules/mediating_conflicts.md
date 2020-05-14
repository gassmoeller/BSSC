# Mediating between users

#### Questions:
- Can I avoid conflicts in my community? 
- How to handle conflicts between members of the community?
- What to do if my community contains bad actors?

#### Objectives:
- Learn about the types of conflicts in scientific software projects
- Understand strategies for handling conflicts during development
- Develop policies for supporting good and containing bad behavior

## The nature of conflicts

- Conflicts are unavoidable. families, companies, countries, software projects all experience conflicts. In particular: Conflicts are disagreements for how something should be handled. In software projects there can be different causes of conflicts, some of the most common conflicts:
  - conflicts about implementations
  - conflicts about policies
  - conflicts about personalities

## The implementation conflict

One of the most common conflicts in software development (in particular in science) is an argument about a particular software implementation. In particular if the implementation is made by someone else than you, there are multiple questions that should be carefully considered:
  - What are the benefits of a particular solution?
  - What is the cost of implementation (consider time, but also effects on rest of project)?
  - Are there multiple sides to this solution (does it help some, but hurt others)? 
  - Who has the time and commitment to do the implementation?

*Exercise:* Consider a typical example conflict in a scientific software project: A new Developer A suggests to implement a relatively simple Algorithm 1 that would address a given problem he encountered while working on the project. Senior Developer B is convinced that a complicated Algorithm 2 would be better suited and she suggests to A to implement this better algorithm. Developer A does not have the skills or time to implement Algorithm 2. How should the project continue? List at least 2 potentially good solutions and 2 potentially bad solutions. Click on the headings below to see some common answers.

<details><summary><b>Potentially good solutions</b></summary>

<ul> 
<li>Go the easy route and let Developer A develop Algorithm 1 and include it in
the project (optionally replacing it by Algorithm 2 from Developer B later).
While not ideal (e.g. in terms of performance, elegance, or code structure) it
solves the immediate problem, improves the project, and lets Developer A feel
useful. Of course if the structure of the algorithm is the problem it creates a
maintenance burden for the maintainers of the project that needs to be handled
by either Developer A (who developed the algorithm) or Developer B (who is
responsible for merging it).</li>
<li>If Developer B has the time and commitment to either implement Algorithm 2
herself, or to sufficiently help Developer A to implement Algorithm 2 then
going for Algorithm 2 is a better long-term solution than the previous one
(given the benefits outweigh the cost of implement Algorithm 1).</li>
<li>The maintainers agree that Algorithm 1 should not be merged into the
project, and offer Developer A to either implement Algorithm 2 with their help,
or to keep Algorithm 1 as an outside plugin (TODO ref). If done kindly and in
accordance with the policies of the project in this case it is Developer A's
responsibility to accept this decision. Not all additions to a project can be
merged (see <a href="https://github.blog/2016-03-15-kindly-closing-pull-requests/">Kindly Closing Pull
Requests</a>).</li>
</ul> 
</details>

<details><summary><b>Potentially bad solutions</b></summary>

<ul> 
<li>Algorithm 1 gets merged without sufficient discussion (e.g. by careless
Developer C). Potential problems are that Developer B feels that her opinion
was ignored, and there might a maintenance burden on the project for this
algorithms.</li>
<li>Algorithm 1 gets rejected without sufficient discussion or the offer of
alternatives. Developar A feels that his commitment and offer to help was not
appreciated and feels less likely to contribute again.</li>
<li>Developer B rejects Algorithm 1 and insists on Algorithm 2, but does not
have the commitment or time to develop it herself, or help Developer A
sufficiently to implement it. This is one of the most common and dangerous
cases! It can easily lead to a situation where neither Algorithm 1 nor
Algorithm 2 makes it into the project **and** Developer A feels like his
commitment was wasted. While Developer A has the responsibility to respect
comments and make reasonable changes due to comments from Developer B he has no
responsibility to rewrite the whole code. Therefore if Developer B insists on
Algorithm 2 she has to make clear how much help Developer A can expect from
her. Then Developer A has to respect that decision and assess for himself if he
is able and willing to rewrite the algorithm.</li>
</ul> 
</details>

#### A note about community: 
The above exampe was formulated as a direct conflict between Developer A and B for simplicity. In practice there can be many more participants. Adding more participants can be a help, or a problem, depending on the commitment and abilities of the participants. Nothing is worse than having a half-commited maintainer who only read through part of the discussion throw in a: "But I think Algorithm 1 is bad." into a nuanced discussion without fully understanding the consequences or the weight of the arguments brought up so far.

#### A note about seniority:
Implementation conflicts are prone to be solved by following the opinion of the most experienced developer. This can be both a correct step (because senior developers often have a broader perspective on the issue) and a problem (younger developers are often closer to the problem at hand and are more flexible). 

## The policy conflict



## The personality conflict


#### Resources:

- [Kindly Closing Pull Requests](https://github.blog/2016-03-15-kindly-closing-pull-requests/)

This module is under construction, please come back later.

Want to help? We welcome contributions. Please see our [contributing guidelines](https://github.com/gassmoeller/BSSC/blob/master/CONTRIBUTING.md#contributing-to-bssc).

