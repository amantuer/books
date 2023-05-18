Jack D. Hidary

Quantum Computing: An Applied Approach Second Edition

Quantum Computing: An Applied Approach

Jack D. Hidary

Quantum Computing: An Applied Approach Second Edition

Jack D. Hidary Palo Alto, CA, USA

ISBN 978-3-030-83273-5 ISBN 978-3-030-83274-2 (eBook)
https://doi.org/10.1007/978-3-030-83274-2 1st edition: © Jack D. Hidary
under exclusive license to Springer Nature Switzerland AG 2019 2nd
edition: © The Editor(s) (if applicable) and The Author(s), under
exclusive license to Springer Nature Switzerland AG 2021 This work is
subject to copyright. All rights are solely and exclusively licensed by
the Publisher, whether the whole or part of the material is concerned,
specifically the rights of translation, reprinting, reuse of
illustrations, recitation, broadcasting, reproduction on microfilms or
in any other physical way, and transmission or information storage and
retrieval, electronic adaptation, computer software, or by similar or
dissimilar methodology now known or hereafter developed. The use of
general descriptive names, registered names, trademarks, service marks,
etc. in this publication does not imply, even in the absence of a
specific statement, that such names are exempt from the relevant
protective laws and regulations and therefore free for general use. The
publisher, the authors, and the editors are safe to assume that the
advice and information in this book are believed to be true and accurate
at the date of publication. Neither the publisher nor the authors or the
editors give a warranty, expressed or implied, with respect to the
material contained herein or for any errors or omissions that may have
been made. The publisher remains neutral with regard to jurisdictional
claims in published maps and institutional affiliations. This Springer
imprint is published by the registered company Springer Nature
Switzerland AG The registered company address is: Gewerbestrasse 11,
6330 Cham, Switzerland

Contents Preface to the Second Edition

xiii

Preface to the First Edition xv Acknowledgements xix Navigating this
Book

I

xxi

Foundations

1 Superposition, Entanglement and Reversibility 4

1.1 Superposition and Entanglement 1.2 The Born Rule

5

1.3 Schrödinger’s Equation

8

1.4 The Physics of Computation

11

2 A Brief History of Quantum Computing

15

2.1 Early Developments and Algorithms 2.2 Shor and Grover

3

16

18

2.3 Defining a Quantum Computer 3 Qubits, Operators and Measurement 3.1
Quantum Operators

19 23

28

Unary Operators 28 Binary Operators 32 Ternary Operators 34 v

vi

Contents

36

3.2 Comparison with Classical Gates 3.3 Universality of Quantum
Operators

3.4 Gottesman-Knill and Solovay-Kitaev 3.5 The Bloch Sphere

37

38

3.6 The Measurement Postulate

39

41

3.7 Computation-in-Place 4 Complexity Theory

37

43

4.1 Problems vs. Algorithms 4.2 Time Complexity 4.3 Complexity Classes

43

44 46

4.4 Quantum Computing and the Church-Turing Thesis

II

Hardware and Applications

5 Building a Quantum Computer

53

5.1 Assessing a Quantum Computer 5.2 Neutral Atoms 5.3 NMR

54

55

56

5.4 NV Center-in-Diamond 5.5 Photonics 5.6 Spin Qubits

57

58 60

5.7 Superconducting Qubits

61

5.8 Topological Quantum Computation 5.9 Trapped Ion 5.10 Summary

64 65

63

49

Contents

6 Development Libraries for Quantum Computer Programming 6.1 Quantum
Computers and QC Simulators 6.2 Cirq

68

70

6.3 Qiskit

72

6.4 Forest

75 77

6.5 Quantum Development Kit 80

6.6 Dev Libraries Summary

Using the Libraries 81 Other Development Libraries 81

82

6.7 Additional Quantum Programs Bell States 82 Gates with Parameters 84

7 Teleportation, Superdense Coding and Bell’s Inequality 7.1 Quantum
Teleportation 7.2 Superdense Coding

87

87

90

7.3 Code for Quantum Teleportation and Superdense Communication 91 7.4
Bell Inequality Test

94

8 The Canon: Code Walkthroughs

101

8.1 The Deutsch-Jozsa Algorithm

103

8.2 The Bernstein-Vazirani Algorithm 8.3 Simon’s Problem

113

8.4 Quantum Fourier Transform 8.5 Shor’s Algorithm

110

114

117

RSA Cryptography 117 The Period of a Function 119 Period of a Function
as an Input to a Factorization Algorithm 121

vii

67

viii

Contents

8.6 Grover’s Search Algorithm

135

Grover’s Algorithm in Qiskit 140 3-Qubit Grover’s Algo 141

9 Quantum Computing Methods

143 143

9.1 Variational Quantum Eigensolver VQE with Noise 148 More
Sophisticated Ansatzes 150

9.2 Quantum Chemistry

151

9.3 Quantum Approximate Optimization Algorithm (QAOA)

156

Example Implementation of QAOA 159

9.4 Machine Learning on Quantum Processors 9.5 Quantum Phase Estimation

167

174

Implemention of QPE 177

9.6 Solving Linear Systems

180

Description of the HHL Algorithm 182 Example Implementation of the HHL
Algorithm 184

9.7 Quantum Random Number Generator 9.8 Quantum Walks

192

194

Implementation of a Quantum Walk 196

9.9 Unification Framework for Quantum Algorithms (QSVT) 203

9.10 Dequantization 9.11 Summary

205

10 Applications and Quantum Supremacy 10.1 Applications

207

207

Quantum Simulation and Chemistry 207 Sampling from Probability
Distributions 208 Linear Algebra Speedup with Quantum Computers 208
Optimization 208 Tensor Networks 208

202

Contents

10.2 Quantum Supremacy

ix

208

Random Circuit Sampling 209 Other Problems for Demonstrating Quantum
Supremacy 214 Quantum Advantage and Beyond Classical Computation 214

10.3 Quantum Error Correction

215

Context and Importance 215 Important Preliminaries 216 Motivating
Example: The Repetition Code 217 The Stabilizer Formalism 219

10.4 Doing Physics with Quantum Computers

III

224

Toolkit

11 Mathematical Tools for Quantum Computing I 11.1 Introduction and
Self-Test 11.2 Linear Algebra

227

227

229

Vectors 229 Introduction to Dirac Notation 230 Basic Vector Operations
231 The Norm of a Vector 234 The Dot Product 237

11.3 The Complex Numbers and the Inner Product

240

Complex Numbers 240 The Inner Product as a Refinement of the Dot Product
242 The Polar Coordinate Representation of a Complex Number 246

11.4 A First Look at Matrices

254

Basic Matrix Operations 254 The Identity Matrix 261 Transpose, Conjugate
and Trace 263 Matrix Exponentiation 270

11.5 The Outer Product and the Tensor Product

271

The Outer Product as a Way of Building Matrices 271

x

Contents

The Tensor Product 273

11.6 Set Theory

276

The Basics of Set Theory 276 The Cartesian Product 279 Relations and
Functions 280 Important Properties of Functions 286

11.7 The Definition of a Linear Transformation

291 293

11.8 How to Build a Vector Space From Scratch Groups 294 Rings 300
Fields 305 The Definition of a Vector Space 308 Subspaces 311

11.9 Span, Linear Independence, Bases and Dimension

313

Span 313 Linear Independence 315 Bases and Dimension 317 Orthonormal
Bases 320

12 Mathematical Tools for Quantum Computing II 12.1 Linear
Transformations as Matrices

323

323

328

12.2 Matrices as Operators

An Introduction to the Determinant 328 The Geometry of the Determinant
332 Matrix Inversion 334

12.3 Eigenvectors and Eigenvalues

341

Change of Basis 344

12.4 Further Investigation of Inner Products

346

The Kronecker Delta Function as an Inner Product 349

12.5 Hermitian Operators

350

Why We Can’t Measure with Complex Numbers 350 Hermitian Operators Have
Real Eigenvalues 352

Contents

353

12.6 Unitary operators

12.7 The Direct Sum and the Tensor Product

354

The Direct Sum 354 The Tensor Product 357

12.8 Hilbert Space

360

Metrics, Cauchy Sequences and Completeness 360 An Axiomatic Definition
of the Inner Product 364 The Definition of Hilbert Space 365

12.9 The Qubit as a Hilbert Space

366

13 Mathematical Tools for Quantum Computing III 13.1 Boolean Functions

371

13.2 Logarithms and Exponentials 13.3 Euler’s Formula 14 Dirac Notation

377

14.1 Vectors

377

14.2 Vector operations

371

372

374

378

Inner and Outer Products 378

14.3 Tensor Products

379

14.4 Notation for PDF and Expectation Value

380

15 Table of Quantum Operators and Core Circuits

383

Works Cited Index

421

387

xi

Preface to the Second Edition

The field of quantum computing has grown rapidly in the two years since
the first publication of this book. The first page of the book went
through five printings in its first year which mirrors the growing
number of individuals ramping up in the sector. I would like to thank
all the faculty, students and other readers from so many countries who
provided helpful input for this new edition. Our world, of course,
changed in many other ways as well since the publication of the first
edition. The global pandemic impacted all areas of society and will
probably transform how we work together for years to come. While
in-person meetings were halted, quantum tech researchers and engineers
found ways to continue their collaborations online. In the last year,
many countries have announced new or expanded quantum tech initiatives.
These programs are injecting significant resources into the quantum tech
ecosystem. We have also noted the rise in private investment in the
sector – both in quantum computing hardware companies as well as various
applications startups. All this activity has sharply increased the
demand for individuals who are trained in quantum computing as well as
those with additional hands-on experience in coding for these machines.
This, in turn, has led many universities to launch and expand their
quantum information science curricular programs and for corporations to
start quantum tech training programs for their teams. With this new
edition I continue to strive towards the goal of making quantum
computing more accessible to a wider range of individuals. This is a
technical book, but one that I hope opens the door to quantum computing
for individuals who would like to get a rigorous grasp of how to make
these novel computing devices work and which kinds of problems we should
focus on when using these platforms.

xiii

xiv

Preface to the Second Edition

This second edition contains several updates and expanded areas of
coverage, including:  Expanded coverage of quantum machine learning and
quantum error correction  Expanded chapter on principles of quantum
mechanics  Updated chapter on quantum hardware  Coverage of the QSVT
framework  New chapter on Dirac notation  This new edition also
corrects known typos from the first edition (thankfully, there were not
many). If any new typos have entered into the second edition please make
a note of them in the online site.  All the code throughout has been
re-tested and updated for the current versions of the various quantum
computing frameworks and libraries. All of these additions and updates
are based on requests from readers. The companion online site for the
book is also updated and I recommend that readers check the site for a
range of resources including updated downloadable code, problem sets and
further instructional material.1 I look forward to all the creativity
that will emerge in this field and the positive impact the discipline
will have on so many important fields. Please continue to send in your
input via the online site. Jack D. Hidary September 2021

1 http://www.github.com/jackhidary/quantumcomputingbook

Preface to the First Edition

We are entering a new era of computation that will catalyze discoveries
in science and technology. Novel computing platforms will probe the
fundamental laws of our universe and aid in solving hard problems that
affect all of us. Machine learning programs powered by specialized chips
are already yielding breakthrough after breakthrough. In this book we
will explore quantum computing – an emerging platform that is
fundamentally different than the way we compute with current digital
platforms. To be sure, we are years away from scaled quantum computers.
Yet, we now know that such systems are possible; with advances in
engineering we are likely to see real impact. Quantum computing is part
of the larger field of quantum information sciences (QIS). All three
branches of QIS – computation, communication and sensing – are advancing
at rapid rates and a discovery in one area can spur progress in another.
Quantum communication leverages the unusual properties of quantum
systems to transmit information in a manner that no eavesdropper can
read. This field is becoming increasingly critical as quantum computing
drives us to a post-quantum cryptography regime. We will cover quantum
teleportation and superdense coding, which are both quantum-specific
protocols, in chapter 7. Quantum sensing is a robust field of research
which uses quantum devices to move beyond classical limits in sensing
magnetic and other fields. For example, there is an emerging class of
sensors for detecting position, navigation and timing (PNT) at the
atomic scale. These micro-PNT devices can provide highly accurate
positioning data when GPS is jammed or unavailable. In this book we will
focus on quantum computation. One of the critical differences between
quantum and classical computation is that in quantum computation we are
manipulating quantum states themselves; this gives us a much larger
computing space to work in than in classical computers. In classical
computers, if we wish to model a real-world quantum physical xv

xvi

Preface to the First Edition

system, we can only do so with representations of such a system and we
cannot implement the physics itself. This key difference leads to
exciting possibilities for the future of computing and science. All this
starts with fundamental truths about our world that were developed
during the quantum mechanics revolution in the first half of the 20th
century. We will review a number of these core concepts in the first
chapter. I had the fortunate circumstance to have studied quantum
mechanics before learning classical physics and therefore relate to
quantum physics as the norm – it is my intellectual home. Until we
change our educational system, most students will learn the classical
before the quantum and so the quantum will seem doubly strange — both
from their own human experience as well as from the inculcation of
classical ideas before quantum ideas can be introduced. What is ironic
about this state of affairs is that the primary mathematical tool in
quantum mechanics is linear algebra, a powerful but very accessible
branch of mathematics. Most students, however, only take linear algebra
after two or three semesters of calculus, if they take it at all. Yet,
no calculus is needed to introduce linear algebra! In any case, we will
leave the remedying of mathematics education to another day while we
embark here on a journey into a new form of computing. In this book we
will explore how to build a computer of a very different kind than
humans have ever built before. What is distinct about this book is that
we will go beyond the theoretical into the practical work of how we can
build such computers and how we can write applications for these
systems. There are now several development libraries which we can use to
program cloud-based quantum systems. We will walk through code examples
and show the reader how to build a quantum circuit comprised of a set of
operators to address a particular challenge. We will mainly use Python
in this book. We are currently in the regime of noisy intermediate-scale
quantum (NISQ) computers, a term coined by John Preskill of CalTech
\[224\]. This refers to systems that do not yet have full
error-correction (thus noisy) and have dozens to thousands of qubits –
well short of the 106 C necessary for scaled faulttolerant computing.
Despite the limitations of these initial systems, the theory, algorithms
and coding techniques we cover in this book will serve readers as they
transition to larger systems that are to come in the future.

Preface to the First Edition

xvii

This work is three books in one: the first part covers the necessary
framework that drives the design of quantum computers and circuits. We
will also explore what kinds of problems may be amenable to quantum
computation in our treatment of complexity classes. The second part of
the book is for those readers who wish to delve into the programming
that makes these new machines tick. If you already have a background in
quantum mechanics, quantum information theory and theoretical computer
science (you know who you are!), you can jump right to the second part
and dig into the code. Please refer to the navigation guide in the
following pages to chart a course through this material. In the third
part we provide a set of critical tools to use in the journey to master
quantum computing (QC). We build up the core concepts of linear algebra
and tie them specifically to their use in QC. The table of operators and
circuit elements in chapter 15 is a handy reference as you design your
own quantum computing protocols. The book is also a portal to the
growing body of literature on the subject. We recommend that the reader
use the bibliography to explore both foundational and recent papers in
the field. We will provide further online examples and code tutorials on
a continual basis. This is a living text that will develop as QC
technology matures. We are all travelers together on this new adventure;
join us online at this book’s GitHub site.2 We are excited to see what
you will develop with these new platforms and tools. Contact us via the
site — we look forward to hearing from you. Jack D. Hidary June 2019
35,000 ft up

2 http://www.github.com/jackhidary/quantumcomputingbook

Acknowledgements

Let me start by thanking my publisher, Elizabeth Loew, who has been so
supportive throughout the process, and the entire SpringerNature team
for their excellence. A book like this is a significant undertaking and
it took a team of people to help in so many ways. The greatest of
appreciation to Stefan Leichenauer who did a great job as book editor
and formatter-in-chief. Stefan reviewed large parts of the book and I
thank him for his commitment to the project. The entire book is written
in TeX and we often pushed the boundaries of what TeX is capable of
implementing. Thank you to Sheldon Axler, author of Linear Algebra Done
Right (also by Springer) who generously shared his TeX template so that
we could format the book correctly for the Springer standards. Thanks to
the many experts who gave of their time to review key sections of the
book and provide technical advice. These include (in alphabetical
order): Scott Aaronson, Ryan Babbush, Sergio Boixo, Ruffin Evans, Eddie
Farhi, Patrick Hayden, Gerry Gilbert, Matt Reagor and Lenny Susskind.
Each improved the work materially with their input. I would also like to
recognize the significant achievement of Michael Nielsen and Isaac
Chuang in developing their textbook \[206\]. Recognition as well to John
Preskill for his in-depth lecture notes \[222\]. Nielsen, Chuang and
Preskill as well as Mermin \[194\] and Rieffel \[236\] have helped many
individuals enter the field. Thanks to my many colleagues at Alphabet,
Google, Sandbox and X who have encouraged this effort including: Sergey
Brin, Astro Teller and Hartmut Neven and his excellent team. Thank you
to the many participants in the workshops I taught on quantum computing
as well as my courses on linear algebra and other mathematical topics.
Your feedback has been invaluable. xix

xx

Acknowledgements

Hearty thanks to James Myer who worked with me intensively on the math
sections; James’ methodical approach assured us of success. We reviewed
these sections countless times, continually reworking them. James is not
only passionate about mathematics; he also cares deeply about pedagogy
and we had productive discussions on the best way to present the core
concepts. Thank you as well to Tai-Danae Bradley who also reviewed the
math sections and made very helpful suggestions. Thank you to Ryan
LaRose who worked with me on the code sections. In this emerging field
where the code frameworks have only been developed within the last few
years, solid information and examples can be hard to come by. Ryan
combined great skill in research as well as compiling the information in
succinct forms. Ryan also did a great job on the book’s GitHub site.
Thank you to Ellen Cassidy who did such a professional job proofreading
the text for grammar and consistency of format. Ellen has an eagle eye
and I commend her work to any author. Joe Tricot also did a wonderful
job coordinating the overall process. Thanks also to Nathan Schor and
Sam Ritchie for their eagle eyes on typo corrections for the second
edition. Naturally, even with all this help, there will remain items to
fix for the next edition. All remaining errors are mine and I will be
posting updates on the GitHub site and then include fixes in upcoming
versions. Thank you to my parents, David and Aimee Hidary, and my entire
wonderful family for their support through this process. It is a great
feeling to share this accomplishment with you.

Navigating this Book

Here are our suggestions to make the best use of this book: 1.
University instructors: You can build several different courses with the
material in this book. All code from the book is on the book’s website.
The math chapters have exercises embedded throughout; for other chapters
please consult the online site for coding exercises and other problem
sets. (a) Course in Quantum Computing for STEM majors: i. For this
course we recommend assigning chapters 1 and 2 as pre-reading for the
course and then proceeding chapter by chapter with the exercises
provided on the GitHub site. Solutions are also available on the site.
ii. If the students do not have sufficient depth in formal linear
algebra and related mathematical tools, Part III forms a strong basis
for a multi-week treatment with exercises. (b) Course in Quantum
Computing for physics graduate students: i. For this course, we
recommend using this book in conjunction with Mike and Ike (which is the
way many of us refer to Nielsen and Chuang’s excellent textbook \[206\])
or another suitable text which covers the theoretical concepts in depth.
We all owe a huge debt of gratitude to Michael Nielsen, Isaac Chuang and
authors of other textbooks over the last twenty years. We also recommend
referring to John Preskill’s lecture notes as you build your course for
advanced physics students \[222\]. Our work is meant to be complementary
to Mike and Ike in several respects: A. This work is more focused on
coding. For obvious reasons, books written prior to the past few years
could not have covered the dev tools and Python-based approaches to
quantum computing that now exist. xxi

xxii

Navigating this Book

B. This book does not go into the depth that Mike and Ike does on
information theoretic concepts. C. This book’s mathematical tools
section has a more detailed ramp-up for those students who may not have
taken a rigorous linear algebra course. The short summaries of linear
algebra and other requisite math tools in other textbooks on quantum
mechanics are often insufficient in our experience. ii. We recommend
first assigning chapters 1 and 2 as pre-reading. iii. Next, we suggest
covering the chapters on unitary operators, measurement and quantum
circuits with exercises on the Github site to check knowledge. iv. We
then recommend spending the bulk of the course in Part II to provide the
students with hands-on experience with the code. (c) Course in Quantum
Computing for CS graduate students: i. We suggest assigning the first
two chapters as pre-reading and then a review of mathematical tools in
Part III. Prior exposure to only undergraduate linear algebra is
typically insufficient as it was most likely taught without the full
formalism. ii. We then recommend chapters 3 and 4 to build up
familiarity with unitary operators, measurement and complexity classes
in the quantum regime. The instructor can make use of the review
questions and answers on the GitHub site. iii. The course can then cover
the approaches to building a quantum computer followed by all the coding
chapters. Please check the book’s GitHub site to find additional
resources including: code from the book, problem sets, solutions, links
to videos and other pedagogical resources. 2. Physicists: For physicists
who specialize in fields outside of quantum computing and wish to ramp
up quickly in this area, we recommend reading the brief history of QC as
we provide more detail than typical treatments, then the survey of
quantum hardware followed by the applications in the second part of the
book. 3. Software engineers: We recommend starting with the opening two
chapters, then reviewing the toolkits in Part III. We then suggest
returning to the treatment of qubits and unitary operators in Part I and
proceeding from there.

Navigating this Book

xxiii

4.  Engineering and business leaders: For readers who will not be doing
    hands-on coding, we recommend focusing on chapters 1- 4. The more
    adventurous may want to work through some of the code examples to
    get a tangible feel for the algorithms.
5.  Independent study: This book can easily be used as a text for
    independent study. We recommend combining it with online resources.
    Please consult the GitHub site for an updated list of resources:
    http://www.github.com/jackhidary/ quantumcomputingbook We recommend
    first assessing your current fluency on the core tools in Part III;
    there are numerous self-tests throughout the section that can be
    used for this purpose. The reader can then proceed to Part I. For
    those with a strong background in quantum mechanics and/or
    information theory we recommend looking up the papers referenced in
    chapters 2- 4 to gain a deeper understanding of the state of the
    field before proceeding to Part II: Hardware and Applications.
    Please consult the book’s GitHub site to find a range of resources
    including: code from the book, problem sets, solutions, links to
    videos and other pedagogical resources.

Part I

Foundations

CHAPTER

1 Superposition, Entanglement and Reversibility What is a quantum
computer? The answer to this question encompasses quantum mechanics
(QM), quantum information theory (QIT) and computer science (CS). For
our purposes, we will focus on the core of what makes a quantum computer
distinct from classical computers. 1.1

Quantum Computer Definition

A quantum computer is a device that leverages specific properties
described by quantum mechanics to perform computation. Every classical
(that is, non-quantum) computer can be described by quantum mechanics
since quantum mechanics is the basis of the physical universe. However,
a classical computer does not take advantage of the specific properties
and states that quantum mechanics affords us in doing its calculations.
To delve into the specific properties we use in quantum computers, let
us first discuss a few key concepts of quantum mechanics:  How do we
represent the superposition of states in a quantum system?  What is
entanglement?  What is the connection between reversibility,
computation and physical systems? We will be using Dirac notation,
linear algebra and other tools extensively in this text; readers are
encouraged to refer to the math chapters later in this work as well as
chapter 14 on Dirac notation to review as needed.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_1

3

4

CHAPTER 1 Superposition, Entanglement and Reversibility

1.1

Superposition and Entanglement

According to the principles of quantum mechanics, systems are set to a
definite state only once they are measured. Before a measurement,
systems are in an indeterminate state; after we measure them, they are
in a definite state. If we have a system, for example, that can take on
one of two discrete states when measured, we can represent the two
states in Dirac notation as j0i and j1i. We can then represent a
superposition of states as a linear combination of these states, such as
1 1 p j0i C p j1i 2 2 1.3

(1.2)

The Superposition Principle

The linear combination of two or more state vectors is another state
vector in the same Hilbert spacea and describes another state of the
system. a See

Part III for a treatment of Hilbert spaces

As an example, let us consider a property of light that illustrates a
superposition of states. Light has an intrinsic property called
polarization which we can use to illustrate a superposition of states.
In almost all of the light we see in everyday life — from the sun, for
example — there is no preferred direction for the polarization.
Polarization states can be selected by means of a polarizing filter, a
thin film with an axis that only allows light with polarization parallel
to that axis to pass through. With a single polarizing filter, we can
select one polarization of light, for example vertical polarization,
which we can denote as j"i. Horizontal polarization, which we can denote
as j!i, is an orthogonal state to vertical polarization1 . Together,
these states form a basis for any polarization of light. That is, any
polarization state j i can be written as linear combination of these
states. We use the Greek letter to denote the state of the system j i D
˛ j"i C ˇ j!i

(1.4)

The coefficients ˛ and ˇ are complex numbers known as amplitudes. In
this example, the coefficient ˛ is associated with vertical polarization
and the 1 We

could have equally used j0i and j1i to denote the two polarization
states; the labels used in kets are arbitrary.

SECTION 1.2 The Born Rule

5

coefficient ˇ is associated with horizontal polarization. The amplitude
has important interpretation in quantum mechanics which we will see
shortly. After selecting vertical polarization with a polarizing filter,
we can then introduce a second polarizing filter after the first.
Imagine we oriented the axis of the second filter perpendicular to the
axis of the first. Would we see any light get through the second filter?
If you answered no to this question, you would be correct. The
horizontal state j!i is orthogonal to the first, so there is no amount
of horizontal polarization after the first vertical filter. Suppose now
we oriented the axis of the second polarizing filter at 45° (i.e., along
the diagonal % between vertical " and horizontal !) to the first instead
of horizontally. Now we ask the same question — would we see any light
get through the second filter? If you answered no to this question, you
may be surprised to find the answer is yes. We would, in fact, see some
amount of light get through the second filter. How could this be if all
light after the first filter has vertical polarization? The reason is
that we can express vertical polarization as a superposition of diagonal
components. That is, letting j%i denote 45° polarization and j-i denote
45° polarization, we may write 1 1 j"i D p j%i C p j-i 2 2

(1.5)

As you may expect from geometric intuition, the vertical state consists
of equal parts j%i and j-i. It is for this reason that we see some
amount of light get past the second filter. Namely, the vertical
polarization can be written as a superposition of states, one of which
is precisely the 45° diagonal state j%i we are allowing through the
second filter. Since the j%i state is only one term in the
superposition, not all of the light gets through the filter, but some
does. The amount that gets transmitted is precisely 1=2 in this case.
(More formally, the intensity of the transmitted light is 1=2 that of
the incident light.) This value is determined from the amplitudes of the
superposition state by a law known as Born’s rule, which we now discuss.

1.2

The Born Rule

Max Born demonstrated in his 1926 paper that the modulus squared of the
amplitude of a state is the probability of that state resulting after

6

CHAPTER 1 Superposition, Entanglement and Reversibility

measurement \[47\]. In this case, since the amplitude is p1 , the
probability of 2 ˇ ˇ2 ˇ p1 ˇ 1 obtaining that state is ˇ ˇ D 2 ; so the
probability of measuring the light in 2 either the vertical or
horizontal polarization state is 50%. Note that we chose an amplitude of
p1 in order to normalize the states so that the sum of the 2 modulus
squared of the amplitudes will equal one; this enables us to connect the
amplitudes to probabilities of measurement with the Born rule. 1.6

The Born rule

In a superposition of states, the modulus squared of the amplitude of a
state is the probability of that state resulting after measurement.
Furthermore, the sum of the squares of the amplitudes of all possible
states in the superposition is equal to 1. So, for the state j i D ˛j0i
C ˇj1i, we have j˛j2 C jˇj2 D 1: While in the polarization example above
we have a 50/50 split in probability for each of two states, if we
examined some other physical system it may have a 75/25 split or some
other probability distribution. One critical difference between
classical and quantum mechanics is that amplitudes (not probabilities)
can be complex numbers. In other words, the coefficients ˛ and ˇ which
appear p in the statementpof the Born rule can be complex numbers, such
as i WD 1 or .1 C i /= 2. It is only after we take the square of the
modulus of these amplitudes that we get real numbers, hence actual
probabilities. Refer to chapter 11 to review complex numbers and how to
calculate the square of the modulus of a complex number. As if quantum
superposition were not interesting enough, QM describes a specific kind
of superposition which stretches our imagination even further:
entanglement. In 1935, when Einstein worked with Podolsky and Rosen to
publish their paper on quantum entanglement, their aim was to attack the
edifice of QM (this paper is now known as EPR \[100\]). Even though
Einstein earned the Nobel Prize for his 1905 work on the quantum nature
of the photoelectric effect, he nevertheless railed against the
implications of QM through his later years. Einstein wrote in 1952 that
quantum mechanics appears to him to be “a system of delusion of an
exceedingly intelligent paranoiac concocted of incoherent elements of
thought” \[99\]. He hoped that the EPR paper would demonstrate what he
perceived to be the deficiencies of QM.

SECTION 1.2 The Born Rule

7

EPR showed that if you take two particles that are entangled with each
other and then measure one of them, this automatically triggers a
correlated state of the second — even if the two are at a great distance
from each other; this was the seemingly illogical result that EPR hoped
to use to show that QM itself must have a flaw. Ironically, we now
consider entanglement to be a cornerstone of QM. Entanglement occurs
when we have a superposition of states that is not separable. We will
put this into a more formal context later on in this text. This "spooky
action at a distance" seems at odds with our intuition and with previous
physics. Podolsky, the youngest of the co-authors, reportedly leaked the
paper to the New York Times to highlight this assault on the tower of QM
to the public. The Times ran the story on the front page of the May 4th,
1935 edition with the headline “Einstein Attacks Quantum Theory." Not
only is entanglement accepted as part of standard quantum mechanics, we
shall see later in this work that we can leverage entanglement to
perform novel types of computation and communication. From an
information theoretic point of view, entanglement is a different way of
encoding information. If we have two particles that are entangled, the
information about them is not encoded locally in each particle, but
rather in the correlation of the two. John Preskill likes to give the
analogy of two kinds of books: nonentangled and entangled \[224\]. In
the regular, non-entangled book we can read the information on each page
as we normally do. In the entangled book, however, each page contains
what appears to be gibberish. The information is encoded in the
correlation of the pages, not in each page alone. This captures what
Schrödinger expressed when he coined the term entanglement: Another way
of expressing the peculiar situation is: the best possible knowledge of
a whole does not necessarily include the best possible knowledge of all
its parts. \[249\] Schrödinger further noted that in his opinion
entanglement was not just one of the phenomena described by quantum
mechanics,“but rather the characteristic trait of quantum mechanics, the
one that enforces its entire departure from classical lines of thought”
\[249\].

p

64

1.7

CHAPTER 1 Superposition, Entanglement and Reversibility

Entanglement

Two systems are in a special case of quantum mechanical superposition
called entanglement if the measurement of one system is correlated with
the state of the other system in a way that is stronger than
correlations in the classical world. In other words, the states of the
two systems are not separable. We will explore the precise mathematical
definitions of separability and entanglement later in this book.

1.3

Schrödinger’s Equation

As we saw above, we can represent the state of a system with a state
vector using Dirac notation. For example, if we wish to represent the
state of a system of one photon that is in a superpositon of vertical
and horizontal polarization we can use the following notation 1 1 j%i D
p j"i C p j!i 2 2

(1.8)

We can also represent the state vector with the Greek letter ‰ in the
ket – recall that the label in the ket is arbitrary. So we now have 1 1
j‰i D p j"i C p j!i 2 2

(1.9)

If we measure this photon for polarization we have a 50% probability of
finding the photon in a vertical polarization state and 50% probability
of finding it in a horizontal polarization state. In the Copenhagen
school of QM we say that the wave function has collapsed to one state or
the other. There are other interpretations of measurement of quantum
systems, but these are beyond the scope of this text. Now that we have a
method of representing the state of a system with a wave function, how
can we represent the evolution of this system through time? For this
exposition, let us consider the wave function of a particle that is
moving through free space which we can represent as ‰.x; t /

(1.10)

where x is its position at time t. The manner in which this wave
function evolves over time can be described by the time-dependent
Schrödinger equa-

SECTION 1.3 Schrödinger’s Equation

9

tion (SE). One conventional way of writing down the time-dependent SE
for a particle along one dimension is as follows @ ‰.x; t / D HO ‰.x; t
/ (1.11) @t There is no need to be intimidated by this mathematical
notation if it is new to you. We will explain the core concepts of the
SE here and the reader can find links to helpful videos on our companion
website for deeper exploration of the SE. On the left hand side (LHS) of
this equation, we see the constants i and \~. i of course is the symbol
that represents the square root of 1. \~ is the reduced form of the
Planck constant h. We call it the reduced form since we take h and
divide it by 2. The next set of symbols is the partial derivative of
the wave function with respect to t which denotes time. A partial
derivative with respect to time refers to how the function, in this case
the wave function ‰.x; t/, will change as t changes while holding
position, denoted as x, constant. The right hand side (RHS) of the
equation denotes the Hamiltonian operator applied to the wave function
‰. The Hamiltonian represents the total energy of a system; the total
energy includes all the kinetic energy, which we can represent as TO and
the potential energy, VO , of the particles in the system. Note that
some conventions use UO instead of VO to denote potential energy, but we
avoid that here to reserve U for the generic reference to unitary
operators which we will encounter later in this book. An operator is a
term we introduce in quantum mechanics for functions that operate on
wave functions. In addition to the Hamiltonian operator we often
encounter the position and momentum operators in QM which are
represented O respectively. Note the carat on top of these operators to
distinguish as xO and p, them from the position and momentum variables,
x and p. The SE tells us that if we want to know how the wave function ‰
will change over time we need to look at the total energy of the system.
We can break down HO to its component parts of TO and VO like so i\~

HO ‰ D TO ‰ C VO ‰

(1.12)

We can then replace TO ‰ with the quantized version of the expression
for kinetic energy. We start with the classical formula for kinetic
energy 1 T D mv2 2

(1.13)

10

CHAPTER 1 Superposition, Entanglement and Reversibility

then we can multiply both the numerator and denominator by m on the RHS
and then realize that since momentum, p, is mass times velocity, we
yield the following .mv2 /m .mv/2 p2 T D D D (1.14) 2m 2m 2m Now we can
take this classical expression and upgrade it to its quantum counterpart
by replacing p with the momentum operator pO which is pO D

i\~

@ @x

(1.15)

Since in equation 1.14 we have p 2 we replace it like so    1 @ @ O
T D i~\ i~ 2m @x @x

(1.16)

To simplify the RHS, we can do the following: realize that the i’s
cancel out to -1 so cancel those out and add a minus sign to the front
of the RHS, then collect the two \~’s to a single \~2 and finally
multiply out the two first order partial derivatives to yield a
second-order partial derivative as follows \~2 2m

TO D



@2 @x 2

 (1.17)

Now let’s turn to the LHS. Since we use the Schrödinger equation to
calculate the evolution over time of the wave function, we represent
this by the partial derivative of the wave function, ‰.x; t /, with
respect to t like so @‰.x; t / @t We now can put all the pieces together
as follows i\~

i\~

@‰.x; t/ D @t

\~2 @2 ‰.x; t / C VO ‰.x; t / 2m @x 2

(1.18)

(1.19)

Voila! Now, what about the term VO ‰.x; t /? This term has to be
determined for the system at hand. Let us consider the case of a quantum
harmonic oscillator. The potential energy of a harmonic oscillator such
as a spring is described by the following expression 1 V D kx 2 2 where
k is the spring constant of the oscillator. We then recall that

(1.20)

SECTION 1.4 The Physics of Computation

r !D

k m

11

(1.21)

where ! is the natural frequency of the system and m is the mass of the
system. We now have 1 1 V D kx 2 D m! 2 x 2 (1.22) 2 2 and therefore the
complete time-dependent SE for a quantum harmonic oscillator would be
the following i\~

@ ‰.x; t/ D @t

\~2 @2 ‰.x; t / 1 C m! 2 xO 2 ‰.x; t / 2m @x 2 2

(1.23)

where xO is evaluated as the x coordinate along the one dimensional
line. As an example of a quantum oscillator we can consider the
molecules of hydrogen or oxygen when found in their usual diatomic
state. The vibrations of these molecules follow the dynamics described
here for quantum harmonic oscillators. Other quantum systems would have
a different formula for their potential energy. In those cases we would
replace the oscillator potential energy formula for that specific
system’s potential energy formula to produce the SE for that wave
function’s evolution over time. Note that the SE is a first-order
partial derivative on the LHS and a secondorder partial derivative on
the RHS. This imbalance raises interesting questions that are beyond the
scope of this text, but we encourage the reader to investigate further.
The online companion site contains links to further videos and
resources.

1.4

The Physics of Computation

Now that we have covered two core ideas of quantum mechanics –
superposition and entanglement – let us turn to another fundamental
concept that is not treated as often – the physicality of information.
Rolf Landauer opened a new line of inquiry when he asked the following
question: The search for faster and more compact computing circuits
leads directly to the question: What are the ultimate physical
limitations on the progress in this direction? ...we can show, or at the
very least strongly suggest, that information processing is inevitably

12

CHAPTER 1 Superposition, Entanglement and Reversibility

accompanied by a certain minimum amount of heat generation. \[163\] In
other words, is there a lower bound to the energy dissipated in the
process of a basic unit of computation? Due to Landauer and others we
now believe that there is such a limit; this is called Landauer’s limit.
More specifically, the energy cost of erasure of n bits is nkT ln 2
where k is the Boltzmann constant, T is the temperature in Kelvin of the
heat sink surrounding the computing device and ln 2 is, of course, the
natural log of 2 ( 0:69315). This limit is the minimum amount of energy
dissipated for an irreversible computation. Landauer acknowledged that
this minimum is not necessarily the constraining factor on the energy
draw of the system: It is, of course, apparent that both the thermal
noise and the requirements for energy dissipation are on a scale which
is entirely negligible in present-day computer components. The
dissipation as calculated, however, is an absolute minimum. \[163\]
Landauer defined logical irreversibility as a condition in which “the
output of a device does not uniquely define the inputs.” He then claimed
that “logical irreversibility...in turn implies physical
irreversibility, and the latter is accompanied by dissipative effects.”
This follows from the second law of thermodynamics which states that the
total entropy of a system cannot decrease and, more specifically, must
increase with an irreversible process. For further background on
reversibility, thermodynamics and computation see Feynman’s Lectures on
Computation \[112\]. In classical computing we make use of irreversible
computations. For example, the Boolean inclusive OR (denoted \_) gate
has the following truth table, where 0 denotes “false” and 1 denotes
“true”: X 0 0 1 1

Y 0 1 0 1

X\_Y 0 1 1 1

Note that an output of value 1 cannot be traced uniquely to a set of
inputs. We can arrive at that output through combinations of inputs; the
state of the inputs is lost once we move to the output. This does not
violate the conser-

SECTION 1.4 The Physics of Computation

13

vation of information because the information was converted into
dissipative heat. The exclusive OR is also irreversible as is the NAND
gate, which is universal for classical computing. NAND stands for “NOT
AND” and is the inverse of the Boolean AND operator. Verify for yourself
that NAND is irreversible by examining its truth table: X 0 0 1 1

Y 0 1 0 1

X"Y 1 1 1 0

In quantum computing, we limit ourselves to reversible logical
operations \[206, p. 29\]. Later in this book we will consider which
combinations of quantum operators are universal, as well as examine
algorithms in the query model where uncomputing — the process of undoing
a series of reversible operations — is important. For now, let’s focus
on the requirement in quantum computation that we limit our set of
operators to reversible gates. This requirement derives from the nature
of irreversible operations: if we perform an irreversible operation, we
have lost information and therefore performed a measurement. Our
computation cycle then will be done and we can no longer continue with
our program. Instead, by limiting all gates to reversible operators, we
may continue to apply operators to our set of qubits as long as we can
maintain coherence in the system. When we say reversible, we are
assuming a theoretical noiseless quantum computer. In a noisy QC that
decoheres, we cannot, of course, reverse the operation. 1.24

Reversibility of Quantum Computation

All operators used in quantum computation other than for measurement
must be reversible. In this chapter, we have examined four essential
principles of quantum mechanical systems: superposition, the Born rule,
entanglement and reversible computation. All four are essential to
understanding the difference between classical and quantum computing as
we shall see further in the book. We provide references on this book’s
website to a number of resources for those who wish to deepen their
understanding of quantum mechanics.

Our generous universe comes equipped with the ability to compute. —Dave
Bacon \[22\]

CHAPTER

2

A Brief History of Quantum Computing The possibility that we can
leverage quantum mechanics to do computation in new and interesting ways
has been hiding in plain sight since the field’s early days; the
principles of superposition and entanglement can form the basis of a
very powerful form of computation. The trick is to build such a system
that we can easily manipulate and measure. While Richard Feynman is
often credited with the conception of quantum computers, there were
several researchers who anticipated this idea. In 1979, Paul Benioff, a
young physicist at Argonne National Labs, submitted a paper entitled
“The computer as a physical system: A microscopic quantum mechanical
Hamiltonian model of computers as represented by Turing machines”
\[30\].1 In this paper, Benioff demonstrated the theoretical basis for
quantum computing and then suggested that such a computer could be
built: That is, the whole computation process is described by a pure
state evolving under the action of a given Hamiltonian. Thus all the
component parts of the Turing machine are described by states which have
a definite phase relation to one another as the calculation
progresses...The existence of such models at least suggests that the
possibility of actually constructing such coherent machines should be
examined. Yuri Manin also laid out the core idea of quantum computing in
his 1980 book Computable and Non-Computable \[181\]. The book was
written in Russian, however, and only translated years later. 1 Note:
Benioff completed and submitted the paper in 1979. It was published in
the following year, 1980.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_2

15

16

CHAPTER 2 A Brief History of Quantum Computing

In 1981, Feynman gave a lecture entitled “Simulating Physics with
Computers” \[111\].2 In this talk, he argued that a classical system
could not adequately represent a quantum mechanical system: ...nature
isn’t classical, dammit, and if you want to make a simulation of nature,
you’d better make it quantum mechanical, and by golly it’s a wonderful
problem, because it doesn’t look so easy... He then set out the features
that a quantum computer should have to be useful. At the time of this
lecture, however, it was unclear to Feynman and the physics community
how one could build such a machine (for additional background see
\[225\]).

2.1

Early Developments and Algorithms

Once Benioff, Manin and Feynman opened the doors, researchers began to
investigate the nature of the algorithms that could be run on QCs. David
Deutsch, a physicist at Oxford, suggested a more comprehensive framework
for quantum computing in his 1985 paper \[88\]. In this work, he
describes in detail what a quantum algorithm would look like and
anticipates that “one day it will become technologically possible to
build quantum computers.” Deutsch then went on to develop an example of
an algorithm that would run faster on a quantum computer. He then
further generalized this algorithm in collaboration with Richard Jozsa
\[90\]. We will cover these and the other algorithms in more detail with
code examples later on in this text. In computer science and quantum
computing, it is often important to evaluate how efficient an algorithm
is — that is, how many steps would it take to run such an algorithm. We
use big-O notation to represent the upper bound of the worst case of
running an algorithm. The O in big-O notation comes from the “order” of
the algorithm. We use big- (Omega) notation to indicate the lower bound
of the worst-case scenario. So, while Deutsch’s problem takes at worst
O.n/ steps to solve on a classical computer, Deutsch-Jozsa’s algorithm
solves the problem in one step on a quantum computer. Big-O notation
will be helpful throughout this book in illuminating the difference
between the classical and quantum algorithms. Umesh Vazirani and his
student Ethan Bernstein picked up where Deutsch and Jozsa left off. In
1993, Bernstein and Vazirani (BV) published a paper which described an
algorithm that showed clear quantum-classical separation 2 Note: Feynman
gave his lecture in 1981 and submitted the lecture for publication in
May of 1981. The lecture was published by IJTP in 1982.

SECTION 2.1 Early Developments and Algorithms

17

even when small errors are allowed \[36\]. Why is this significant?
While Deutsch-Jozsa demonstrated a deterministic quantum advantage, if
small errors are allowed in the computation, both classical and quantum
versions can be run at worst in O.1/ steps, showing no separation. By
contrast, the Bernstein-Vazirani (BV) algorithm demonstrates separation
even when small errors are allowed, thus showing non-deterministic
quantum advantage. The problem posed in BV can be solved in O.n/ time on
a classical computer and in O.1/ using the BV circuit on a quantum
computer. BV made a further contribution in their 1993 paper. They
described a quantum version of the Fourier transform. This quantum
Fourier transform (QFT) would serve as a critical component for Peter
Shor when he developed his algorithm to factor large numbers. The work
of BV was quickly followed by Daniel Simon, then a postdoc at the
University of Montreal, in 1994. Simon outlined a problem that a quantum
computer would clearly solve exponentially faster than a classical one
\[257\]. To be more specific, Simon’s algorithm has an upper bound of
O.n/ on a quantum computer, but a higher .2n=2 / on a classical
computer. Since the lower bound on the classical computer is of higher
order than the upper bound on the quantum computer, there is a clear
demonstration of quantum advantage. Just prior to Daniel Simon’s work on
algorithms, Seth Lloyd, working at Los Alamos, published a paper in
Science which described a method of building a working quantum computer
\[173\]. He proposed that a system sending pulses into a unit can
represent a quantum state: Arrays of pulsed, weakly coupled quantum
systems provide a potentially realizable basis for quantum computation.
The basic unit in the array could be a quantum dot, a nuclear spin, a
localized electronic state in a polymer, or any multistate quantum
system that interacts locally with its neighbors and can be compelled to
switch between states with resonant pulses of light. Lloyd realized
that: The proposed device is capable of purely quantummechanical
information-processing capacities above and beyond the conventional
digital capacities already presented. One of the most important of these
capacities is that bits can be placed in superpositions of 0 and 1 by
the simple application of pulses at the proper resonant

18

CHAPTER 2 A Brief History of Quantum Computing

frequencies but at a length different from that required to fully switch
the bit. Such bits have a number of uses, including the generation of
random numbers. This was the first practical approach to a working QC.
It is interesting that Lloyd noted the possible use case of generating
random numbers from a quantum system; this has been a topic of recent
research in the quantum computing community. See, for example. \[139\]
and \[1\].

2.2

Shor and Grover

Enter Peter Shor. In 1994, Shor was a researcher in the mathematical
division of Bell Labs in New Jersey. Shor studied the work of Deutsch,
BV and Simon and realized he could construct an algorithm for factoring
large numbers into two prime factors; factoring large numbers is
believed to be intractable on a classical computer, but Shor’s factoring
algorithm runs quickly on a QC. Factoring large numbers is, of course,
the intentionally hard problem at the core of public key cryptography
(PKC) as implemented in the RSA algorithm\[239\], the kind of
cryptography that is the basis of almost all communications today over
the internet. This includes securely sending credit card numbers, bank
payments and ensuring the security of online messaging systems.
RSA-based cryptography depends on the one-way hardness of the factoring
of large numbers into two prime factors. Producing the large number is
easy; we just multiply the two factors. Given an arbitrarily large
number, however, it is exponentially difficult to find its two prime
factors. Inspired by Simon, Shor realized that we can use a QC to solve
another problem that is equivalent to the factoring problem; the
factoring problem is in fact equivalent to the period-finding problem
which Simon had tackled in his paper \[254\]. He also realized that the
QFT described by BV was exactly what he needed to set up the amplitudes
of each qubit prior to measurement so that the measurement would yield
the answer needed from the quantum computation with high probability.
Shor’s breakthrough led more researchers to work on quantum algorithms
since it then became clear that QCs, if built, would be quite powerful.
In fact, Shor’s algorithm is one of the first to have been demonstrated
on early QC physical systems. In 2001, Isaac Chuang et al. implemented
Shor’s algorithm on a nuclear magnetic resonance (NMR) system to factor
the number 15 as a demonstration \[278\].

SECTION 2.3 Defining a Quantum Computer

19

After Shor, Lov Grover contributed to the quantum algorithm arsenal by
demonstrating that one can achieve some speedup in a search algorithm on
a QC \[130\]. Grover’s algorithm only achieves quadratic speedup, not
exponential speedup (as Shor’s does), but this is still significant.
Quadratic speedup means that if an algorithm would take p O.N / steps on
a classical computer, we can achieve the same goal in O. N / steps on a
QC. A few months after Grover’s paper in May of 1996, Farhi and Gutmann
laid out the framework for a continuous time Hamiltonian version of
Grover’s algorithm \[107\]. This introduced the concept of Hamiltonian
oracles and the idea of implementing continuous time models of quantum
computation which are different than gate-based approaches. As one set
of researchers were making progress in identifying algorithms that would
run on a quantum computer with speedup over classical computers, others
were making progress on the physical implementation of a QC. In
19992001, Yasunobu Nakamura built and demonstrated a functioning,
controllable superconducting qubit \[202, 203\]. Nakamura used Josephson
junctions to create a two-level system that the user could manipulate
between its two states. We will discuss processors based on
superconducting qubits in chapter 5. Another approach to implementing a
quantum computer is to trap and manipulate ions. In 1995, Cirac and
Zoller proposed an ion trap as the physical system to perform quantum
computation \[79\]. In this setup, lasers are used to ionize atoms which
are then trapped in electric potentials. We will cover ion trap quantum
computers in chapter 5 as well.

2.3

Defining a Quantum Computer

As the activity in the quantum computing field began to rise,
researchers in the field formalized what constituted a quantum computer
and computation. In 1996, David DiVincenzo outlined the key criteria of
a quantum computer \[93\] in this manner:3 1. A scalable physical system
with qubits that are distinct from one another and the ability to count
exactly how many qubits there are in the system (no fudging allowed).
The system can be accurately represented by a Hilbert space. 3 Note that
we are summarizing DiVincenzo’s criteria from his original 1996 paper.
See \[94\] for another version of his criteria.

20

CHAPTER 2 A Brief History of Quantum Computing

2.  The ability to initialize the state of any qubit to a definite state
    in the computational basis. For example, setting all qubits to state
    j0i if the computational basis vectors are j0i and j1i.
3.  The system’s qubits must be able to hold their state. This means
    that the system must be isolated from the outside world, otherwise
    the qubits will decohere. Some decay of state is allowed (, where 
    is a small quantity). In practice, the system’s qubits must hold
    their state long enough to apply the next operator with assurance
    that the qubits have not changed state due to outside influences
    between operations.
4.  The system must be able to apply a sequence of unitary operators to
    the qubit states. The system must also be able to apply a unitary
    operator to two qubits at once. This entails entanglement between
    those qubits. As DiVincenzo states in his paper, “...entanglement
    between different parts of the quantum computer is good;
    entanglement between the quantum computer and its environment is
    bad, since it corresponds to decoherence” \[93, p. 4\].
5.  The system is capable of making “strong” measurements of each qubit.
    By strong measurement, DiVincenzo means that the measurement says
    “which orthogonal eigenstate of some particular Hermitian operator
    the quantum state belongs to, while at the same time projecting the
    wavefunction of the system irreversibly into the corresponding
    eigenfunction.” This means that the measuring technique in the
    system actually does measure the state of the qubit for the property
    being measured and leaves the qubit in that state. DiVincenzo wants
    to prevent systems that have weak measurement, in other words,
    measuring techniques that do not couple with the qubit sufficiently
    to render it in that newly measured state. At the time he wrote the
    paper, many systems did not have sufficient coupling to guarantee
    projection into the new state. In the last few years, we have
    witnessed a significant increase in the activity in the field. On
    the hardware side, there are numerous companies, large and small,
    that are now pursuing the various approaches described in chapter 5
    to build quantum computers. This has landed us in the era of noisy
    intermediate-scale quantum (NISQ) computers, a term coined by John
    Preskill of CalTech \[224\]. This refers to systems that do not yet
    have full error-correction (thus noisy) and have dozens to thousands
    of qubits – well short of the 106 C necessary for scaled
    fault-tolerant computing.

SECTION 2.3 Defining a Quantum Computer

21

With this increase in funding and attention in both the private and
public sectors, we anticipate significant developments in the field. Let
us now turn our attention to qubits and the operators we use in quantum
computation.

CHAPTER

3 Qubits, Operators and Measurement In this chapter we will cover qubits
and the core set of operators we use to manipulate the state of qubits.
A qubit is a quantum bit. A qubit is similar to a classical bit in that
it can take on 0 or 1 as states, but it differs from a bit in that it
can also take on a continuous range of values representing a
superposition of states. In this text we will use qubit to refer to
quantum bits and the word bit to refer to classical bits. While in
general we use two-level qubit systems to build quantum computers we can
also choose other types of computing architectures. For example, we
could build a QC with qutrits which are three-level systems. We can
think of these as having states of 0, 1 or 2 or a superposition of these
states. The more general term for such a unit is qudit; qubits and
qutrits are specific instances of qudits which can be computing units of
any number of states. The Siddiqi Lab at UC Berkeley, for example, has
designed a qutritbased QC \[42, 43\]. In a qutrit system we can
represent more states than a qubit system with the same number of
computational units. A qubit system of say 100 qubits can handle 2100
states (1:26765EC30), while a qutrit system can handle 3100 states
(5:15378EC47), a number which is 17 orders of magnitude larger. Put
another way, to represent the same number space as a 100 qubit system,
we only need  63 qutrits (log3 .2100 /). Since it is more difficult to
build qutrit systems, the mainstream QCs are currently based on qubits.
Whether we choose qubits, qutrits or some other

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_3

23

24

CHAPTER 3 Qubits, Operators and Measurement

qudit number, each of these systems can run any algorithm that the
others can, i.e., they can simulate each other.1 In QM we represent
states as vectors and operators as matrices; we use Dirac notation
instead of traditional linear algebra symbols to represent vectors and
other abstractions. Part III of this book contains a review of linear
algebra, Dirac notation and other mathematical tools that are crucial
for our inquiry into quantum computing. In this chapter we will assume
knowledge of these mathematical tools; we encourage the reader to use
the math chapters to review these concepts in the context of quantum
computing. Let us begin with the definition of a qubit: 3.1

What is a Qubit?

A physical qubit is a two-level quantum mechanical system. As we will
see in the chapter on building quantum computers, there are many ways to
construct a physical qubit. We can represent a qubit as a
two-dimensional complex Hilbert space, C2 . The state of the qubit at
any given time can be represented by a vector in this complex Hilbert
space. The Hilbert space is equipped, by definition, with an inner
product which allows us to determine the relative position of two
vectors representing qubit states. We denote the inner product of
vectors jui, jvi as hujvi ; this will equal 0 if jui and jvi are
orthogonal and 1 if jui = jvi. To represent two or more qubits we can
tensor product Hilbert spaces together to represent the combined states
of the qubits. As we shall see, we have methods to represent separable
states, where the qubits are independent of one another, and entangled
states such as a Bell state, where we cannot separate the two qubit
states. We can represent the states j0i and j1i with vectors as shown
below. We call these two the computational basis of a two-level system.
We can then apply operators in the form of matrices to the vectors in
the state space. j0i D

1 Note

  1 ; 0

j1i D

  0 1

that we could consider the same question in classical systems, i.e., we
could have used a 3-state “trit” instead of the bit, but we choose to
use bits as there are distinct advantages to the binary system.

CHAPTER 3 Qubits, Operators and Measurement

3.2

25

Quantum Operators

In gate-based quantum computers, the operators which we use to evolve
the state of the qubits are unitary and therefore reversible. Some of
the operators are unitary, reversible and involutive (i.e., they are
their own inverses); others are not involutive. A measurable quantity,
or observable, is a Hermitian operator; thus the measurement in a
quantum computer outputs real values from the system. We use the terms
operators and gates interchangeably. In addition to an inner product of
two vectors, linear algebra gives us the outer product. In this
operation, we take two vectors and form a matrix (whereas an inner
product gives us a scalar). If we take the outer product j0ih0j, for
example, we produce the following operator      1 1 0 1 0 D j0ih0j
D 0 0 0 Similarly, we can take the outer product of the other three
combinations to produce these matrices      1 0 1 0 1 D j0ih1j D 0
0 0 j1ih0j D

     0 1 0 0 0 D 1 1 0

     0 0 1 0 0 D j1ih1j D 1 0 1 so

We can take the sum of two of these matrices to form a unitary matrix,
like   0 1 (3.3) j0ih1j C j1ih0j D 1 0

This, in fact, is the X or NOT operator which we will encounter shortly
in this chapter. We have established that a qubit can be in one of the
computational basis states of 0 or 1 or in a superposition of these two
states. How can we represent the superposition of multiple states? We
can do so as a linear combination of the computational bases of the
state space.

26

CHAPTER 3 Qubits, Operators and Measurement

3.4

Representing Superposition of States

We represent a superposition of states as the linear combination of
computational bases of the state space. Each term in the superposition
has a complex coefficient or amplitude. Using the two computational
basis vectors in the case of a single qubit, two examples of
superpositions of states are 1 jCi WD p .j0i C j1i/ 2 and 1 j i WD p
.j0i 2

j1i/

These two states differ by a minus sign on the j1i state. More formally,
we call this difference a relative phase. The term phase has numerous
meanings in physics — in this context, it refers to an angle. The minus
sign is related to the angle  (180°) by Euler’s identity2 ei  D

1

Relative phases are of fundamental importance for quantum algorithms in
that they allow for constructive interference and destructive
interference. For example, if we evaluate the sum of the above states,
we obtain 1 1 1 p .jCi C j i/ D .j0i C j1i/ C .j0i 2 2 2

j1i/ D j0i

Here, we say that the amplitudes of the j1i state interfere
destructively — the differing relative phases cause them to sum to zero.
On the other hand, the amplitudes of the j0i state interfere
constructively — they have the same sign (relative phase), so they do
not sum to zero, and thus we are left with the state j0i as the result.
We can also consider subtracting the two superposition states. We leave
it to the reader to verify that 1 p .j i 2 2 For

jCi/ D

more on Euler’s identity, refer to chapter 13.

j1i

CHAPTER 3 Qubits, Operators and Measurement

27

Here, the amplitudes of the j0i state interfere destructively while the
amplitudes of the j1i state interfere constructively. In this example,
we do not end up with the j1i state exactly — it is multiplied by a
minus sign. As we saw above, we can interpret this minus sign as an
angle (or phase) e i  . Here, it is applied to the entire state, not
just one term in the superposition. We refer to this type of phase as a
global phase. While it is true that the j1i state is not exactly the j1i
state, we will see in future chapters that a global phase change has no
impact on quantum measurements. That is, the measurement statistics
obtained by measuring the j1i state and the j1i state are exactly
identical. In this case, we often say that the two states are equal, up
to global phase.

Quantum Circuit Diagrams We use circuit diagrams to depict quantum
circuits. We construct and read these diagrams from left to right; we
can think of circuit diagrams like a staff of music which we read in the
same direction. A quantum circuit specifies which operators we will
apply to which qubit or qubits in which order. Barenco et al. set forth
a number of the foundational operators that we use today in QC \[26\].
Fredkin and Toffoli \[275, 118\] added to this set with two ternary
operators. We begin the construction of a quantum circuit diagram with
the circuit wire which we represent as a line

A line with no operator on it implies that the qubit remains in the
state in which it was previously prepared. This means that we are
relying on the quantum computer to maintain the state of the qubit. We
denote the initial prepared state with a ket and label on the left of
the wire

j0i We denote n number of qubits prepared in that state with a slash n
symbol across the wire.

=n

28

3.1

CHAPTER 3 Qubits, Operators and Measurement

Quantum Operators

Let us now turn to the set of commonly used quantum operators. We denote
a single-qubit operator with a box containing the letter representing
that operator straddling the line. We denote a binary gate with an
operator box spanning two quantum wires and spanning three wires for a
ternary operator, etc. Note that we could have chosen a different set of
operators to accomplish universal quantum computation; the set of
operators chosen is arbitrary and is sufficient as long as it meets the
test of universality which we will cover later in this chapter. Here are
representations for unary and binary operators

U

U Unary Operators Let us now cover the set of one-qubit, or unary,
quantum operators. The first three operators we will examine are the
Pauli operators. These three matrices along with the identity matrix and
all of their ˙1 and ˙i multiples constitute what is known as the Pauli
group. First, we have X, which is the NOT operator (also known as the
bit flip operator and can be referred to as x )   0 1 X WD 1 0 If we
apply X to j0i then we have        0 1 1 0C0 0 D D D j1i 1 0 0
1C0 1 We can represent the initial state of a qubit and the operators we
apply to them with a circuit diagram. We use the following symbol to
represent the X operator in circuit diagrams

This is different from the convention of the operator name in a box,
which one may also encounter in circuit diagrams

SECTION 3.1 Quantum Operators

29

X As we have seen, we can represent the X operator in ket notation as X
WD j0ih1j C j1ih0j and the application of the X operator like so: X jj i
D jj ˚ 1i where j 2 f0; 1g. Here the ˚ operation denotes addition
modulo-2, and j ˚ 1 is equivalent to the NOT operation. So if we start
with the qubit in state j0i and apply NOT then we have

j0i

j1i

Next we have the Y operator, also denoted y , which rotates the state
vector about the y axis3 .   0 i Y D i 0 So that if we apply it to the
j1i state we have        0 i 0 0 i i D D D i 0 1 0C0 0

i j0i

The circuit diagram for the Y operator is

Y And the Z operator, also denoted z , which rotates the state vector
about the z axis (also called the phase flip operator since it flips it
by  radians or 180 degrees)   1 0 Z WD 0 1 If we apply Z to the
computational basis state we have Z jj i D . 1/j jj i or to show this in
matrix form for the special case j D 0 3 The

x, y and z axes in this section refer to representation of the qubit’s
state on a Bloch sphere, which we will cover later in this chapter.

30

CHAPTER 3 Qubits, Operators and Measurement



1 0

0 1

      1 1C0 1 D D D . 1/0 j0i D j0i 0 0C0 0

For the case where j D 1 we have        1 0 0 0C0 0 D D D . 1/1
j1i D 0 1 1 0 1 1

j1i

Note that we can multiply the bit-flip operator X by the phase-flip
operator Z to yield the Y operator with a global phase shift of i . That
is, Y D iXZ. The circuit diagram for the Z operator is

Z Next we turn to the more general phase shift operator. When we apply
this operator we leave the state j0i as is and we take the state j1i and
rotate it by the angle (or phase) denoted by ', as specified in the
matrix   1 0 R' WD 0 e i' So the Pauli Z operator is just a special
case of R' where ' D . Let’s recall that e i D 1 by Euler’s identity
(see chapter 13) so we can replace e i with 1 in the Z matrix. The
circuit diagram for the R operator is

R' Let’s discuss two additional phase shift operators that are special
cases of the R' matrix. First, the S operator, where ' D =2   1 0 S
WD 0 i The S operator thus rotates the state about the z-axis by 90°.
The circuit diagram for the S operator is

S Next let’s turn to the T operator which rotates the state about the
z-axis by 45°. If we give ' the value of =4 then4 4 Note that the T
gate is also known as the =8 gate, since if we factor out e i =8 , the
diagonal components each have j'j D =8, but this is of course the same
operator.

SECTION 3.1 Quantum Operators



1 0 T WD i =4 0 e

31



Note that S D T 2 . In other words, if we apply the T matrix to the
vector representing the state and then apply T again to the resulting
vector from the first operation we have accomplished the same result as
applying S once (45° C 45° D 90°/. The circuit diagram for the T
operator is

T Now let’s turn to the Hadamard operator. This operator is crucial in
quantum computing since it enables us to take a qubit from a definite
computational basis state into a superposition of two states. The
Hadamard matrix is   1 1 1 H WD p 1 2 1 It was actually the
mathematician John Sylvester who developed this matrix, but we name it
after Jacques Hadamard (see Stigler’s law of eponymy which, of course,
was probably conceived by Merton and others). The circuit diagram for
the H operator is

H If we apply the Hadamard to state j0i we obtain        1 1 1 1
1C0 1 1 j0i C j1i 1 Dp Dp D p p 1 1 0 1 C 0 1 2 2 2 2 And to state j1i
we have        1 1 1 1 0C1 1 j0i j1i 0 1 Dp Dp D p p 1 1 1 2 1 2
0 1 2 2 So we can see that the H operator takes a computational basis
state p and p projects it into a superposition of states .j0i C j1i/= 2
or .j0i j1i/= 2, depending on the initial state. p What is the 2 doing
in this state? Let us recall the Born rule that the square of the
modulus of the amplitudes of a quantum state is the probability of that
state. Furthermore, for all amplitudes ˛, ˇ, etc. of a state j˛j2 C jˇj2
D 1 That is, the probabilities must sum to one since one of the states
will emerge from the measurement.

32

CHAPTER 3 Qubits, Operators and Measurement

Before moving on to the binary operators, let us define the identity
operator and then determine which operators can be expressed as
sequences of other operators. The identity operator is simply the matrix
which maintains the current state of the qubit. So for one qubit we can
use   1 0 I WD 0 1 Having covered the set of unary operators, we can
show the following identities: HXH D Z HZH D X HYH D

Y

H D H H2 D I Please see chapter 15 for a list of additional identities.

Binary Operators Let us now consider two qubit, or binary, operators. In
a two-qubit system, by convention, we use the following computational
basis states: 0 1 0 1 0 1 0 1 1 0 0 0 B0C B1C B0C B0C C B C B C B C j00i
D B @0A ; j01i D @0A ; j10i D @1A ; j11i D @0A 0 0 0 1 Let us first
discuss the SWAP operator. The SWAP takes the state j01i to j10i and, of
course, j10i to j01i. We can represent this operator with the following
matrix 0 1 1 0 0 0 B0 0 1 0C C SWAP WD B @0 1 0 0A 0 0 0 1 And apply it
to a 4-d vector representing the state j01i as follows 0 10 1 0 1 0 1 1
0 0 0 0 0C0C0C0 0 B0 0 1 0C B1C B0 C 0 C 0 C 0C B0C B CB C B C B C @0 1
0 0A @0A D @0 C 1 C 0 C 0A D @1A D j10i 0 0 0 1 0 0C0C0C0 0

SECTION 3.1 Quantum Operators

33

Satisfy yourself that this operator applied to one of the two-qubit
computational basis vectors will have the desired result. For the
circuit diagram of the SWAP operator we use

  Now we come to a critical operator for quantum computing —
controlledNOT (CNOT). In this binary operator, we identify the first
qubit as the control qubit and the second as the target qubit. If the
control qubit is in state j0i then we do nothing to the target qubit.
If, however, the control qubit is in state j1i then we apply the NOT
operator (X) to the target qubit. We use the CNOT gate to entangle two
qubits in the QC. We can represent CNOT with the following matrix 0 1 1
0 0 0 B0 1 0 0C C CNOT WD B @0 0 0 1A 0 0 1 0 So, for example, we
compute the action of CNOT on the state j10i as follows 0 10 1 0 1 0 1 1
0 0 0 0 0C0C0C0 0 B0 1 0 0C B0C B0 C 0 C 0 C 0C B0C B CB C B C B C @0 0
0 1A @1A D @0 C 0 C 0 C 0A D @0A D j11i 0 0 1 0 0 0C0C1C0 1 And for the
circuit diagram, we depict the CNOT in this way



Here is an identity connecting the SWAP and CNOT operators: SWAPij D
CNOTij CNOTj i CNOTij Now let’s turn to another control operator: CZ.
Here we have a control qubit and a target qubit just as with CNOT;
however, in this operation if the control qubit is in state j1i then we
will apply the Z operator to the target qubit. We can represent the CZ
operator in a circuit diagram as

 Z

34

CHAPTER 3 Qubits, Operators and Measurement

and as a matrix

0 1 B0 C Z WD B @0 0

0 1 0 0

0 0 1 0

1 0 0C C 0A 1

We can represent the CZ operator in circuit diagrams as

  Note that unlike the CNOT gate, the CZ gate is symmetric: we can
choose either qubit as the control or the target and we will end up with
the same result. This is why we can represent the CZ gate with a dot on
both circuit wires.

Ternary Operators We have discussed both unary and binary operators. Now
let’s consider the ternary or 3-qubit operators. First, we have the
Toffoli operator, also known as the CCNOT gate \[275\]. Just as in the
CNOT operator, we have control and target qubits. In this case, the
first two qubits are control and the third is the target qubit. Both
control qubits have to be in state j1i for us to modify the target
qubit. Another way of thinking about this is that the first two qubits
(x and y) have to satisfy the Boolean AND function — if that equals TRUE
then we apply NOT to the target qubit, z. We can represent this action
as .x; y; z/ 7! .x; y; .z ˚ xy// or, as a matrix, 1 B0 B B0 B B0 B B0 B
B0 B @0 0 0

0 1 0 0 0 0 0 0

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 1 0 0 0

0 0 0 0 0 1 0 0

0 0 0 0 0 0 0 1

1 0 0C C 0C C 0C C 0C C 0C C 1A 0

As an example, we apply this gate to the state j110i

SECTION 3.1 Quantum Operators

0 1 B0 B B0 B B0 B B0 B B0 B @0 0

0 1 0 0 0 0 0 0

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 1 0 0 0

0 0 0 0 0 1 0 0

0 0 0 0 0 0 0 1

35

10 1 0 1 0 0 0 B0C B0C 0C CB C B C B C B C 0C C B0C B0C B C B C 0C C B0C
D B0C D j111i C C B C 0C B B0C B0C C B B C 0C B0C C B0C 1A @1A @0A 0

0

1

In circuit diagrams, we use the following to denote the Toffoli

  Next, let’s consider the Fredkin gate, also known as the CSWAP gate
\[118\]. When we apply this operator, the first qubit is the control and
the other two are the target qubits. If the first qubit is in state j0i
we do nothing and if it is in state j1i then we SWAP the other two
qubits with each other. The matrix representing this operations is 1 B0
B B0 B B0 B B0 B B0 B @0 0 0

0 1 0 0 0 0 0 0

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 1 0 0 0

0 0 0 0 0 0 1 0

0 0 0 0 0 1 0 0

1 0 0C C 0C C 0C C 0C C 0C C 0A 1

For example, the Fredkin gate applied to j110i gives 0 1 B0 B B0 B B0 B
B0 B B0 B @0 0

0 1 0 0 0 0 0 0

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 1 0 0 0

0 0 0 0 0 0 1 0

0 0 0 0 0 1 0 0

10 1 0 1 0 0 0 C B C B 0C B0C B0C C B C B C 0C C B0C B0C B C B C 0C C
B0C D B0C D j101i C C B C 0C B B0C B0C B C B C 0C C B0C B1C A 0 @1A @0A
1

0

0

In circuit diagrams we use this symbol for the Fredkin operator

36

CHAPTER 3 Qubits, Operators and Measurement

  

3.2

Comparison with Classical Gates

In classical computing we have a set of commonly used gates: AND, NOT,
OR, NAND, XOR, FANOUT, etc. We can use combinations of these gates to
perform any computation in classical computing. A classical computer
that can run these gates is Turing-complete or universal. In fact, we
can show that the NAND gate alone is sufficient to construct all other
classical operators \[252\] (and so is the NOR gate!). We can construct
classical circuits with these basic building blocks such as a circuit
for the half-adder

Figure 3.1: Half-adder in classical computing

Source: Wikimedia

We can then build a full-adder from those elements:

Figure 3.2: Full-adder in classical computing

Source: Wikimedia

SECTION 3.3 Universality of Quantum Operators

37

Neither AND, OR, XOR, NAND or FANOUT can be used in quantum computing.
The AND, OR, XOR and NAND gates are not reversible. The FANOUT gate
would not be allowed in quantum computing since it involves the
duplication, or cloning, of a state; this would violate the no-cloning
theorem. Of the primary classical gates, only the NOT operator can be
used in the quantum computing regime as it is reversible and does not
involve cloning. For more reading on classical gates and computer
architectures, see \[27, 112, 167\].

3.3

Universality of Quantum Operators

If NAND is universal for classical computing, is there such a gate or
set of gates that are universal for quantum computing? In fact, there
are several combinations of unary and binary operators that lead to
universality. No set of unary gates on their own can achieve universal
QC. Two of the gate sets that yield universality are: 1. The Toffoli
gate is universal for QC when paired with a basis-changing unary
operator with real coefficients (such as H ) \[253\]. 2. Another set of
gates which is universal is fCNOT; T; H g \[53, 206\]. Another way of
stating this approach is to realize that S is T 2 ; we then recall that
the Clifford group of operators is generated by the set C D fCNOT; S; H
g \[128\] \[214\]. Therefore, by definition we can achieve universality
in quantum computing by utilizing the Clifford group of operators along
with the gate T .

3.4

Gottesman-Knill and Solovay-Kitaev

The Gottesman-Knill theorem states that circuits built with only
Clifford gates can be simulated efficiently on classical computers
assuming the following conditions:  state preparation in the
computational basis  measurements in the standard basis  any classical
control conditioned on the measurement outcomes A further theorem that
is worth considering at this juncture is that of Solovay-Kitaev. This
theorem states that if a set of single-qubit quantum gates generates a
dense subset of S U.2/, which is the special unitary group of unitary
matrices which are 2 x 2, then that set is guaranteed to fill S U.2/
quickly, i.e., it is possible to obtain good approximations to any
desired

38

CHAPTER 3 Qubits, Operators and Measurement

gate using surprisingly short sequences of gates from the given
generating set \[85\]. The theorem generalizes to multi-qubit gates and
for operators from SU(d) \[85\]. A simplified version of this statement
is that all finite universal gate sets can simulate a given gate set to
a degree ı of precision. More precisely, if L is the size of the circuit
(i.e., the number of gates) then the approximation L0 of L has a bounded
number of gates; this can be specified in big-O notation by    0 4 L
L D O L log ı If D denotes the depth of the circuit, i.e., the number of
computational steps, then the approximation D 0 of D has a bounded depth
specified in big-O notation by    4 D D D O L log ı 0

So, these expressions demonstrate that the simulation is quite efficient
and better than polynomial time.

3.5

The Bloch Sphere

There are several ways to represent the state of a qubit: 1. We can
write out the state in Dirac notation. For example, if we have a qubit
that is prepared in state j0i and then apply the X operator, we will
then find the qubit in state j1i (assuming no outside noise) X j0i ! j1i
2. We can use the Bloch sphere to represent the state of a single qubit.
Any state in a quantum computation can be represented as a vector that
begins at the origin and terminates on the surface of the unit Bloch
sphere. By applying unitary operators to the state vectors, we can move
the state around the sphere. We take as convention that the two
antipodes of the sphere are j0i on the top of the sphere and j1i on the
bottom. As we can see in Figure 3.3, one of the advantages of
visualization with the Bloch sphere is that we can represent
superposition states such as j0i C j1i p 2

SECTION 3.6 The Measurement Postulate

39

as we see at the X axis. We can also differentiate between states that
contain different phases as is shown in the states along the X and Y
axes. Let us return to computational universality which we treated
above. Now that we have introduced the Bloch sphere, another way to
think about a set of gates that satisfies universal computation is one
which enables us to reach any point on the Bloch sphere.

Figure 3.3: The Bloch sphere

Source: \[122\]

For interactive visualizations of qubits on the Bloch sphere, see the
book’s online website. Now that we have covered the main unitary
operators which we use in QC, let’s turn to the measurement of the QC’s
state.

3.6

The Measurement Postulate

Measurement in classical physics is a seemingly straightforward process.
The act of measurement is assumed to have no effect on the item that we
are measuring. Furthermore, we have the ability to measure one property
of a system, get a reading, then measure another property and be
confident that the first property measured still retains its observed
value. Not so in quantum mechanics; in this regime, the act of
measurement has a profound effect on the observation. Building on the
principles of quantum mechanics, we can state the measurement postulate
as: 3.5

Measurement Postulate

Every measurable physical quantity, o, is described by a corresponding
Hermitian operator, O, acting on the state ‰.

40

CHAPTER 3 Qubits, Operators and Measurement

According to this postulate, there exists a Hermitian operator, which we
call an observable, associated with each property. So, for example, the
observable xO is associated with the position of a particle. We recall
that a Hermitian operator is equal to its adjoint (which is its complex
conjugate transpose). If O is Hermitian then we can state that O D O 
(see chapter 12 for more discussion on Hermitians). Hermitian operators
have the desirable property that their eigenvalues are guaranteed to be
real numbers. When measuring a physical system for properties such as
momentum or position we need to specify a real number. Each possible
outcome of the measurement is an eigenvalue, ; of the observable and is
characterized by jP j i j2 where P is the projector onto the eigenspace
of the observable. Since we normalize the vectors, the state after
measurement is represented by a unit eigenvector of the observable with
eigenvalue i . We discussed earlier how a system can be in a
superposition of two or more states. We can represent this as a linear
combination of the orthonormal basis vectors. For example, 1 1 j‰i D p
j0i C p j1i 2 2 This leads to the question of how we can set up the
measurement in such a way as to obtain the output we require. This in
turn is dependent on the amplitudes of each state since, as discussed
previously, the square of the modulus of the amplitude is the
probability of that state appearing as the output upon measurement
(Born’s rule). We can represent a measurement in a quantum circuit like
this:

Now that we have our unitary and measurement operators, we will
construct some basic quantum circuits. Let’s figure out what this one
does:

j0i

H



j0i We start with two qubits, let’s call them q0 and q1, each prepared
in state j0i. We then apply the Hadamard operator to q0 which puts it
into the superposition of states 1 1 jq0i D p j0i C p j1i 2 2

SECTION 3.7 Computation-in-Place

41

We then apply a CNOT across q0 and q1. This entangles the two qubits so
we now have the combined, non-separable state of the two qubits of 1 1 p
j00i C p j11i 2 2 We have thus created a Bell state, or an EPR pair. We
then measure q0 with a 50/50 chance of finding a 0 or a 1 value for the
real-valued output.

3.7

Computation-in-Place

We can depict the circuit in a 3-dimensional manner as in Figure 3.4.
Here you can see the qubits beginning in a prepared state followed by a
Hadamard step to put them all into a superposition; then they undergo a
series of one and two-qubit operations such as X, Y , T and CZ.
Measurement is then applied in the final step. In this diagram, we see a
crucial difference between classical and quantum computing.

Figure 3.4: 3-D Quantum circuit diagram

Source: Google

42 3.6

CHAPTER 3 Qubits, Operators and Measurement

Computation-in-Place

In most forms of gate-based quantum computing, the information is
represented in the states of the qubits as they evolve over time with
the successive application of unitary operators. Computation-in-place is
in stark contrast to classical computing, where we shuttle data around
the processor to various memory and calculation registers. In most forms
of quantum computers, all processing takes place on the qubits
themselves. After measurement in a QC we output real-valued bits which
we can share with the CPU that is controlling the quantum processor and,
if necessary, incorporate in further processing on classical machines.
We now come to one of the key questions in quantum computing: if
measurement is based on the modulus squared of the amplitude of each
qubit state, then how can we pre-determine which of the qubits will be
the output? Deutsch, Jozsa, Bernstein, Vazirani, Shor and others
realized that we can influence the output by setting up the amplitudes
prior to measurement to favor the output we need for that computational
task. One method for accomplishing this goal is the quantum Fourier
transform (QFT – not to be confused with quantum field theory!). By
applying a QFT across all qubits prior to measurement, we can obtain
phase information upon measurement instead of amplitude information. The
QFT is an efficient process on a quantum computer: the discrete Fourier
transform on 2n amplitudes only takes O.n2 / applications of Hadamard
and phase-shift operators (where n is the number of qubits). We will
cover the QFT in greater detail later in this text. Here we display the
circuit for QFT for n D 4:

jx1 i jx2 i jx3 i jx4 i

H R=2 R=4 R=8 H R=2 R=4

 

H R=2

 





H

Before we turn our attention to quantum hardware, let’s delve into
computational complexity in the next chapter. This will give us the
foundation to understand which sorts of problems are appropriate for a
quantum computer.

If you take just one piece of information from this blog: Quantum
computers would not solve hard search problems instantaneously by simply
trying all the possible solutions at once. —Scott Aaronson

CHAPTER

4

Complexity Theory Since quantum computing offers an alternative approach
to computation, it is logical to consider which classes of problems are
now tractable in this new regime that were not thought to be tractable
in a classical framework. To do so, let’s consider a range of problem
classes.

4.1

Problems vs. Algorithms

Let us first clarify the difference between computational problems (or
tasks), algorithms and programs. Here is an example of a computational
problem: Given a data set of n numbers, sort the numbers in increasing
numerical order. We can then analyze several different algorithms to
solve this problem: quicksort, merge sort, insertion sort and others. An
algorithm is a hardwareindependent method of solving a computational
problem. We generally try to find algorithms that can solve a problem
efficiently. A program is a particular implementation of an algorithm in
a given coding language. Analysis of algorithms is the study of the
resources that an algorithm needs to run.1 We can bucket algorithms into
different computational orders both in time (number of steps) and space
(amount of memory). Computational complexity theory, by contrast, is the
study of classes of problems; we will define a number of important
problem classes below. 1 Note:

It is common to refer to the analysis of the time and memory resource
requirements of an algorithm as the time and space complexity of the
algorithm. Although the strict definition of "complexity" would only
apply to computational problems, the usage is sufficiently widespread
that we will occasionally use complexity in the context of algorithms as
well.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_4

43

44

CHAPTER 4 Complexity Theory

When defining complexity classes we focus on decision problems; these
are mathematical problems that can be answered with a binary yes/no
response given an input. Examples of decision problems include: Given x,
is x a prime number? Given x and y, does y divide x evenly? Complexity
analysis for a decision problem determines the computational resources
needed to deliver an answer. We generally look at the characteristics of
the worst-case scenario for this determination.

4.2

Time Complexity

As we discussed in an earlier chapter, we can use big-O notation to
denote the upper bound of the worst case of a problem. For example, if
we have a series of items that we want to sort, the big-O time
complexity will depend on which algorithm we choose to sort the items.
Here are some complexity orders of common sorting algorithms: 
Insertion sort: O.n2 /  Mergesort: O.n log.n//  Timsort: O.n log.n//
These differences can be significant if n is large. When analyzing
algorithms for the computational resources needed to run them, we are
performing asymptotic analysis; in other words, what resources will be
needed as the input, n, gets very large. Refer to Figure 4.1 for a plot
of common big-O time computational orders. In addition to big-O notation
which designates the upper bound on the worst case computational order
for that algorithm, we can consider big- (Omega) notation which
designates the lower bound of the worst case computational order. Adding
now to the list above we can compare lower and upper bounds for the
computational resources needed for these sorting algorithms:  Insertion
sort: .n/, O.n2 /  Mergesort: .n log.n//, O.n log.n//  Timsort:
.n/, O.n log.n//

SECTION 4.2 Time Complexity

Figure 4.1: Big-O time complexity chart

45

Source: \[23\]

We see that the lower bound for insertion sort and timsort are
significantly better than their upper bound. However, since we have to
plan for the upper bound, we generally focus on the big-O complexity.
There is a third metric we use for cases in which the upper bound
(big-O) and the lower bound (big-) of the worst-case match. For these
algorithms we can describe their big-‚ computational order, which is
both their big-O and their big- since they match. To use more formal
notation, we say that a function f .n/ (which could represent the time
necessary to run an algorithm for an input of size n) is on the order of
a function g.n/ (which could represent the time necessary to run a
different algorithm given n inputs) if and only if the limit superior of
the absolute value of the quotient of f .n/ and g.n/ is finite as n
tends to infinity. In symbols ˇ ˇ ˇ f .n/ ˇ ˇ ˇ&lt;1 f .n/ D O.g.n// if
and only if lim sup ˇ ˇ n!1 g.n/ In this expression, lim sup is the
limit superior or supremum limit. Following Hardy and Littlewood \[134\]
and as described by Knuth \[156\], we state that f .n/ D .g.n// iff
g.n/ D O.f .n//

46

CHAPTER 4 Complexity Theory

and f .n/ D ‚.g.n// iff f .n/ D O.g.n// and f .n/ D .g.n// There are
two more notations called little-o and little-!. Little-o provides a
strict upper bound (equality condition is removed from big-O) and
little-! provides a strict lower bound (equality condition removed from
big-). Let’s also introduce the concept of completeness. A problem, G,
is said to be H-complete if it is a part of class H and we can prove
that all problems in class H can be reduced to G. In other words, if we
have a subroutine, S , which when run can solve for problem G, and this
subroutine can also solve for any problem in H , then we can say that
all problems in H can be reduced to G and that G is H-complete.

4.3

Complexity Classes

Let us first define a number of common complexity classes from classical
computing: P – Polynomial time: problems that can be solved in
polynomial time. In other words, the problem can be solved in a
reasonable amount of time on a classical computer. Problems of O.1/,
O.log.n//, O.n/, O.n log.n//, and O.n2 /, as examples, are in class P.
Although O.log.n// doesn’t look polynomial since log.n/ is not a
polynomial in n, O.log.n// is in P since is it upper-bounded by O.n2 /,
which is a polynomial. NP – Non-deterministic polynomial time: a problem
is in NP if whenever the answer is "yes," there’s a polynomialsize
witness or proof for the yes-answer, which a polynomial-time algorithm
can verify. We can imagine a Turing machine which can switch to a state
that is not determined by its previous state. If PSPACE and related
classes through such a move it happens upon a Source: Wikimedia correct
solution to a problem, this solution can be verified in polynomial time.
A problem, A, is said to be NP-Complete iff2 : (1) A is in NP, and (2)
all NP problems are polynomial-time reducible to A. If we only know (2),
and not necessarily (1), we say A is NP-hard. 2 Note:

we often abbreviate if and only if as iff throughout the book.

SECTION 4.3 Complexity Classes

47

Figure 4.2: Complexity classes - note: it is not yet proven whether
graph isomorphism is in P or not Source: \[2\]

One of the seven Clay Mathematics Institute Millennium Problems is the
question of whether the complexity class P is equivalent to the class
NP. This \$1 million challenge is the most recently developed of all the
Clay prizes and is most closely tied to computer science; this question
is still the subject of active research. PSPACE – Polynomial space: This
class focuses on memory resources, not time. PSPACE is the class of
decision problems that are solvable by some algorithm whose total space
usage, in all instances, can be upper-bounded by a polynomial in the
instance size. See Figure 4.2 for the position of PSPACE in the context
of other classes. BPP – Bounded-error probabilistic polynomial time: BPP
is a class that contains P; many believe that BPP = P, but we have not
been able to prove that yet \[3, Lecture 4\]. BPP is the class of
decision problems for which there exists a polynomial-time randomized
algorithm that solves every instance with a success probability of at
least 32 (over the choice of random bits). The core idea of BPP is that
sometimes randomized algorithms give us faster

48

CHAPTER 4 Complexity Theory

time results than a deterministic algorithm trying to achieve the same
goal. Problems that are in BPP either have a deterministic algorithm
that can run in polynomial time or have a probabilistic algorithm which
will give the wrong answer to a decision problem no worse than 13 of the
time. The bound of 13 is not fixed. We can choose any lower bound in the
interval Œ0; 12 / and BPP will not change. The reason is that when run
many times the overall probability of producing a wrong error is low.
This is described by the Chernoff bound. Now let us consider a range of
complexity classes that arise with quantum computing: BQP –
Bounded-error quantum polynomial time: BQP is the quantum analogue of
the class BPP for classical computation. A decision problem is in BQP if
it can run in polynomial time and yields a correct result with a high
probability. BQP is the primary complexity class we focus on for QC. As
you can see from Figure 4.2, BQP contains problems which are thought to
be intractable in the classical regime but are thought to be tractable
in bounded-error polynomial time for a quantum computer. We say "thought
to be" as it is still not yet proven whether the computational problem
of factoring large numbers, for example, is in P or NP. Although we have
no classical algorithm at the moment that can factor large numbers, this
does not mean such an algorithm does not exist. Thus, complexity
theorists are not sure of the exact position of BQP with respect to P,
NP and PSPACE \[206\]. EQP – Exact quantum polynomial time: this is the
set of decision problems solvable by a quantum circuit that yields the
correct answer with a probability of 1. In other words, this class is
the same as BQP except that it must give the correct answer with
probability of 1 instead of having some bounded error margin \[6\]. Note
that a QC does not render all NP problems tractable; only problems that
have some structure we can exploit can be handled efficiently by a QC.
For example, Shor’s algorithm takes advantage of the periodicity of the
function which then enables us to solve the equivalent problem of
factoring a large number. QMA – Quantum Merlin-Arthur: QMA is the
quantum analogue to the non-probabilistic class MA. In a Merlin-Arthur
(MA) problem, a prover (Merlin) sends a message to a verifier (Arthur).
In the classical complexity class MA, Arthur can verify the message in
polynomial time. Problems that live in QMA are ones with the following
characteristic \[46\]:

SECTION 4.4 Quantum Computing and the Church-Turing Thesis

49

 If the answer is Yes, then the verifier can verify with probability
greater than 23 using a proof that can run in polynomial time on a
quantum computer.  If the answer is No, then the verifier can reject
the proof with a wrong outcome in no more than 13 of the cases. Table of
Classical and Quantum Complexity Classes3 Classical P BPP NP

4.4

Quantum EQP BQP QMA

Quantum Computing and the Church-Turing Thesis

Let us now turn to the relationship between quantum computing and the
Church-Turing thesis. Alonzo Church and Alan Turing developed the
initial conjecture that: 4.1

Church-Turing Thesis (CTT)

If an algorithm can be performed on any piece of hardware (say, a modern
personal computer), then there is an equivalent algorithm for a
Universal Turing Machine (UTM) which performs exactly the same algorithm
\[206, p. 5\]. This conjecture was then updated to take into account the
efficiency of the algorithm. Algorithmic efficiency refers to the
quantification of a particular resource that is used in running the
algorithm. It is important in this analysis to maintain consistency when
comparing the efficiency of a set of algorithms; if we are analyzing the
number of steps of one algorithm, we should do so for all others in the
comparison and not switch to the analysis of memory resources, for
example, midway through the analysis. The additional requirement of
running an algorithm efficiently gives us the Strong Church-Turing
Thesis (SCTT): 3 Readers

interested in this subject should consult the complexity zoo \[6\].

50 4.2

CHAPTER 4 Complexity Theory

Strong Church-Turing Thesis (SCTT)

Any algorithmic process can be simulated efficiently using a Universal
Turing Machine (UTM) \[206, p. 5\]. Researchers then realized that there
were probably counterexamples to the SCTT, namely, algorithms that made
use of randomness. For example, Solovay and Strassen demonstrated that
an algorithm using randomness could test for primality of a number
\[262\]. By repeating the algorithm a finite number of times, one could
obtain a correct answer with almost near certainty. It was later shown
that there is an efficient polynomial-time algorithm for testing
primality \[9\], but historically, it was the initial insight that an
algorithm using randomness could get the task done that led to the
refinement of the SCTT. The SCTT was thus updated to give us the
Extended CTT (ECTT): 4.3

Extended Church-Turing Thesis (ECTT)

Any algorithmic process can be simulated efficiently using a
Probabilistic Turing Machine (PTM) \[206, p. 6\]. Enter quantum
computation. QC challenges the ECTT by demonstrating that it can solve
certain problems exponentially faster than a classical computer. This
undermines the ECTT assertion that any UTM or even PTM can simulate any
other computing device in running any given algorithm \[11\]. We now
arrive at the quantum version of the ECTT, which still stands: 4.4

Quantum Extended Church-Turing Thesis (QECTT)

Any realistic physical computing device can be efficiently simulated by
a fault-tolerant quantum computer. Now that we have a foundation of
quantum operators, circuits and complexity classes, let us explore how
to build a physical quantum computer.

Part II

Hardware and Applications

CHAPTER

5 Building a Quantum Computer Now that we have covered the essential
workings of a quantum computer, let us discuss how we can physically
realize these devices. There are many different architectures and
designs of gate-based quantum computers each with its own pros and cons.
In this chapter we will cover the leading paradigms of quantum
computational hardware. Check the book’s online site for updates as the
technology is changing rapidly.1 All of the architectures below require
a set of classical computers for control of the system. As you can see
in Figure 5.6, a superconducting qubit QC, for example, is controlled by
a traditional computer. We develop our quantum circuit protocols in
high-level languages on the classical computer which can then manipulate
the quantum system to apply the operators in the circuit. Upon
measurement, the output of a QC is classical information which is fed
back to the classical computer for readout or further processing. We can
think of the QC portion of a computation as a subroutine in a much
larger computation, much of which may take place in the classical
regime. We can therefore refer to a quantum computer as a quantum
processing unit (QPU) and we envision these QPUs will be used in
combination with CPUs, GPUs and other processors to complete
computational tasks. In the application of Shor’s algorithm, for
example, many tasks are performed by the classical computer and then the
hard part – the implementation of the period-finding algorithm (which is
a key step in prime number factoring) – is sent out as a subroutine to
the QC. This output is then integrated back into the classical platform.
1 The

online site is at this URL:
https://github.com/jackhidary/quantumcomputingbook

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_5

53

54

5.1

CHAPTER 5 Building a Quantum Computer

Assessing a Quantum Computer

There are many advances occurring in quantum hardware. Here is a useful
checklist to analyze the potential impact of engineering progress in
this field: 1. Universality: The first question to ask about a hardware
platform that is presented as a quantum computer is whether it is
Turing-complete, or universal. The device may be a non-universal
annealer, for instance. We can turn to the DiVincenzo criteria we
described in chapter 2 to aid us in this test. For example, DiVincenzo
calls for the qubits to be individually addressable in a quantum
computer. If we have, for example, a two-level system comprised of an
ensemble of atoms, but where the qubits are not individually
addressable, this system would fail the QC test. 2. Fidelity: While it
is tempting to focus on the horse race of the number of qubits of each
platform, we recommend first examining the claims made on the fidelity
of those qubits. Fidelity is a measure of the ability for a qubit to
remain in coherence through a computation; specifically it is calculated
as: 1 - the error rate. When presented with a system, it is useful to
examine the fidelity of the qubits under one and two-qubit operations.
Fidelity is harder to maintain when spanning two qubits with a CNOT, for
example, than when applying single-qubit operators such as X or Y . 3.
Scalability: Is the architecture scalable to 106 qubits and beyond?
While it is of some benefit to create NISQ-regime QCs across a multitude
of hardware frameworks at this stage, it is also important to examine
the ability to achieve a fault-tolerant platform in that architecture.
4. Qubits: Once the above questions are considered, we can turn to
numbers of qubits. Maintaining the simultaneous coherence of larger and
larger numbers of qubits is a technical challenge. Also, it is important
to look at architecture-specific limitations of the qubits, such as
nearestneighbor connections. In some platforms, for example, if we
operate on two adjacent qubits, we cannot make use of other adjacent
qubits at the same time due to potential crosstalk. 5. Circuit depth:
This refers to how many operations we can implement before coherence
breaks down. A 106 qubit computer would be wonderful, but if it cannot
implement more than a few operations before losing coherence it is of
limited value.

SECTION 5.2 Neutral Atoms

55

6.  Logical connectivity: Can we implement two-qubit gates on any pair
    of qubits, or only for certain pairs? Limited logical connectivity
    requires that logical SWAP operations be inserted into our
    algorithms to effectively simulate greater connectivity. More
    operators means more potential for noise and errors.
7.  Cloud access: Is the hardware easily made available over the cloud?
    It is unlikely that most organizations will purchase or build their
    own QCs. Instead, they will rely on a range of academic and
    commercial providers who will provide cloud access. Criteria to
    consider in this category include reset time between computations
    and labor required to keep the platform available to meet its
    service level agreement (SLA). With that introduction, let’s
    consider the leading QC architectures in alphabetical order. Please
    consult this book’s online site for links to additional papers and
    updates as they are posted. For additional background on the
    approaches outlined in this chapter, please see \[161\].

5.2

Neutral Atoms

Neutral atoms present an intriguing approach to quantum computing. While
trapped-ion research has been going on for some time, several labs have
more recently ramped up their ability to control ensembles of neutral
atoms. To implement a neutral atom system, engineers can set up four
laser beams around the atom ensemble to form a magneto-optical trap
(MOT). Labs typically use either cesium (Cs) or rubidium (Rb) atoms for
this work. By confining the atoms with this quadruple laser system, we
can cool the atoms down to mK temperatures. Now that we have hundreds of
millions of neutral atoms in a reservoir, we can transfer a small number
of them into an addressable array (see Figures 5.1 and 5.2). See \[141\]
for an in-depth discussion of neutral atom systems. The Lukin Lab at
Harvard has made good progress on neutral atom systems \[220, 169\]. In
their recent paper \[98\], the Lukin lab reports a number of
breakthroughs in their ability to control larger arrays of neutral
atoms. This could lead to faster scaling of high-fidelity qubits on this
platform. David Weiss and his group at Penn State have also focused on
neutral atom platforms and have demonstrated a Stern-Gerlach-inspired
neutral atom experiment \[290, 301\]. The group at Pascal in France have
been developing a neutral atom quantum computer and together with their
academic partner at IOGS have achieved a neutral atom QC of more than
100 qubits \[216\].

56

CHAPTER 5 Building a Quantum Computer

Figure 5.1: A. Diagram of addressing a 5  5  5 array of neutral atoms.
Each addressing beam can be parallel-translated within 5s to any line
of atoms, so that any site can be put at their intersection. The
addressing beams are circularly polarized, and the 140mG magnetic field
is in the same plane. B.) The relevant part of the ground state energy
level structure for addressing (not to scale) a target atom experiences
twice the AC Stark shift of any other atom (its shift is illustrated by
the orange dashed lines), so that, starting in the storage basis, j3; 0i
and j4; 0i, it alone is resonant with !1 . After it is transferred to
the computation basis, j3; 1i and j4; 1i, it alone is resonant with !2 .
Image and caption from \[290\]

IOGS has also demonstrated multiple atomic configurations for use in
neutral atom QCs \[28\]. Each of these configurations can lead to
different topologies optimized for different computational problems.
Neutral atom systems meet the DiVincenzo criteria for a quantum
computer: qubits are individually separable and addressable, they can
hold their state and we can perform a measurement on them. Saffman et
al. offers a good review of implementing gates on a neutral atom system
\[246\]. The challenge now is to scale such systems. See \[294\] \[141\]
for helpful reviews. For an example of programming for a neutral atom QC
see \[217\] which uses Pennylane and Cirq to code for the Pasqal neutral
atom QC.

5.3

NMR

Some of the first demonstrations of quantum computation made use of spin
qubits using nuclear magnetic resonance (NMR) devices. Chuang and
colleagues demonstrated the factoring of the number 15 using Shor’s
algorithm in a liquid-state NMR setup (LSNMR) \[278\]. While the number
15 is trivial to factor, it was one of the first demonstrations that
quantum principles could be used in a physically realizable system for
computation. Later, researchers ex-

SECTION 5.4 NV Center-in-Diamond

57

Figure 5.2: (a) Overview of the main hardware components constituting a
quantum processor. The trapping laser light (in red) is shaped by the
spatial light modulator (SLM) to produce multiple microtraps at the
focal plane of the lens (see inset). The moving tweezers (in purple),
dedicated to rearranging the atoms in the register, are controlled by a
2D acousto-optic laser beam deflector (AOD) and superimposed on the main
trapping beam with a polarizing beamsplitter (PBS). The fluorescence
light (in green) emitted by the atoms is split from the trapping laser
light by a dichroic mirror and collected onto a camera. (b) Photography
of the heart of a neutral-atom quantum co-processor. The register is
prepared at the center of this setup. Image and caption from \[141\]

perimented with solid state NMR (SSNMR) using nitrogen-vacancy centered
diamonds, which relates to another approach covered in this chapter.
While a number of researchers use NMR platforms to test various QC
phenomena, this platform is unlikely to scale for fault-tolerant quantum
computation. We will need millions of physical qubits (translating to
thousands of logical qubits) for such a device and NMR as currently
implemented becomes impractical at those scales.

5.4

NV Center-in-Diamond

In the nitrogen-vacancy (NV) center-in-diamond approach to QC, two
carbon atoms in the diamond lattice are missing, and one of them is
replaced with a nitrogen ion. The resulting system forms a paramagnetic
defect that can act as a qubit. The qubit state can be manipulated with
microwave fields and read out optically. A number of labs have
demonstrated basic NV systems \[248, 277, 70\]. Instead of doping with
nitrogen, several labs have doped with silicon \[143, 101\]. These and
other materials each have their own unique advantages and disadvantages
\[66, 157\]. For helpful reviews of NV approaches see \[73, 95, 305\].
Researchers are currently investigating the successful application of a
two-qubit operator on this platform (see \[172, 35, 219, 142\]).

58

CHAPTER 5 Building a Quantum Computer

Figure 5.3: NV diamond schematic

5.5

Source: \[305\]

Photonics

Photonics can also be used to construct a gate-based quantum computer
(see \[259\] for a review). Linear Optics Quantum Computing (LOQC) uses
linear optical elements (such as mirrors, beam splitters and phase
shifters) to process quantum information \[8, 155, 158\]. These optical
elements preserve the coherence of input light and hence equivalently
apply a unitary transformation on a finite number of qubits. However,
photons do not interact with each other in a vacuum. They can only
interact indirectly via another medium. In 2001, Knill, Laflamme and
Milburn (KLM) \[155\] presented a method of implementing scalable
quantum computing using single photons, linear optics, photodetection
and post-processing. These elements enable the application of nonlinear
operations solely with linear optical elements \[158\]. More recently,
the PsiQuantum group has described the Fusion-Based Quantum Computing
(FBQC) approach to LOQC \[29\]. PsiQuantum is focused on building a
faulttolerant photonic QC using this approach; they rely on silicon
photonics fabrication techniques as their method to scale to millions of
qubits. Another paradigm is the so-called one-way, measurement-based or
clusterstate quantum computer (MBQC) \[229, 230, 231, 232\] which first
prepares a highly entangled multi-particle cluster state. Then, in order
to implement a quantum circuit, one has to perform a sequence of
single-qubit projective measurements. Every subsequent measurement
choice is driven by the outcome of the previous measurement. The Xanadu
group of Canada has described their approach to MBQC \[276\]. Arbitrary
two-qubit processing requires the equivalent of three consecutive
entangling gates in the circuit model of quantum computing \[133\] which
is beyond the level of complexity that can be practically constructed
and maintained with free-space quantum optics \[185, 65\]. Photonic
chips can take advantage of the entire silicon-based infrastructure to
miniaturize LOQC and

SECTION 5.5 Photonics

59

Figure 5.4: Quantum circuits and a schematic of a silicon photonic chip
Source: \[227\]

bring down the cost \[255\]. Researchers from the University of Bristol,
together with researchers from China’s National University of Defense
Technology, have demonstrated a photonic quantum processor on a silicon
photonics chip. The processor generates two photonic qubits on which it
performs arbitrary two-qubit unitary operations, including arbitrary
entangling operations \[227\]. The quantum processor was fabricated with
mature Complementary Metal Oxide Semiconductor (CMOS) compatible
processing and comprises more than 200 photonic components; the
processor was programmed to implement 98 different two-qubit unitary
operations with an average quantum process fidelity of 93:2 ˙ 4:5%.
Semiconductor quantum transistor The lack of deterministic photon-photon
interactions is a challenge for quantum computation in this approach. To
deterministically control an optical signal with a single photon
requires strong interactions with quantum memory. Nanophotonic
structures coupled to quantum emitters may offer an attractive approach
to realize single-photon nonlinearities in a compact solid-state device.
Recently, there has been great progress in controlling photons with
solid-state qubits \[16, 258, 38\], as well as controlling a solid-state
qubit with a photon \[267\]. Arazolla et al. demonstrated a programmable
optical chip for QC using optical squeezed states \[17\]. Researchers at
the University of Maryland and the Joint Quantum Institute have realized
the first single-photon switch and transistor enabled by solid-state
quantum memory using a semiconductor chip \[266\]. The device

60

CHAPTER 5 Building a Quantum Computer

allows one photon to switch other photons, and hence to produce strong
and controlled photon-photon interactions. It consists of a spin qubit
strongly coupled to a nanophotonic cavity (an idea first proposed by
Duan and Kimble \[96\]). They combined a semiconductor membrane with
quantum dots; together they sit in the middle of the array. The array
forms a photonic crystal, which uses the Bragg reflection mechanism
where light bounces around a trap. That allows the quantum dot to store
the information about the photon with a single electron, which has spin
properties. By using this transistor, they should be able to apply
quantum gates to photons. A scalable device suitable for quantum
information processing will require higher efficiencies, as photon loss
constitutes a dominant error source for photonic qubits. Topological
photonic chip Topological insulators are exotic materials which insulate
in their bulk but conduct on their surface \[137, 226\]. These states
exhibit remarkable properties such as unidirectional propagation and
robustness to noise. Since the discovery of these phases of matter,
several topological effects have been observed using integrated
photonics \[179, 213, 304, 291, 131, 233, 132, 40, 197, 303, 69, 208,
171, 160, 280, 279, 310, 41, 198\]. Topological photonics is a promising
option for scalable quantum computers since they have the advantage of
not requiring strong magnetic fields and feature intrinsically
high-coherence, room-temperature operation and easy manipulation.
Recently, scientists from RMIT University, Australia, in collaboration
with researchers from the Politecnico di Milano and ETH Zurich, have
developed a topological photonic chip that encodes, processes and
transfers quantum information at a distance \[270\]. They have used
photonic chips to demonstrate that topological states can undergo
quantum interference by replicating the well known Hong-Ou-Mandel (HOM)
experiment with 93.1 ˙ 2.8% visibility \[145\].

5.6

Spin Qubits

Silicon-based spin-qubit technology represents another approach to
quantum computation. If we could construct qubits from common
semiconductor materials, we could scale such a system by leveraging the
decades of know-how in the integrated chip industry. It is difficult,
however, to develop a stable, addressable qubit on the standard CMOS
platform. Initial prototypes have been demonstrated, but it has been
challenging to stabilize these qubits for scale-up.

SECTION 5.7 Superconducting Qubits

Figure 5.5: Spin qubit experimental system

61

Source: \[188\]

In these early attempts, a pair of quantum dots is placed between the
source and sink in a traditional CMOS setup on a silicon semiconductor
substrate. The entire device is placed in a dilution fridge to bring it
down to about 1K; this is much warmer than the temperature needed for
superconducting qubits. Microwave pulses are then used to apply unitary
operators to the qubits \[292\]. Intel, HRL Laboratories, as well as
labs at the University of Cambridge, Delft University of Technology,
Harvard, and the University of New South Wales (UNSW) are working on
silicon-based spin qubit approaches.

5.7

Superconducting Qubits

Several groups are building quantum computers with superconducting
qubits. The core design is based on a qubit made from a Cooper pair with
a Josephson junction \[51\]. Microwave leads are attached to the qubit
to control it. By sending specific pulses of microwave frequencies for
controlled amounts of time into the physical qubit, the user can apply
the range of unitary operators. The entire apparatus must be cooled
below 10mK to operate. The system is also shielded from magnetic fields
and other factors that could cause decoherence.

62

CHAPTER 5 Building a Quantum Computer

Figure 5.6: Classical CPU controlling a superconducting quantum
computer. The red circle denotes the area within the dilution fridge for
the quantum processor. In more recent implementations the temperature in
this area is brought down below 10mK. See Figure 5.7 for images of
various superconducting quantum processors Source: \[215\]

Figure 5.7: Superconducting processors (l to r): Google, IBM, Rigetti
\[164\], \[274\]

Source (l to r): Google,

The NAS report summarizes the various types of superconducting qubits
\[204, page C-1\]: Fixed-frequency versus tunable qubits:
Frequencytunable qubits can be calibrated and corrected for qubit
frequency variations that arise from variations in the fabrication
process or as a result of device aging. An advantage is that one
microwave tone can control multiple qubits, a savings in hardware.
Gaining this advantage requires an additional control signal to adjust
the frequency and adds an additional path for noise to enter the qubit.
The two most common qubits in use today for digital superconducting
quantum computing are the “transmon qubit”, which comes in
single-junction nontunable and two-junction tunable forms, and the “flux

SECTION 5.8 Topological Quantum Computation

63

qubit.”...Both transmon designs are being used in leading edge efforts.
Static versus tunable coupling: Static coupling between qubits — for
example, by using a capacitor or an inductor to mediate interaction — is
an “always-on” coupling that is fixed by design. The coupling is turned
“on” by bringing two qubits into resonance, and it is turned off by
detuning the qubits. Yet even in the off state, there still is a small
residual coupling. This tuning can be further reduced by adding a third
object — either another coupler qubit or a resonator — between the two
qubits. The two qubits are then coupled by adjusting the qubits and the
resonator to the proper frequency. A number of groups are working on
superconducting qubit quantum computers including: Google, IBM, Rigetti,
QCI and others (see Figure 5.7) and \[211, 242\]. Check this book’s
GitHub site for updated information in this area. See \[154\] and
\[159\] for helpful reviews of this approach.

5.8

Topological Quantum Computation

Topological quantum computing (TQC) attempts to take advantage of the
unique properties of anyons. An anyon is a 2-dimensional quasiparticle
which is neither a boson (such as a photon) nor a fermion (such as an
electron). By braiding the pathways of an anyon in 4D spacetime, one can
theoretically create a system for quantum computation which is robust to
decohering effects (see Figure 5.8). This is due to the braided nature
of the system — even if there are a series of small perturbations to the
system, the topology of the system does not change, and therefore it
stays coherent and quantum computation can continue. See Roy and
DiVincenzo for more background on this approach \[245\]. Alexei Kitaev,
then of the Landau Institute of Theoretical Physics, first proposed the
idea of TQC \[153\]. Freedman, Kitaev, et al. then demonstrated that
such a topological computer would be Turing complete \[119\]. Freedman
and others then launched a program at Microsoft to investigate the
physical realization of a topological quantum computer. For useful
surveys of this approach, see \[162\] and \[207\]. See \[244\] for an
overview of the mathematics of topological computing and see \[269\] for
discussion of a gate implementation in a TQC setting.

64

CHAPTER 5 Building a Quantum Computer

Figure 5.8: Braided anyons for topological computing

5.9

Source: \[244\]

Trapped Ion

In the trapped-ion approach, ytterbium atoms (or another element) are
ionized with lasers and trapped in electric potentials to form a line of
qubits. An additional laser is then used to measure the state of the
qubits. Proponents of trapped-ion systems point to the ability Source:
\[300\] to run their systems without having to cool it to mK ranges
which is a requirement of hardware realizations such as superconducting
qubits. Cirac and Zoller did early work in this field \[79\]. Chris
Monroe of the University of Maryland, College Park and Jungsang Kim of
Duke University have been active in this space and reported on several
advances \[14, 25\]. Other groups include those at NIST \[44\], Oxford
\[180\], Innsbruck \[121\], MIT \[168\] and ETH \[115\]. Pino et al.
have demonstrated an ion trap QC using their quantum charged-coupled
device (QCCD) approach \[221\]. Figure 5.9 details two types of qubits
that can be realized in a trapped ion system: optical qubits and
hyperfine qubits. Optical qubits leverage the difference in energy
levels between ground and metastable states; hyperfine qubits
distinguish between two different ground states. See \[63\] and \[204\]
for helpful reviews of the trapped-ion approach.

SECTION 5.10 Summary

65

Figure 5.9: Qubits in an atomic ion. (a) An optical qubit consists of
one of the atomic ground states and one of the metastable excited
states, separated by approx. 1014 to 1015 H z. (b) A hyperfine qubit
consists of two of the ground states, separated by approx. 109 to 1010 H
z. Usually some excited states are used to support qubit manipulation
operations. In both cases, there are other (auxiliary) states in the
ground, excited and metastable excited states than those chosen to
represent the qubit. Source: \[204, Appendix B\]

5.10

Summary

Figure 5.10: Quantum computing roadmap

Source: Google

Researchers are pursuing a range of architectures in the quest for a
faulttolerant, scaled universal quantum computer. This period in quantum
computing hardware is probably most akin to the 1940s and 1950s in
classical computing. Research groups today are still figuring out which
architecture will scale and to understand the kinds of problems which
can be addressed with these platforms. Quantum hardware development is
likely to move at

66

CHAPTER 5 Building a Quantum Computer

a faster pace as we have the benefit of a global community of academic
and commercial researchers forging ahead. Figure 5.10 indicates that we
are in the NISQ era of 102 to 103 qubits. We aim to reach &gt;106 qubits
in order to build a fully error-corrected quantum computer. Current
quantum error correction techniques require about 1,000 physical qubits
for every logical qubit. Since at least a few thousand logical qubits
are needed for Shor’s and other important algorithms, we will have to be
in the 106 to 107 regime to realize this goal. Now that we have surveyed
the various approaches to quantum computing hardware, let us turn to the
QC development platforms and software.

CHAPTER

6 Development Libraries for Quantum Computer Programming With the
growing interest in quantum computing, there are an increasing number of
development libraries and tools for the field. There are development
environments and quantum circuit simulators in all the major languages
including Python, C/C++, Java and others. A comprehensive list can be
found on this book’s website. Many of the leading QC research centers
have focused on Python as the language of choice for building quantum
circuits. One of the reasons for choosing Python is that it is a
flexible, high-level language that allows programmers to focus on the
problem being solved without worrying about too many formal details. For
example, Python is dynamically typed (meaning variable types do not have
to be declared by the programmer) and is an interpreted language
(meaning it does not have to be pre-compiled into a binary executable).
For these reasons and others, Python has a relatively easy learning
curve for new users and has already seen strong support from the QC
community. In this chapter, we will provide an overview of how these
libraries work and provide code examples for each framework. In the
upcoming chapters, we will go into further detail with examples of
algorithm implementations using these libraries. These quantum
development libraries have methods for all the major unary and binary
operators that we cover in this book. A few offer built-in modules for
ternary operators, but these can be constructed if not offered in the
library. © The Author(s), under exclusive license to Springer Nature
Switzerland AG 2021 J. D. Hidary, Quantum Computing: An Applied
Approach, https://doi.org/10.1007/978-3-030-83274-2\_6

67

68

CHAPTER 6 Development Libraries for Quantum Computer Programming

Figure 6.1: Quantum computing stack

Source: \[123\]

Figure 6.1 shows a schematic diagram of the quantum computing stack,
which ranges from quantum algorithms and applications at the highest
level to physical realizations of quantum computers at the lowest level.
Numerous components sit between these layers such as control, readout,
and — in the future — quantum error correction modules. Quantum
programming languages (QPL) are used to interface with the top of the
stack \[165\]. A quantum language consists of low-level instructions
indicating which gates to perform on which qubits. Since it would be
very tedious to program this by hand, when we program quantum computers,
we interface with the higher-level quantum programming language in a
development library. Many QPLs are now available including both
functional and imperative languages. The functional set includes:
Qiskit, LIQUiji, Q\# and Quipper. Imperative languages for QC
programming include: Cirq, Scaffold and ProjectQ. See \[114\] for a
helpful review of open source frameworks for quantum computing. See
\[13\] for an overview of the quantum computing stack.

6.1

Quantum Computers and QC Simulators

Cloud quantum computers make it possible to run algorithms on real
quantum hardware, and development libraries enable this capability. In
order to test code prior to running it on a quantum computer, most QC
frameworks provide a QC simulator which runs on a classical computer.
This simulator can run locally or in the cloud. Since it is running on a
classical computer, it cannot, of

SECTION 6.1 Quantum Computers and QC Simulators

69

course, process actual quantum states, but it is helpful to test the
code syntax and flow. There are numerous techniques to classically
simulate quantum circuits, all of which suffer from the “exponential
explosion” of classical memory: to store the most general state of an n
qubit system, all 2n complex numbers of the system’s wavefunction must
be stored. How much memory does this require? For simplicity, suppose
that each complex number is stored using one byte. Then, for n D 30
qubits, 230 bytes, or a gigabyte, of memory is required. For n D 40, a
terabyte of memory is required, and for just n D 50, a petabyte is
required. These memory requirements are already reaching the limits of
today’s best supercomputers, even for a modest number of qubits. Larger
systems cannot hope to be simulated, since we wouldn’t even have enough
memory to write the wavefunction down! The most basic method for
simulating a quantum computer is to note that a quantum circuit simply
expresses a unitary transformation, U , on a wavefunction, j i. The QC
simulator algorithm then just performs matrix multiplication to get the
resulting state j 0 i via j

0

iDUj i

Note that this method requires storing the entire unitary of the
circuit, which is a 2n  2n matrix, in memory (in addition to storing
the wavefunction). A method that improves on these memory requirements,
only having to store the wavefunction itself, works by applying one- and
two-qubit gates to the wavefunction individually. To apply a
single-qubit gate   G11 G12 GD G21 G22 to the i th qubit, one applies
a matrix product to each amplitude ˛ whose index differs in the i th bit
\[120, 260\] ˛0i  D G11 ˛0i  C G12 ˛1i 
˛1i  D G21 ˛0i  C G22 ˛1i  Here, the
subscript i on either 0 or 1 denotes that this index is in the i th
position, and asterisks denote indices that are the same on either side
of the equation. A similar update equation exists for two-qubit gates.
The algorithm for this “state vector” or “wavefunction” simulator then
consists of iterating through all single-qubit and two-qubit gates in
the circuit and applying the appropriate update equation.

70

CHAPTER 6 Development Libraries for Quantum Computer Programming

Other types of QC simulators exist, such as Clifford circuit simulators,
which can efficiently simulate several hundreds or thousands of qubits.
However, as discussed in chapter 3, these circuits are not universal. In
this chapter, we focus on programming universal QCs and QC simulators.
When a program is sent to a quantum backend, it is first compiled into
gates the computer can actually implement. This compilation is expressed
in a lower level language — quantum assembly or instruction language —
which is sent to the computer. At the lowest level, gates are
implemented by physical operations acting on the qubits. These physical
operations can include microwave pulses, laser pulses or other
interactions acting on a qubit, depending on which physical realization
of a qubit is used.

6.2

Cirq Cirq Overview Institution First Release Open Source? License Github
Documentation OS Classical Language

Google v0.1 on April 17, 2018 Yes Apache-2.0
https://github.com/quantumlib/Cirq
https://cirq.readthedocs.io/en/stable/ Mac, Windows, Linux Python

Figure 6.2: Overview of the Cirq dev library. Modified with permission
from \[165\].

Cirq is Google’s quantum computing development library. Cirq enables the
developer to build and execute quantum circuits comprised of all the
usual unary, binary and ternary operators we have covered in this book.
We will use Cirq for the majority of code examples throughout this book.
Source:\[80\] To get acquainted with the language, a sample program in
Cirq is provided below \[80\]. This program creates a quantum circuit
with one qubit and performs the NOT operator on it followed

SECTION 6.2 Cirq

71

by a measurement. This circuit is simulated several times and its
measurement outcomes are displayed to the console. The full program is
shown below.1 """Simple program in Cirq.""" \# Import the Cirq package
import cirq \# Pick a qubit qubit = cirq.GridQubit(0, 0) \# Create a
circuit circuit = cirq.Circuit( cirq.X(qubit), \# NOT.
cirq.measure(qubit, key=’m’) \# Measurement ) \# Display the circuit
print("Circuit:") print(circuit) \# Get a simulator to execute the
circuit simulator = cirq.Simulator() \# Simulate the circuit several
times result = simulator.run(circuit, repetitions=10) \# Print the
results print("Results:") print(result)

In this circuit, we first set up a qubit within a grid pattern. Cirq
also allows qubits to be set up in a linear fashion if needed, since
both linear and two-dimensional qubit arrays are the most popular for
near-term quantum computer architectures. We then apply the NOT operator
to the qubit. If the qubit was in a state of j0i before, it will now be
in the state j1i and vice-versa. We then measure the qubit to output the
classical bit of the measurement result. Note that the keyword argument
key=’m’ in the measure operation makes it easy to access measurement
results using the histogram method of a Cirq TrialResult. In this simple
program, it is not necessary, but in more complex programs it can be a
useful tool. The next lines of code get a QC simulator and execute the
circuit ten times. Then, the results of executing the circuit are
printed to the screen. A sample output from this program is shown below.

1 To find versions of each program shown in this chapter for the latest
releases of each development library, see the book’s GitHub page.

72

CHAPTER 6 Development Libraries for Quantum Computer Programming

Figure 6.3: The Bloch sphere

Source: \[122\]

Circuit: (0, 0): ---X---M(’m’)--Results: m=1111111111

The circuit is printed out in ASCII text, as is standard for drawing
circuits in Cirq, and the results are indicated by a sequence of binary
digits. As we anticipate, on a noiseless QC simulator all measurement
outcomes are equal to 1. Finally, note that the string of measurement
outcomes is labeled by the measurement key m provided as a keyword
argument to the measure operation. We can represent the application of
the X operator in this circuit on a Bloch sphere (see Figure 6.3). We
recall that the Bloch sphere represents the computational basis states
of j0i and j1i at the poles. By applying the X gate to the prepared
state of j0i we move the qubit to state j1i. If we then apply a Hadamard
gate, we can represent the new qubit state with a horizontal vector on
the Bloch sphere corresponding to: j0i j1i p 2 For circuits of many
operators we can use dynamic Bloch sphere simulation software from
Q-Ctrl (and other sites listed on the companion website) to visualize
the unitary transformations.

6.3

Qiskit

The Quantum Information Science Kit, or Qiskit for short, is a quantum
computing dev library created by IBM. The Qiskit library is a flexible
frame-

SECTION 6.3 Qiskit

73

Qiskit Overview Institution IBM First Release 0.1 on March 7, 2017 Open
Source? Yes License Apache-2.0 Homepage https://qiskit.org/ Github
https://github.com/Qiskit Documentation
https://qiskit.org/documentation/ OS Mac, Windows, Linux Classical Host
Language Python Quantum Language OpenQASM Figure 6.4: Overview of the
Qiskit development library. Modified with permission from \[165\].

work for programming quantum computers. The Qiskit development library
consists of four core modules distributed across the quantum computing
stack:  Qiskit Terra: Terra provides core elements for composing
quantum programs at the level of circuits and pulses, and optimizing
them for the constraints of a particular physical quantum processor. 
Qiskit Aer: Aer provides a C++ simulator framework and tools for
constructing noise models for performing realistic noisy simulations of
the errors that occur during execution on real devices.  Qiskit Ignis:
Ignis is a framework for understanding and mitigating noise in quantum
circuits and devices.  Qiskit Aqua: Aqua contains a library of
cross-domain quantum algorithms upon which applications for near-term
quantum computing can be built. Except for Aqua, at the time of writing,
each of these components is installed automatically with Qiskit. The
Aqua module can be installed separately and requires a working
installation of the core Qiskit library. To demonstrate the coding
syntax in Qiskit, we include below the same example program that was
shown previously in Cirq. """Simple program in Qiskit.""" \# Import the
Qiskit package import qiskit \# Create a quantum register with one qubit
qreg = qiskit.QuantumRegister(1, name=’qreg’) \# Create a classical
register with one qubit creg = qiskit.ClassicalRegister(1, name=’creg’)

74

CHAPTER 6 Development Libraries for Quantum Computer Programming

Figure 6.5: Circuit diagram drawn in Qiskit for the above program

Create a quantum circuit with the above registers
=================================================

circ = qiskit.QuantumCircuit(qreg, creg) \# Add a NOT operation on the
qubit circ.x(qreg\[0\]) \# Add a measurement on the qubit
circ.measure(qreg, creg) \# Print the circuit print(circ.draw()) \# Get
a backend to run on backend =
qiskit.BasicAer.get\_backend("qasm\_simulator") \# Execute the circuit
on the backend and get the measurement results job =
qiskit.execute(circ, backend, shots=10) result = job.result() \# Print
the measurement results print(result.get\_counts())

This program in Qiskit closely mirrors that in Cirq, with minor
differences due to language design, syntax and notation. After importing
the Qiskit development library, the program declares a quantum and
classical register with one qubit, which it then uses to create a
circuit. Note how this is different from Cirq, in which (1) a classical
register is never explicitly created and (2) qubits are only referred to
in a circuit when operations are added. Continuing through the Qiskit
program, the next lines add the appropriate operations (NOT and measure)
to the circuit, which is subsequently printed out by drawing the
circuit. Qiskit has the ability to draw and save circuits as files in
addition to printing out text representations. Figure 6.5 shows the
circuit for this program drawn with the code shown below:
circ.draw(filename="qiskit-circuit", output="latex")

After printing the circuit, a backend is declared for executing the
quantum circuit. In the final lines, the circuit is executed, the
results are retrieved, and finally the measurement statistics (counts)
are printed to the screen. An

SECTION 6.4 Forest

75

example output of this program is shown below. Note that the circuit
will also be printed to the console in the above program — we omit the
text representation here. {’1’: 10}

In Qiskit, measurement outcomes are stored as dictionaries (a Python
data type consisting of key-value pairs) where keys are bit strings and
values are the number of times each bit string was measured. Here, this
output says that the only bit string present in the measurement is 1.
Similar to the Cirq output, since we are running this program on a QC
simulator without activating a noise model, all measurement outcomes are
1 as expected.

6.4

Forest

Forest Overview Institution Rigetti First Release v0.0.2 on Jan 15, 2017
Open Source? Yes License Apache-2.0 Homepage
https://www.rigetti.com/forest GitHub https://github.com/rigetti/pyquil
Documentation pyquil.readthedocs.io/en/latest/ OS Mac, Windows, Linux
Classical Language Python Quantum Programming Library pyQuil Quantum
Language Quil Figure 6.6: Overview of the Forest development library.
Modified with permission from \[165\].

Forest is a development library by Rigetti. Similar to the previous two
libraries, Forest is Python-based and features a collection of tools for
effective quantum programming. Users type quantum programs in pyQuil,
and lowlevel instructions are sent to the quantum computer as Quil,
short for Quantum Instruction Language \[261\]. The name Forest refers
to the collection of all programming tools in this toolchain including
Quil, pyQuil and other components such as Grove, a collection of quantum
algorithms written in pyQuil. To get a sense for the language we
implement the “NOT and measure” program in pyQuil below.

76

CHAPTER 6 Development Libraries for Quantum Computer Programming

"""Simple program in pyQuil.""" \# Import the pyQuil library import
pyquil \# Create a quantum program prog = pyquil.Program() \# Declare a
classical register creg = prog.declare("ro", memory\_type="BIT",
memory\_size=1) \# Add a NOT operation and measurement on a qubit prog
+= \[ pyquil.gates.X(0), pyquil.gates.MEASURE(0, creg\[0\])\] \# Print
the program print("Program:") print(prog) \# Get a quantum computer to
run on computer = pyquil.get\_qc("1q-qvm") \# Simulate the program many
times prog.wrap\_in\_numshots\_loop(10) \# Execute the program on the
computer. NOTE: This requires the QVM to be running result =
computer.run(prog) \# Print the results print(result)

Here, we first import the pyQuil library and then create a program, the
equivalent of a circuit in Cirq or Qiskit. After creating the program,
we declare a classical register of one bit, then add the operations for
this circuit — NOT and measure. Note that qubits can be indexed
dynamically in pyQuil; there is no explicit reference to a qubit
register, but rather we provide an index (0) to the gate operations. In
contrast, classical memory does have to be explicitly declared, and so
we measure the qubit into a classical register. After printing out the
program to visualize its instructions, we send the instructions to a QC
for execution. Here, the string key designates that we want a one qubit
(1q) quantum virtual machine (qvm), which is Rigetti’s terminology for
their quantum computer simulator. To simulate the program many times, we
call the method wrap\_in\_numshots\_loop on the program, and provide as
input a number of repetitions (shots). Finally, we run the program on
the specified computer and print the result. To execute this

SECTION 6.5 Quantum Development Kit

77

program on the quantum virtual machine, we can initiate the QVM with the
following command in a terminal: qvm -S

Once executed in the QVM, the program will produce and the following
results: Program: DECLARE ro BIT\[1\] X 0 MEASURE 0 ro\[0\] Result:
\[\[1\]\[1\] \[1\]\[1\] \[1\]\[1\] \[1\]\[1\] \[1\]\[1\]\]

Unlike Cirq and Qiskit, pyQuil does not produce a circuit diagram of the
program, but rather displays the Quil instructions line by line. In this
particular Quil program, a readout register called ro is declared, a NOT
operation is applied to qubit 0, and the measurement outcome of qubit 0
is stored into the readout register. The results of simulating the
circuit appears as a list of lists. Each inner list is the measurement
outcome for a particular execution of the circuit. The number of inner
lists is equal to the total number of times the circuit was executed.
All of these are wrapped in an outer list containing the results of all
simulations. As with the previous programs, all measurement outcomes are
1 on a noiseless quantum computer simulator, as we expect.

6.5

Quantum Development Kit

The Quantum Development Kit (QDK) is a quantum computing development
library by Microsoft. Unlike the previous languages, which were based in
Python, the QDK contains its own language, called Q\# (pronounced “Q
sharp”), for writing quantum programs. The Q\# language is different in
several respects compared with Pythonbased libraries such as Cirq,
Qiskit and pyQuil. In Q\# we need to explicitly

78

CHAPTER 6 Development Libraries for Quantum Computer Programming

Institution First Release Open Source? License Homepage Github
Documentation OS Quantum Prog. Lang.

QDK Overview Microsoft 0.1.1712.901 on Jan 4, 2018 Yes MIT
microsoft.com/en-us/quantum/development-kit

https://github.com/Microsoft/Quantum
docs.microsoft.com/en-us/quantum/?view=qsharp-preview

Mac, Windows, Linux Q\#

Figure 6.7: Overview of the QDK development library. Modified with
permission from \[165\].

declare types, as well as use curly braces instead of indents as in
Python. Additionally, three separate files are required to execute
programs using the QDK: 1. A file ending in .qs where quantum operations
(analogues of functions in Python) are stored 2. A driver file ending in
.cs where quantum operations are executed in the main program 3. A file
ending in .csproj which defines the project and contains metadata about
computer architecture and package references An example program in Q\#
that executes the same “NOT and measure” circuit we have seen in other
languages is included below. We first show the .qs file which defines
the quantum operations we will use in the driver file. namespace
Quantum.Simple { // Importing the libraries open
Microsoft.Quantum.Primitive; open Microsoft.Quantum.Canon; // Sets a
qubit in a desired state operation Set(desired\_state: Result, qubit:
Qubit) : Unit { let current = M(qubit); if (current != desired\_state) {
X(qubit); } } // Executes the NOTandMeasure circuit for an input number
// of repetitions and returns the number of ones measured operation
NotAndMeasure(repetitions: Int) : Int { // Variable to store the number
of measured ones mutable num\_ones = 0;

SECTION 6.5 Quantum Development Kit

79

// Get a qubit to use using (qubit = Qubit()) { // Loop over the desired
number of repetitions for (test in 1..repetitions) { // Get a qubit in
the zero state Set(Zero, qubit); // Perform a NOT operation X(qubit); //
Measure the qubit let res = M (qubit); // Keep track of the number of
ones we measured if (res == One) { set num\_ones = num\_ones + 1; } } //
"Released qubits" must be in the zero state to avoid a
System.AggregateException Set(Zero, qubit); } // Return the number of
ones measured return num\_ones; } }

In the first line we define a namespace for the operations. This
namespace is used in the driver file to access these operations. The
next two lines are the equivalent of import packages in Python — they
make operations defined in the QDK available for us to use in the
program (e.g., the X gate). Next, we declare an operation called Set
which inputs a desired computational basis state and an arbitrary qubit
state; it then changes the state of the qubit to match the desired
state. This is accomplished by measuring the qubit in the computational
basis and then performing a NOT operation if necessary. We then define
the NotAndMeasure operation which sets up the quantum circuit and
measures the qubit for a user-specified number of times. Explicitly, the
operation sets a qubit to be in the 0 state using the previous operation
we defined, performs a NOT operation, then measures, keeping track of
the number of 1s measured. After the total number of repetitions, the
number of 1s measured is returned. In order to use this file, we must
define a separate driver file ending in .cs which executes these
operations. The driver file used to execute this program is shown below.
using System; using Microsoft.Quantum.Simulation.Core; using
Microsoft.Quantum.Simulation.Simulators;

80

CHAPTER 6 Development Libraries for Quantum Computer Programming

namespace Quantum.Simple { class Driver { static void Main() { // Get a
quantum computer simulator using (var qsim = new QuantumSimulator()) {
// Run the operation NotAndMeasure and get the result var num\_ones =
NotAndMeasure.Run(qsim, 10).Result; // Print the measurement outcome to
the console System.Console.WriteLine( \$"Number of ones measured:
{num\_ones, 0}."); } } } }

Here, we import System, which allows us to print to the console, and the
necessary tools to use the QC simulator in the QDK. Next, we invoke the
namespace declared in the .qs file above and define a Main function
inside the driver class. This Main function uses a QC simulator to run
the NotAndMeasure operation, then prints the results to the console. The
output of this program is shown below. Number of ones measured: 10.

As in other languages, we obtain the correct output of measuring all
ones. The final file .csproj needed to execute this code is included on
this book’s GitHub site. We omit the program here since it is nearly
identical for each project in the QDK.

6.6

Dev Libraries Summary

In the sample programs shown for these libraries, we have seen that most
frameworks are fairly similar in terms of constructing quantum circuits.
The general recipe for each of them is: 1. Build a quantum circuit
consisting of quantum and/or classical registers 2. Add operations to
the circuit 3. Simulate the circuit However, there are some differences
across the various libraries. For example, qubits are defined separately
from a quantum circuit in Cirq, whereas qubits are required as input to
a quantum circuit in Qiskit. Similarly, all qubits must be allocated in
a quantum register before performing operations on them

SECTION 6.6 Dev Libraries Summary

81

in Qiskit, but qubits can be allocated dynamically when programming in
pyQuil. While these differences may seem small, there are bigger
differences in the features each development library contains. For
example, some libraries include the ability to simulate noise, compile
algorithms to arbitrary architectures, access the wavefunction for
debugging and so on. These differences lead to certain algorithms being
easier to implement in particular libraries. While one development
library is usually sufficient for most tasks, having experience in
multiple libraries is helpful to choose the the appropriate library for
certain cases.

Using the Libraries In the remainder of the book, we will use these
development libraries to explore the core algorithms that make up the
canon of quantum computing and more recent QC methods. While Cirq is the
main library used, some programs are shown in other libraries for
comparison. Before continuing on to this core part of the text, we
briefly mention other development libraries that we have not yet
covered.

Other Development Libraries As mentioned, before the emergence of cloud
quantum computing, many quantum computer simulators were developed in
languages ranging from C++ (e.g., Quantum++) to Java (e.g., jSQ) to Rust
(e.g., QCGPU). A full list of quantum computer simulators is available
at https://quantiki.org/wiki/list-qcsimulators. While many of these
simulators are outdated or deprecated, a number of them are still
actively developed and being improved upon. Indeed, while classical
algorithms for simulating quantum circuits are widely believed to be
intractable, finding new ways to simulate more qubits with greater speed
is still an active area of research. In addition to the libraries above,
here are other libraries of interest: ProjectQ, a Python library with a
high-performance C++ quantum computer simulator; Strawberry Fields, a
Python library built around continuous variable quantum computing; and
Ocean, a Python library for quantum annealing on D-Wave quantum
computers. Additionally, a hardware independent quantum programming
framework called XACC is also actively being developed, as is a library
for simulating quantum circuits on Tensor Processing Units (TPUs) called
Floq \[297\]. Libraries for pulse-level control of superconducting qubit
computers have recently emerged, for example Qiskit Pulse and Quil-T,

82

CHAPTER 6 Development Libraries for Quantum Computer Programming

and a library for designing superconducting qubits called Qiskit Metal
has recently been introduced. Several domain-specific libraries have
also recently emerged. For example, Google’s open-source quantum
computing software includes OpenFermion, a library for quantum
chemistry; qsim, a high-performance classical simulator; and
TensorFlow-Quantum, a library for quantum machine learning. Other
researchers have developed additional quantum machine learning
libraries, for example Pennylane by the company Xanadu and Qiskit Aqua
by IBM. Finally, we mention a few notable cloud-level access providers
(i.e., institutions which allow users to execute quantum circuits on
real hardware over the cloud). IBM Quantum has several superconducting
qubit computers available for the public to use, with additional
privileges given to researchers in the field. Amazon Web Services (AWS)
allows users to execute circuits on trapped ion and superconducting
quantum computers as well as quantum annealers in a paid service.
Microsoft’s Azure Quantum provides access to trapped ion quantum
computers in a similar model. We expect current cloud-level access
providers to expand the types of quantum computing architectures they
support in the coming years. We also expect additional providers to
emerge. For a full list of open-source quantum software projects, see
the companion website to this book.

6.7

Additional Quantum Programs

In principle, knowing how to program circuits, simulate them and access
measurement results are the core skills needed for coding quantum
algorithms in future chapters. While the simple “NOT and measure”
program contains these three key features, it is nonetheless too
rudimentary to prepare us for further algo work. To help bridge this gap
to the more complex programs to come, we include two additional example
quantum programs in this section.

Bell States One common circuit pattern is the set of operators we use to
prepare one of the four Bell states 1 jˆC i D p Œj00i C j11i 2 from the
ground state. It can be easily verified that such a circuit consists of
a Hadamard on the first qubit and then a CNOT between the two qubits,
where the first qubit is the control qubit. This structure appears, for
example, in the

SECTION 6.7 Additional Quantum Programs

83

quantum teleportation circuit for creating entangled pairs of qubits
between two parties. A circuit for preparing a Bell state, written in
Cirq, is shown below. For pedagogical purposes, we add measurements
after the Bell state preparation circuit to see the possible measurement
outcomes. """Script for preparing the Bell state |\Phi\^{+}&gt; in
Cirq.""" \# Import the Cirq library import cirq \# Get qubits and
circuit qreg = \[cirq.LineQubit(x) for x in range(2)\] circ =
cirq.Circuit() \# Add the Bell state preparation circuit
circ.append(\[cirq.H(qreg\[0\]), cirq.CNOT(qreg\[0\], qreg\[1\])\]) \#
Display the circuit print("Circuit") print(circ) \# Add measurements
circ.append(cirq.measure(\*qreg, key="z")) \# Simulate the circuit sim =
cirq.Simulator() res = sim.run(circ, repetitions=100) \# Display the
outcomes print("\nMeasurements:") print(res.histogram(key="z"))

Note that in this Cirq program, we utilize the measurement key to access
measurement outcomes using the histogram method. An example output of
this program is shown below: Circuit 0: ---H---@--| 1:
-------X--Measurements: Counter({3: 53, 0: 47})

Here, the circuit drawing shows the Bell state preparation circuit
consisting of a Hadamard and CNOT gate. After, the measurement outcomes
enumerate how many 0 and 3 states were measured. Note that this is a
binary representation of bitstrings — i.e., 0 stands for 00 and 3 stands
for 11. As expected, these are the only two measurement outcomes in the
program, meaning that

84

CHAPTER 6 Development Libraries for Quantum Computer Programming

the measurements are perfectly correlated: when one qubit is measured
0.1/, the other qubit is always measured 0.1/.

Gates with Parameters Several quantum gates are defined in terms of
angles, for example the standard rotation gates Rx ./, Ry ./ and Rz
./. In many quantum algorithms, known as variational quantum
algorithms, these angles, or parameters, are iteratively adjusted in
order to minimize cost. For example, in the variational quantum
eigensolver, gate parameters are adjusted in order to minimize the
expectation of a Hamiltonian h ./jH j ./i. Regardless of the
application, such variational quantum algorithms depend critically on
the ability to update and change gate parameters. Because of this, most
quantum computing development libraries contain built-in features and
methods for working with parameterized gates. In the following program,
we demonstrate this functionality in Cirq. In particular, we set up a
simple quantum circuit with one parameterized gate, execute the
algorithm for a sweep of parameters and plot the measurement results.
"""Working with parameterized gates in Cirq.""" \# Imports import
matplotlib.pyplot as plt import sympy import cirq \# Get a qubit and a
circuit qbit = cirq.LineQubit(0) circ = cirq.Circuit() \# Get a symbol
symbol = sympy.Symbol("t") \# Add a parameterized gate
circ.append(cirq.XPowGate(exponent=symbol)(qbit)) \# Measure
circ.append(cirq.measure(qbit, key="z")) \# Display the circuit
print("Circuit:") print(circ) \# Get a sweep over parameter values sweep
= cirq.Linspace(key=symbol.name, start=0.0, stop=2.0, length=100) \#
Execute the circuit for all values in the sweep sim = cirq.Simulator()

SECTION 6.7 Additional Quantum Programs

85

Frequency of 0 Measurements

1.0 0.8 0.6 0.4 0.2 0.0 0.00 0.25 0.50 0.75 1.00 1.25 1.50 1.75 2.00
Exponent of X gate

Figure 6.8: Measurement outcomes at each value of the exponent t 2 Œ0;
2 in the circuit X t j0i

res = sim.run\_sweep(circ, sweep, repetitions=1000) \# Plot the
measurement outcomes at each value in the sweep angles = \[x\[0\]\[1\]
for x in sweep.param\_tuples()\] zeroes =
\[res\[i\].histogram(key="z")\[0\] / 1000 for i in range(len(res))\]
plt.plot(angles, zeroes, "--", linewidth=3) \# Plot options and
formatting plt.ylabel("Frequency of 0 Measurements")
plt.xlabel("Exponent of X gate") plt.grid()
plt.savefig("param-sweep-cirq.pdf", format="pdf")

We highlight several key components in this program. First, a symbol in
Cirq is used to represent a numerical value of a parameter that will be
determined later, before executing the circuit. When the circuit is
printed (see below), the name of the symbol appears in the circuit.
Circuit: 0: ---X\^t---M(’z’)---

Next, a sweep is a set of values that the symbol will take on.
Simulators in Cirq have a method, called run\_sweep, for executing
circuits at all values in a sweep. At each value, the circuit is
simulated a number of times set by the repetitions keyword argument. The
remaining code in the program is for plotting the outcome of the
run\_sweep, which is shown in Figure 6.8. Now that we have explored the
various quantum computing development libraries, let us look at three
protocols — quantum teleportation, superdense

86

CHAPTER 6 Development Libraries for Quantum Computer Programming

coding, and Bell’s inequality test — and then turn to the canon of
quantum algorithms that helped establish the field.

CHAPTER

7 Teleportation, Superdense Coding and Bell’s Inequality Two of the most
fascinating quantum circuits enable us to transmit information in ways
that are not possible in the classical regime. In this chapter, we will
learn how to build these two circuits. We will then examine a
foundational advance in quantum mechanics, the Bell Inequality.

7.1

Quantum Teleportation

Quantum teleportation, despite its name, does not teleport any physical
object. It does transmit the state of a qubit over any given distance in
a way that is completely secure. It is remarkable that it took more than
seventy years from the formulation of QM to realize that this framework
gave us a new form of secure communication. The protocol was developed
in 1993 \[33\] by Bennett and Brassard et al.; it was experimentally
verified in 1997 \[50\]. Bennett and Brassard had also developed quantum
key distribution in 1984, known as BB84 \[32\]. One of the key insights
of quantum teleportation is that we can treat entangled states as a
resource. We can use entangled states (known as EPR pairs or Bell
states) to perform a range of tasks that cannot be accomplished using
classical means. In quantum teleportation, Alice is the sender and she
wishes to transmit the state of a qubit, Q, to a receiver, Bob. The
algorithm requires three qubits in total: Alice’s qubit, Bob’s qubit,
and an ancilla qubit to create the EPR pair. An ancilla qubit is a qubit
we add to the circuit in order to facilitate a quantum computation; for
example, we can entangle an ancilla qubit with a primary qubit in order
to keep track of a certain state. © The Author(s), under exclusive
license to Springer Nature Switzerland AG 2021 J. D. Hidary, Quantum
Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_7

87

88

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

Figure 7.1: Quantum teleportation diagram. Relative to the notation in
the main text, jˆi is the state of qubit Q, A D R and B D S . Source:
Wikimedia

Let’s walk through the protocol in detail: 1. We set up the system with
three qubits: (a) Alice has a qubit, Q, with state jˆi. Alice wishes to
transmit the state jˆi to Bob in a secure manner. (b) To accomplish this
goal, Alice also starts with two additional qubits, which we will label
R and S. One of these qubits, say S, will be sent to Bob, and the other
will stay with Alice. In practice, S can be sent over a quantum channel
such as an optical fiber if the qubits are photons. 2. Alice prepares a
Bell state with qubits R and S. This is done by applying a Hadamard to
qubit R and then a CNOT between R and S, controlling on R. At this
point, Alice sends qubit S to Bob. 3. Alice now performs a Bell
measurement on her original qubit Q and her half of the EPR pair, R.
This is done by performing a CNOT between the qubits, controlling on Q,
then performing a Hadamard gate on Q, and finally measuring both qubits
in the computational basis. 4. After measuring, Alice now has two bits
of classical information, one from each measured qubit. Alice now
transmits these bits to Bob over

89

SECTION 7.1 Quantum Teleportation

Figure 7.2: Circuit diagram for quantum teleportation

Source: Wikimedia

a classical communication channel. Note that there are four possible
outcomes from her measurements: 00, 01, 10, and 11. 5. Depending on
which bit string Bob receives from Alice, he performs a set of
operations on his qubit, S. The dictionary of operations for each
measurement result is listed below. Performing the appropriate operation
guarantees Bob’s qubit, S, will be in the same state as Alice’s original
qubit Q — even though neither Alice nor Bob know what this state is! If
Alice transmits 00 01 10 11

then Bob applies this operator None — Bob’s qubit is in the right state
Z X XZ (apply Z first then X )

Two ways to represent quantum teleportation in a circuit diagram can be
seen in figure 7.2 and below; they are equivalent and it is useful to be
familiar with different ways of presenting circuits:

QW

jˆi

RW

j0i

SW

j0i

 H



H

 X

Z

jˆi

Let us highlight the following points on teleportation: 1. Note how
Alice prepares a Bell state with an H on R and then a CNOT across the
pair of qubits, R and S.

90

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

2.  Note how Alice transmits two bits of classical information to Bob —
    these are denoted with the sets of double wires in the quantum
    circuit.
3.  In this circuit Alice successfully transmits the state of jˆi to Bob
    via an EPR pair and the use of two classical bits. We can also
    represent this transmission as Œqq C Œcc  Œq where Œqq
    represents an EPR pair, Œcc represents a pair of classical bits and
    Œq is the state of a qubit we wish to transmit. While quantum
    teleportation is a tool we can use in quantum communications, it
    also has applications in quantum computing \[77\]. We can
    potentially use quantum teleportation to create a modular
    architecture for quantum computing by sending a quantum state from
    one module to another in a scaled quantum computer (see \[77\]).

7.2

Superdense Coding

Superdense coding is a method to transmit classical bits by sending only
one qubit from sender to receiver. If Alice wishes to transmit two
classical bits to Bob using a classical channel, she would have to use
two bits. With superdense coding, however, she can communicate the two
bits with the transmission of just one qubit. This protocol was
initially developed by Bennett and Wiesner \[34\] and then further
specified as a secure communications protocol \[287\]. Anton Zeilinger
experimentally demonstrated superdense coding transmission in 1995
\[187\]. To achieve superdense coding, Alice first prepares an EPR pair.
She then performs one of four operations on her half of the pair. Let’s
say that these are a pair of photons. To create the Bell pair, Alice
first applies a Hadamard to her photon and then a CNOT across the two
photons as she did in the case of preparing an EPR pair for quantum
teleportation protocol. The pair of photons is now entangled. Now Alice
chooses which of four classical states she wishes to transmit to Bob as
the intended message. Depending on the message she chooses to send,
Alice applies a specific quantum operator to her photon.

SECTION 7.3 Code for Quantum Teleportation and Superdense Communication

Figure 7.3: Circuit diagram for superdense coding

If Alice wants to send 00 01 10 11

91

Source: Wikimedia

Alice applies I (identity operator) X Z ZX (first apply X, then apply Z)

Next she sends her photon to Bob via a quantum communications channel
that preserves entanglement. Upon receipt of the photon, Bob applies the
Hadamard to her photon and then a CNOT across the photon pair. He then
performs a measurement. The result will be two classical bits of
information. Let us recall that the output of a measurement is classical
information. We can represent superdense coding in shorthand as follows:
Œq C Œqq  Œcc

7.3

Code for Quantum Teleportation and Superdense Communication

A program for quantum teleportation is provided in Cirq below. This
program encodes a random quantum state in Alice’s qubit and prints out
its Bloch sphere .x; y; z/ components. It then executes the quantum
teleportation circuit and prints out the Bloch sphere .x; y; z/
components of Bob’s qubit.

92

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

"""Quantum teleportation in Cirq. Modified from
quantum\_teleportation.py example at:
https://github.com/quantumlib/Cirq/tree/master/examples """ \# Imports
import random import cirq

def make\_quantum\_teleportation\_circuit(ranX, ranY): """Returns a
quantum teleportation circuit.""" circuit = cirq.Circuit() msg, alice,
bob = cirq.LineQubit.range(3) \# Creates Bell state to be shared between
Alice and Bob circuit.append(\[cirq.H(alice), cirq.CNOT(alice, bob)\])
\# Creates a random state for the Message
circuit.append(\[cirq.X(msg)**ranX, cirq.Y(msg)**ranY\]) \# Bell
measurement of the Message and Alice’s entangled qubit
circuit.append(\[cirq.CNOT(msg, alice), cirq.H(msg)\])
circuit.append(cirq.measure(msg, alice)) \# Uses the two classical bits
from the Bell measurement to recover the \# original quantum Message on
Bob’s entangled qubit circuit.append(\[cirq.CNOT(alice, bob),
cirq.CZ(msg, bob)\]) return msg, circuit

def main(): \# Encode a random state to teleport ranX = random.random()
ranY = random.random() msg, circuit =
make\_quantum\_teleportation\_circuit(ranX, ranY) \# Simulate the
circuit sim = cirq.Simulator() message =
sim.simulate(cirq.Circuit.from\_ops( \[cirq.X(msg)**ranX,
cirq.Y(msg)**ranY\])) \# Print the Bloch Sphere of Alice’s qubit
print("Bloch Sphere of Alice’s qubit:") b0X, b0Y, b0Z =
cirq.bloch\_vector\_from\_state\_vector( message.final\_state\_vector,
0) print("x: ", round(b0X, 4), "y: ", round(b0Y, 4), "z: ", round(b0Z,
4)) \# Display the teleportation circuit print("\nCircuit:")
print(circuit)

SECTION 7.3 Code for Quantum Teleportation and Superdense Communication

93

Record the final state of the simulation
========================================

final\_results = sim.simulate(circuit) \# Print the Bloch sphere of
Bob’s qubit print("\nBloch Sphere of Bob’s qubit:") b2X, b2Y, b2Z =
cirq.bloch\_vector\_from\_state\_vector(
final\_results.final\_state\_vector, 2) print("x: ", round(b2X, 4), "y:
", round(b2Y, 4), "z: ", round(b2Z, 4))

if **name** == ’**main**’: main()

An example output of this program is shown below. Bloch sphere of
Alice’s qubit: x: 0.654 y: -0.6177 z: -0.4367 Bloch sphere of Bob’s
qubit: x: 0.654 y: -0.6177 z: -0.4367

As can be seen, the Bloch sphere components of Alice and Bob’s qubit are
identical – in other words, the qubit has been “teleported” from Alice
to Bob. A program for superdense coding written in Cirq is provided
below. """Superdense coding in Cirq.""" \# Imports import cirq \# Helper
function for visualizing output def bitstring(bits): return ’’.join(’1’
if e else ’0’ for e in bits) \# Create two quantum and classical
registers qreg = \[cirq.LineQubit(x) for x in range(2)\] circ =
cirq.Circuit() \# Dictionary of operations for each message message =
{"00": \[\], "01": \[cirq.X(qreg\[0\])\], "10": \[cirq.Z(qreg\[0\])\],
"11": \[cirq.X(qreg\[0\]), cirq.Z(qreg\[0\])\]} \# Alice creates a Bell
pair circ.append(cirq.H(qreg\[0\])) circ.append(cirq.CNOT(qreg\[0\],
qreg\[1\])) \# Alice picks a message to send m = "01" print("Alice’s
sent message =", m)

94

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

Alice encodes her message with the appropriate quantum operations
=================================================================

circ.append(message\[m\]) \# Bob measures in the Bell basis
circ.append(cirq.CNOT(qreg\[0\], qreg\[1\]))
circ.append(cirq.H(qreg\[0\])) circ.append(\[cirq.measure(qreg\[0\]),
cirq.measure(qreg\[1\])\]) \# Print out the circuit print("\nCircuit:")
print(circ) \# Run the quantum circuit on a simulator backend sim =
cirq.Simulator() res = sim.run(circ, repetitions=1) \# Print out Bob’s
received message: the outcome of the circuit print("\nBob’s received
message =", bitstring(res.measurements.values()))

An example output of this program for the message 01 is shown below.
Alice’s sent message = 01 Circuit: 0: ---H---@---X---@---H---M--| | 1:
-------X-------X-------M--Bob’s received message = 01

As can be seen, Bob’s received message is exactly Alice’s sent message
via superdense coding.

7.4

Bell Inequality Test

Now let’s turn to another code walk-through: the Bell inequality test.
After briefly describing the experiment, we will go through a complete
program in Cirq to simulate it. The Bell inequality test is best
understood through a cooperative game involving two players, Alice and
Bob, that make decisions based on input from a referee. Alice and Bob
are separated (sitting in different rooms, say) and cannot communicate
during the game. At each round of the game, the referee sends one bit to
Alice, call it x, and one bit to Bob, call it y. Depending on the value
of the bit, Alice sends a bit of her own, a.x/, back to the referee.
Similarly, Bob sends a bit of his own, b.y/, back to the referee. The
referee

SECTION 7.4 Bell Inequality Test

95

looks at both bits and decides if Alice and Bob win or lose that round.
The condition for winning the round is a.x/ ˚ b.y/ D xy where ˚ denotes
addition modulo-2 (or, equivalently, XOR). Alice and Bob’s goal is to
win as many rounds as possible. Although they cannot communicate during
the game, they are allowed to meet before the game and set up a
strategy. An example strategy might be “Alice always sends back a.x/ D
x, and Bob always sends back a.y/ D 0.” Since each of a.x/ and b.y/ can
have two possible values, there are four possible deterministic
strategies that Alice and Bob can implement. Additionally, since there
are only four bits involved in the entire game, it’s not difficult to
enumerate all possible outcomes and see which strategy allows Alice and
Bob to win the most rounds (or, equivalently, win each round with the
highest probability). x 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1

y 0 0 0 0 1 1 1 1 0 0 0 0 1 1 1 1

a.x/ 0 0 1 1 0 0 1 1 0 0 1 1 0 0 1 1

b.y/ 0 1 0 1 0 1 0 1 0 1 0 1 0 1 0 1

a.x/ ˚ b.y/ 0 1 1 0 0 1 1 0 0 1 1 0 0 1 1 0

xy 0 0 0 0 0 0 0 0 0 0 0 0 1 1 1 1

Win? Yes No No Yes Yes No No Yes Yes No No Yes No Yes Yes No

Strategy \# \#1 \#2 \#3 \#4 \#1 \#2 \#3 \#4 \#1 \#2 \#3 \#4 \#1 \#2 \#3
\#4

Table 7.1: All possible outcomes of the Bell inequality test game: the
first two columns show bits the referee sends to Alice (x) and Bob (y).
The next two columns show Alice’s response (a.x/) and Bob’s response
(b.y/. The next column computes a.x/ ˚ b.y/, and the next column shows
the product xy. If these are equal, Alice and Bob win. The final column
shows which strategy Alice and Bob are using in each row, numbered \#1 -
\#4.

Table 7.1 enumerates all possible outcomes of the game. By analyzing
each strategy, one can see that Alice and Bob win at most 75% of the
time. The strategies that achieve this win percentage are \#1, in which
a.x/ D b.y/ D 0,

96

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

and \#4 in which a.x/ D b.y/ D 1. So the best that Alice and Bob can do
is to agree on either strategy \#1 or strategy \#4 before the game
begins to achieve the the best possible classical win rate of 75%. An
interesting phenomena happens when we allow a quantum strategy between
Alice and Bob. By a quantum strategy, we mean Alice and Bob are allowed
to use entanglement as a resource in their strategy. As we have seen in
this book, entanglement allows for stronger than classical correlations
in physical systems. If Alice and Bob are allowed to share entangled
qubits, they can remarkably win the Bell inequality test game with a
higher probability! The best quantum strategy achieves a winning
probability of cos2 .=8/, or about 85%. The quantum strategy for this
game is shown in the circuit diagram below. Here, the top (first) qubit
belongs to Alice, and the third qubit from the top belongs to Bob. The
first part of the circuit creates entanglement between Alice and Bob’s
qubits. Then, the referee “sends” in a random bit each to Alice and Bob.
In the circuit, this is done by performing a Hadamard operation on a
“fresh qubit” (one in the j0ipstate) to produce equal superposition.
Alice and Bob then perform a control- X operation on their qubits and
measure to record the results.

H



X

0:25

X 0:5 H

 X 0:5

H



Below, we show the complete program in Cirq for setting up this circuit
and simulating the quantum strategy for the Bell inequality test.
"""Creates and simulates a circuit equivalent to a Bell inequality
test.""" \# Imports import numpy as np import cirq def main(): \# Create
circuit circuit = make\_bell\_test\_circuit() print(’Circuit:’)

SECTION 7.4 Bell Inequality Test

97

print(circuit) \# Run simulations print() repetitions = 1000
print(’Simulating {} repetitions...’.format(repetitions)) result =
cirq.Simulator().run(program=circuit, repetitions=repetitions) \# a b x
y

Collect results = np.array(result.measurements\[’a’\]\[:, =
np.array(result.measurements\[’b’\]\[:, =
np.array(result.measurements\[’x’\]\[:, =
np.array(result.measurements\[’y’\]\[:,

0\]) 0\]) 0\]) 0\])

Compute the winning percentage
==============================

outcomes = a \^ b == x & y win\_percent = len(\[e for e in outcomes if
e\]) \* 100 / repetitions \# Print data print() print(’Results’)
print(’a:’, bitstring(a)) print(’b:’, bitstring(b)) print(’x:’,
bitstring(x)) print(’y:’, bitstring(y)) print(’(a XOR b) == (x AND
y):\n ’, bitstring(outcomes)) print(’Win rate:
{}%’.format(win\_percent))

def make\_bell\_test\_circuit(): \# Qubits for Alice, Bob, and referees
alice = cirq.GridQubit(0, 0) bob = cirq.GridQubit(1, 0) alice\_referee =
cirq.GridQubit(0, 1) bob\_referee = cirq.GridQubit(1, 1) circuit =
cirq.Circuit() \# Prepare shared entangled state between Alice and Bob
circuit.append(\[ cirq.H(alice), cirq.CNOT(alice, bob),
cirq.X(alice)\*\*-0.25,\]) \# Referees flip coins circuit.append(\[
cirq.H(alice\_referee), cirq.H(bob\_referee),\]) \# Players do a sqrt(X)
based on their referee’s coin circuit.append(\[
cirq.CNOT(alice\_referee, alice)**0.5, cirq.CNOT(bob\_referee,
bob)**0.5,\])

98

CHAPTER 7 Teleportation, Superdense Coding and Bell’s Inequality

Then results are recorded
=========================

circuit.append(\[ cirq.measure(alice, key=’a’), cirq.measure(bob,
key=’b’), cirq.measure(alice\_referee, key=’x’),
cirq.measure(bob\_referee, key=’y’),\]) return circuit

def bitstring(bits): return ’’.join(’1’ if e else ’\_’ for e in bits)

if **name** == ’**main**’: main()

An example output of this program is shown below, where we simulate 75
repetitions only to visualize the output more easily. The output of this
program is interpreted as follows. The bitstrings for Alice and Bob are
shown in the first line. These are the bits each player sends back to
the referee (the underscore indicates the 0 bit). The next lines show
the bitstrings sent to Alice (x) and Bob (y). Finally, the winning
condition a.x/ ˚ b.y/ D xy is shown as a bitstring for each round. The
win rate is computed from the number of 1s in this bitstring, which
indicate a win. Simulating 75 repetitions... Results a:
1\_1111\_1\_1111\_11\_1111\_1\_1\_\_\_\_\_\_1\_1\_*
11\_1**111\_1\_1\_111\_1111\_*11\_1111\_1\_1**** b:
1\_1\_*11\_1\_1\_1\_11**11\_*1\_1\_1*1***
\_11**11\_1\_1**\_11\_\_1\_\_1111\_1\_1\_\_\_1**11\_1 x:
11\_11\_1\_1111*1\_11***\_11\_1\_\_111\_1
1\_\_1\_11\_1\_\_\_11\_111111111\_\_11\_\_1\_111\_\_11 y:
\_1\_11111111\_\_11\_11\_\_1**1111**\_1111\_\_
1\_\_111\_1**111**\_1\_\_11\_\_1\_111\_11\_\_\_1\_\_\_1 (a XOR b) == (x
AND y): 1\_11111\_11\_\_1111111111111\_11111111111
1\_1111\_11111111111111\_11\_111\_11111\_\_11 Win rate: 84.0%

As can be seen, we achieve a win rate of 84% in this example, which is
greater than possible with purely classical strategies. Note that using
a larger

SECTION 7.4 Bell Inequality Test

99

number of repetitions (i.e., simulating more rounds) we would see
asymptotic convergence to the optimal win rate of cos2 .=8/  85%.

Summary Quantum teleportation, superdense coding and Bell’s inequality
test are some of the most intriguing circuits for quantum processors.
For additional quantum networking protocols, see the Quantum Protocol
Zoo at http://wiki. veriqloud.fr. Now let us turn to the canon of
quantum algorithms that demonstrated the potential of quantum advantage
over classical computing.

CHAPTER

8 The Canon: Code Walkthroughs In this chapter, we will walk through a
number of fundamental quantum algorithms. We call these algorithms the
canon as they were all developed in the early years of quantum computing
and were the first to establish provable computational speedups with
quantum computers. We discussed most of these algorithms at a high level
in chapter 2; we will now walk through them in a more detailed manner. A
number of these algorithms require a quantum computer that is still in
the future, but by analyzing them now we can deepen our understanding of
what will be possible. Additionally, variants of these algorithms can be
used to prove advantages with near-term quantum computers in the
noiseless \[58\] and even noisy \[59\] regimes. Several of the
algorithms considered in this chapter are known as “black box” or “query
model” quantum algorithms. In these cases, there is an underlying
function which is unknown to us. However, we are able to construct
another function, called an oracle, which we can query to determine the
relationship of specific inputs with specific outputs. More
specifically, we can query the oracle function with specific inputs in
the quantum register and reversibly write the output of the oracle
function into that register. That is, we have access to an oracle Of
such that Of .jxijyi/ D jx ˚ f .y/i

(8.1)

where ˚ denotes addition modulo-2. It’s easy to see that Of is unitary
(reversible) because it is self-inverse. This can seem like “cheating”
at first — how could we construct a circuit to perform Of ? And how
could we know if it is an efficient circuit? One reason to think about
quantum algorithms in the query model is that it provides a lower bound
on the number of steps (gates). Each query is at least one step in the
algorithm, so if it cannot be done efficiently with queries, it can
certainly not be done efficiently with gates. © The Author(s), under
exclusive license to Springer Nature Switzerland AG 2021 J. D. Hidary,
Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_8

101

102

CHAPTER 8 The Canon: Code Walkthroughs

Figure 8.1: Overview of studied quantum algorithms; paradigms include:
Grover Operator (GO), Quantum Fourier Transform (QFT),
Harrow/Hassidim/Lloyd (HHL), Variational Quantum Eigensolver (VQE), and
direct Hamiltonian simulation (SIM). The simulation match column
indicates how well the hardware quantum results matched the simulator
results. Table and Caption Source: \[84\]

The query model can also be used to prove fast quantum algorithms
relative to the oracle. We can give both a quantum computer and a
classical computer access to the same oracle and see which performs
better. It’s possible to prove lower bounds or exact expressions for the
number of queries in the classical and quantum cases, thereby making it
possible to prove computational advantages relative to oracles. Examples
of quantum algorithms with provable relative speedups include Deutsch’s
algorithm and the Berstein-Vazirani algorithm. Finally, if one can find
a way to instantiate the oracle in a number of gates that scales
polynomially in the size of the input register, one can find “true”
(i.e., not relative) quantum speedups. This is the case with Shor’s
algorithm for quantum factoring.1 Shor’s algorithm built off previous
work in query model algorithms for artificial problems. Shor was able to
modify this work and instantiate the oracle to construct an explicit
(i.e., not involving oracle access) algorithm for factoring. Factoring
is markedly not an artificial problem — it is exceedingly important as
we base most of our public-key cryptography on the belief that factoring
is hard to do! Section 8.5 discusses this further. Before this, we
discuss the historical quantum algorithms leading up to Shor’s
algorithm. We note that these black box/oracle algorithms are one
particular class of quantum algorithms. Other algorithm classes such as
1 The classical complexity of factoring has not been proven to be
intractable, but it is widely believed to be so since no one has yet
discovered an efficient algorithm.

SECTION 8.1 The Deutsch-Jozsa Algorithm

103

quantum simulation are shown in Figure 8.1. In upcoming chapters, we
will cover additional applications and code for algorithms that are
focused on the NISQ-regime processors. For now, though, we cover the
canon.

8.1

The Deutsch-Jozsa Algorithm

Deutsch’s algorithm was the first to demonstrate a clear advantage of
quantum over classical computing. In Deutsch’s problem we are given a
black box which computes a one-bit Boolean function. That is, a function
which takes in one bit and outputs one bit. We can represent the
function f as f W f0; 1g ! f0; 1g

(8.2)

We can imagine, for example, as David Deutsch has pointed out, that the
black box function is computing some complicated function such as a
routing algorithm and the output (0 or 1) indicates which route is
chosen \[89\]. There are exactly four one-input, one-output Boolean
functions:2 x 0 1

f0 0 0

f1 1 1

fx 0 1

fxN 1 0

The first two of these are constant functions, f0 and f1 . That is, they
always output a constant value. We call the other two, fx and fxN ,
balanced. Over their inputs 0 and 1, they have an equal number of 0s and
1s in their truth table. We can now state Deutsch’s problem: Given
access to a one bit input and one bit output Boolean function,
determine, by querying the function as few times as possible, whether
the function is balanced or constant. If you were to approach this with
classical tools, you would have to query the function at least twice:
first to see the output when the input is 0 and then the output when the
input is 1. The remarkable discovery by David Deutsch is that you only
need one query on a quantum computer! The original Deutsch algorithm
handles this case of a one-bit Boolean oracle \[88\], and the 2 Code and
exposition of the DJ algorithm adapted from “Textbook algorithms in
Cirq” linked on the book’s website.

104

CHAPTER 8 The Canon: Code Walkthroughs

Deutsch-Jozsa (DJ) algorithm generalizes the approach to handle Boolean
functions of n inputs \[90\]. It’s not difficult to see that, with
classical tools, one must query an n bit Boolean function at least n
times. The DJ algorithm solves this problem in only one query. 8.3

Quantum Advantage Demonstrated by Deutsch-Jozsa

Classically, one must query the one-bit Boolean function twice to
distinguish the constant function from the balanced function. For an
n-bit Boolean function, one must query n times. On a quantum computer
using DJ one only has to query once. We now turn to the quantum approach
to this problem. Above, we have described a classical function on bits
that is not reversible, e.g., the constant functions f0 and f1 . That
is, knowing the value of the output does not allow us to determine
uniquely the value of the input. In order to run this on a quantum
computer, however we need to make this computation reversible. A trick
for taking a classical non-reversible function and making it reversible
is to compute the value in an extra register (or, equivalently, store
inputs to the function in an extra register). Suppose we have an n bit
input x and we are computing a (potentially non-reversible) Boolean
function f .x/. Then we can implement this via a unitary Uf that acts on
n C 1 qubits Uf .jxijyi/ WD jxijy ˚ f .x/i Here the symbol ˚ denotes
addition modulo-2 (a.k.a. XOR); in the expression above, we have
identified how Uf acts on all computational basis states jxi and on the
single output qubit jyi. Since we have defined Uf on the computational
basis, we extend its definition to all vectors in the state space by
linearity. To see that this is reversible, one can note that applying
the transformation twice returns the state to its original form. Even
further, Uf is unitary since it maps the orthonormal computational basis
to itself and so preserves the length of the vectors that it acts on.
One core idea in this algorithm is that we will measure in a different
basis than the computational basis. If we measure in the computational
basis (e.g., the z-basis) then we will gain no quantum advantage as we
have two basis states, j0i and j1i, and those correspond to the
classical bits, 0 and 1. One of the tricks that makes this algorithm
work is that we will measure in the Hadamard basis state which is a
superposition of j0i and j1i \[176\]. Figure 8.2 shows a circuit diagram
of DJ. Let’s see how to implement these functions in Cirq. f0 enacts the
transform

SECTION 8.1 The Deutsch-Jozsa Algorithm

Figure 8.2: The DJ circuit

105

Source: Wikimedia

j00i ! j00i j01i ! j01i j10i ! j10i j11i ! j11i This is just the
identity transform, i.e., an empty circuit. f1 enacts the transform j00i
! j01i j01i ! j00i j10i ! j11i j11i ! j10i This is a bit flip gate on
the second qubit. To gain an understanding of how this newly defined
reversible operator works, we will compute Ufx .j0ij0i/ as an example to
demonstrate. Recall that j00i is shorthand for j0ij0i. Then, by
definition, Ufx .j00i/ D Ufx .j0ij0i/ WD j0ij0 ˚ fx .0/i D j0ij0 ˚ 0i D
j0ij0i It is worthwhile to compute Ufx for each of j0ij1i, j1ij0i and
j1ij1i; then let us check that fx enacts the transform j00i ! j00i j01i
! j01i j10i ! j11i j11i ! j10i

106

CHAPTER 8 The Canon: Code Walkthroughs

This is nothing more than a CNOT from the first qubit to the second
qubit. Finally fxN enacts the transform j00i ! j01i j01i ! j00i j10i !
j10i j11i ! j11i which is a CNOT from the first qubit to the second
qubit followed by a bit flip on the second qubit. We can encapsulate
these functions into a dictionary which maps oracle names to the
operations in the circuit needed to enact this function: \# Import the
Cirq Library import cirq \# Get two qubits, a data qubit and target
qubit, respectively q0, q1 = cirq.LineQubit.range(2) \# Dictionary of
oracles oracles = {’0’: \[\], ’1’: \[cirq.X(q1)\], ’x’: \[cirq.CNOT(q0,
q1)\], ’notx’: \[cirq.CNOT(q0, q1), cirq.X(q1)\]}

Let us turn now to Deutsch’s algorithm. Suppose we are given access to
the reversible oracle functions we have defined before. By a similar
argument for our irreversible classical functions, you can show that you
cannot distinguish the balanced from the constant functions by using
this oracle only once. But now we can ask the question: what if we are
allowed to query this function in superposition, i.e., what if we can
use the power of quantum computing? Deutsch was able to show that you
could solve this problem with quantum computers using only a single
query of the function. To see how this works, we need two simple
insights. Suppose we prepare the second qubit in the superposition state
1 j i D p .j0i j1i/ 2 and apply the oracle. Using the linearity of the
operator Uf to acquire the second equation and an observation for the
third, we can check that 1 Uf jxij i D Uf jxi p .j0i j1i/ 2 1 D jxi p
.jf .x/i jf .x/ ˚ 1i/ D . 1/f .x/ jxij i 2

SECTION 8.1 The Deutsch-Jozsa Algorithm

107

This is the phase kickback trick. By applying Uf onto a target which is
in superposition, the value of the function ends up in the global phase,
thus kicking back the information we need on whether the function is
constant or balanced; the information is encoded in the phase. How can
we leverage this to distinguish between constant and balanced functions?
Note that for constant functions the phase that is applied is the same
for all inputs jxi, whereas for balanced functions the phase is
different for each value of x. To use the phase kickback trick for each
of the oracles, we apply the following transform on the first qubit f0 !
I f1 !

I

fx ! Z fxN ! Uf 0

D

Uf 1

D

Z

X Uf x

D

UfxN

D

  X

Now we only need to distinguish between the identity gate and the Z gate
on the first qubit; we can do this by recalling that: HZH D X   1 1 1
H Dp 1 2 1 This means that we can turn a phase flip into a bit flip by
applying Hadamard gates before and after the phase flip. If we look at
the constant and balanced functions we see that the constant functions
will be proportional to I and the balanced will be proportional to X. If
we feed in j0i to this register, then in the first case we will only see
j0i and in the second case we will see j1i. In other words we will be
able to distinguish constant from balanced using a single query of the
oracle.

108

CHAPTER 8 The Canon: Code Walkthroughs

H

H Uf

X

H

Import the Cirq Library
=======================

import cirq \# Get two qubits, a data qubit and target qubit,
respectively q0, q1 = cirq.LineQubit.range(2) \# Dictionary of oracles
oracles = {’0’: \[\], ’1’: \[cirq.X(q1)\], ’x’: \[cirq.CNOT(q0, q1)\],
’notx’: \[cirq.CNOT(q0, q1), cirq.X(q1)\]} def
deutsch\_algorithm(oracle): """Yields a circuit for Deutsch’s algorithm
given operations implementing the oracle.""" yield cirq.X(q1) yield
cirq.H(q0), cirq.H(q1) yield oracle yield cirq.H(q0) yield
cirq.measure(q0) \# Display each circuit for all oracles for key, oracle
in oracles.items(): print(’Circuit for {}...’.format(key))
print(cirq.Circuit.from\_ops(deutsch\_algorithm(oracle)), end="\n\n") \#
Get a simulator simulator = cirq.Simulator() \# Execute the circuit for
each oracle to distinguish constant from balanced for key, oracle in
oracles.items(): result = simulator.run(
cirq.Circuit.from\_ops(deutsch\_algorithm(oracle)), repetitions=10 )
print(’oracle: {:&lt;4} results: {}’.format(key, result))

Now let’s extend the Deutsch problem to Boolean functions of n Boolean
inputs, not just single-input functions as above. We saw that with the
Deutsch algorithm we can double our speed, going from two queries
classically to one query quantum mechanically.

=n

H ˝n

H ˝n Uf

X

H

SECTION 8.1 The Deutsch-Jozsa Algorithm

109

If we are able to query an n-bit oracle just once and determine whether
the function is constant or balanced we have a time complexity of O.1/,
a significant speedup over O.n/ queries. All Boolean functions for
one-bit input are either constant or balanced. For Boolean functions
with two input bits there are two  constant functions, f .x0 ; x1 / D 0
and f .x0 ; x1 / D 1, while there are 42 D 6 balanced functions. We call
this more generalized form the Deutsch-Jozsa algorithm. The following
code gives you the operations for querying these functions.
"""Deutsch-Jozsa algorithm on three qubits in Cirq.""" \# Import the
Cirq library import cirq \# Get three qubits -- two data and one target
qubit q0, q1, q2 = cirq.LineQubit.range(3) \# Oracles for constant
functions constant = (\[\], \[cirq.X(q2)\]) \# Oracles for balanced
functions balanced = (\[cirq.CNOT(q0, q2)\], \[cirq.CNOT(q1, q2)\],
\[cirq.CNOT(q0, q2), cirq.CNOT(q1, q2)\], \[cirq.CNOT(q0, q2),
cirq.X(q2)\], \[cirq.CNOT(q1, q2), cirq.X(q2)\], \[cirq.CNOT(q0, q2),
cirq.CNOT(q1, q2), cirq.X(q2)\]) def your\_circuit(oracle): """Yields a
circuit for the Deutsch-Jozsa algorithm on three qubits.""" \# phase
kickback trick yield cirq.X(q2), cirq.H(q2) \# equal superposition over
input bits yield cirq.H(q0), cirq.H(q1) \# query the function yield
oracle \# interference to get result, put last qubit into |1&gt; yield
cirq.H(q0), cirq.H(q1), cirq.H(q2) \# a final OR gate to put result in
final qubit yield cirq.X(q0), cirq.X(q1), cirq.CCX(q0, q1, q2) yield
cirq.measure(q2)

Get a simulator
===============

simulator = cirq.Simulator() \# Execute circuit for oracles of constant
value functions print(’Your result on constant functions’) for oracle in
constant:

110

CHAPTER 8 The Canon: Code Walkthroughs

result = simulator.run(cirq.Circuit.from\_ops(your\_circuit(oracle)),
repetitions=10) print(result) \# Execute circuit for oracles of balanced
functions print(’Your result on balanced functions’) for oracle in
balanced: result =
simulator.run(cirq.Circuit.from\_ops(your\_circuit(oracle)),
repetitions=10) print(result)

We can now see how to query an oracle of n-bit boolean inputs to check
whether it is constant or balanced.

8.2

The Bernstein-Vazirani Algorithm

Now let’s turn to the Bernstein-Vazirani (BV) algorithm that we
considered earlier in this book \[36\]. As with DJ, the goal of BV is
also to ascertain the nature of a black-box Boolean function. While it
is true that DJ demonstrates an advantage of quantum over classical
computing, if we allow for a small error rate, then the advantage
disappears: both classical and quantum approaches are in the order of
O.1/ time complexity \[176\]. BV was the first algorithm developed that
shows a clear separation between quantum and classical computing even
allowing for error, i.e., a true nondeterministic speedup. Here is the
BV problem statement: Given an unknown function of n inputs: f .xn

1 ; xn 2 ; :::; x1 ; x0 /;

let a be an unknown non-negative integer less than 2n . Let f .x/ take
any other such integer x and modulo-2 sum x multiplied by a. So the
output of the function is: a  x D a0 x0 ˚ a1 x1 ˚ a2 x2 :::: Find a in
one query of the oracle \[194\]. Just as in DJ, we prepare the states of
two sets of qubits: the data register qubits and the target qubit. The
data register qubits are set to j0i and the target set to j1i. We then
apply H to both sets of qubits to put them in superposition. H applied
to the data register qubits prepares us to measure in the X basis.

SECTION 8.2 The Bernstein-Vazirani Algorithm

111

We then apply the unitary Uf , an H to the data register qubits and then
measure those qubits. Since we only applied Uf once, the time complexity
of BV is O.1/.

=n

H ˝n

H ˝n Uf

X

H

The Bernstein-Vazirani Algorithm """Bernstein-Vazirani algorithm in
Cirq.""" \# Imports import random import cirq

def main(): """Executes the BV algorithm.""" \# Number of qubits
qubit\_count = 8 \# Number of times to sample from the circuit
circuit\_sample\_count = 3 \# Choose qubits to use input\_qubits =
\[cirq.GridQubit(i, 0) for i in range(qubit\_count)\] output\_qubit =
cirq.GridQubit(qubit\_count, 0) \# Pick coefficients for the oracle and
create a circuit to query it secret\_bias\_bit = random.randint(0, 1)
secret\_factor\_bits = \[random.randint(0, 1) for \_ in
range(qubit\_count)\] oracle = make\_oracle(input\_qubits,
output\_qubit, secret\_factor\_bits, secret\_bias\_bit) print(’Secret
function:\nf(x) = x\*&lt;{}&gt; + {} (mod 2)’.format( ’, ’.join(str(e)
for e in secret\_factor\_bits), secret\_bias\_bit)) \# Embed the oracle
into a special quantum circuit querying it exactly once circuit =
make\_bernstein\_vazirani\_circuit( input\_qubits, output\_qubit,
oracle) print(’\nCircuit:’) print(circuit) \# Sample from the circuit a
couple times simulator = cirq.Simulator()

112

CHAPTER 8 The Canon: Code Walkthroughs

result = simulator.run(circuit, repetitions=circuit\_sample\_count)
frequencies = result.histogram(key=’result’, fold\_func=bitstring)
print(’\nSampled results:\n{}’.format(frequencies)) \# Check if we
actually found the secret value. most\_common\_bitstring =
frequencies.most\_common(1)\[0\]\[0\] print(’\nMost common matches
secret factors:\n{}’.format( most\_common\_bitstring ==
bitstring(secret\_factor\_bits)))

def make\_oracle(input\_qubits, output\_qubit, secret\_factor\_bits,
secret\_bias\_bit): """Gates implementing the function f(a) = a\*factors
+ bias (mod 2).""" if secret\_bias\_bit: yield cirq.X(output\_qubit) for
qubit, bit in zip(input\_qubits, secret\_factor\_bits): if bit: yield
cirq.CNOT(qubit, output\_qubit)

def make\_bernstein\_vazirani\_circuit(input\_qubits, output\_qubit,
oracle): """Solves for factors in f(a) = a\*factors + bias (mod 2) with
one query.""" c = cirq.Circuit() \# Initialize qubits c.append(\[
cirq.X(output\_qubit), cirq.H(output\_qubit),
cirq.H.on\_each(\*input\_qubits),\]) \# Query oracle c.append(oracle) \#
Measure in X basis c.append(\[ cirq.H.on\_each(*input\_qubits),
cirq.measure(*input\_qubits, key=’result’)\]) return c

def bitstring(bits): """Creates a bit string out of an iterable of
bits.""" return ’’.join(str(int(b)) for b in bits)

if **name** == ’**main**’: main()

SECTION 8.3 Simon’s Problem

113

Here we initialize the target (or output) register to j1i with an X
operator and the data register qubits from state j0i to the jCi / j i
basis by applying H . We then query the oracle, apply H to each of the
input qubits and measure the input qubits. This gives us the answer that
we were seeking, a, in one query. Thus, no matter how many inputs we
have, we can perform this algorithm in O.1/ time. """ === EXAMPLE OUTPUT
for BV === Secret function: f(x) = x\*&lt;0, 1, 1, 1, 0, 0, 1, 0&gt; + 1
(mod 2) Sampled results: Counter({’01110010’: 3}) Most common matches
secret factors: True """

8.3

Simon’s Problem

Soon after BV’s result, Daniel Simon demonstrated the ability to
determine the periodicity of a function exponentially faster on a
quantum computer compared with a classical one. Let us recall that a
function can map two different inputs to the same output but must not
map the same input to two different outputs. In other words, 2W1 is
acceptable, but 1W2 is not. For example, the function f .x/ D x 2 which
squares each input is in fact a function; two different inputs, namely 1
and 1 both map to 1, i.e., f .x/ is 2:1. See Part III for a review of
functions and injectivity, surjectivity and bijectivity. If we determine
that the function is of the 2W1 type, then our next challenge is to
investigate the period of the function (see section 8.5 for an
explanation of periodicity); this is the core objective of Simon’s
problem. Here is an outline of the problem in more formal language: The
problem considers an oracle that implements a function mapping an n-bit
string to an m-bit string f Wf0; 1gn ! f0; 1gm , with m  n, where it is
promised that f is a 1W1 type function (each input gives a different
output) or 2W1 type function (two inputs give the same

114

CHAPTER 8 The Canon: Code Walkthroughs

output) with non-zero period s 2 f0; 1gn such that for all x; x0 we have
f .x/ D f .x0 / if and only if x0 D x ˚ s, where ˚ corresponds to
addition modulo-2.3 The problem is to determine the type of the function
f and, if it is 2W1, to determine the period s. \[271\] Simon’s problem
is in the same vein as Deutsch’s problem — you are presented with an
oracle — a black box function where you can observe the output for
specific inputs, but not the underlying function. The challenge is to
determine if this black-box process ever sends two different inputs to
the same output, and if so, determine how often that occurs. Note that
in these algorithms we do not find out what the underlying function in
the black box is, only the relationship between the input and the output
as seen from outside the box. The actual function may be quite
complicated and may require even more steps to analyze than the
input/output relationship. We explore the concept of oracles further in
this chapter. Simon was successful in proving that we can solve this
problem to determine the periodicity of a function exponentially faster
on a quantum computer compared with a classical one. Shor built on this
key result in developing his algorithm for factoring large numbers when
he realized that the two problems — finding the periodicity of a
function and factoring a large composite number — are in fact
isomorphic. Twenty years after Simon presented his problem, researchers
did in fact successfully use a quantum system to determine the
periodicity of a function \[271\]. Check the book’s website for sample
code for Simon’s problem.

8.4

Quantum Fourier Transform

In chapter 3, we discussed the Quantum Fourier Transform (QFT) as a
method to set up the amplitudes for measurement that will favor the
qubit which has the information we require. We can implement a QFT
circuit on NISQ hardware in a straightforward manner. Here is the
standard circuit diagram for QFT: 3 When we do addition modulo-2, we
equate 2 with 0. So, for example, 1 ˚ 1 D 0 and we would say, “The sum
of 1 and 1 modulo-2 is 0.”

115

SECTION 8.4 Quantum Fourier Transform

jx1 i

H R=2 R=4 R=8 H R=2 R=4



jx2 i



jx3 i



jx4 i

H R=2

 



H

Now let’s walk through the code for QFT as we will use this technique in
the upcoming section on Shor’s algorithm. We’ll go through the program
step by step, explaining first high-level details and then discussing
implementation details. First, we import the necessary packages for this
program including the Cirq library. """Creates and simulates a circuit
for Quantum Fourier Transform (QFT) on a 4 qubit system. """ \# Imports
import numpy as np import cirq

Next, we define the main function, which simply calls the circuit
generation function and then runs it — in this case on the simulator.
The program then prints the final state of the wavefunction after the
QFT has been applied. def main(): """Demonstrates the Quantum Fourier
transform.""" \# Create circuit and display it qft\_circuit =
generate\_2x2\_grid\_qft\_circuit() print(’Circuit:’)
print(qft\_circuit) \# Simulate and collect the final state simulator =
cirq.Simulator() result = simulator.simulate(qft\_circuit) \# Display
the final state print(’\nFinalState’)
print(np.around(result.final\_state, 3))

116

CHAPTER 8 The Canon: Code Walkthroughs

Figure 8.3: Modified QFT circuit including SWAP operations fit for
running on a 2x2 grid of qubits with nearest-neighbor interactions.

Next, we define a helper function for building the QFT circuit. This
function yields a controlled-Rz rotation as well as a SWAP gate on the
input qubits. def cz\_and\_swap(q0, q1, rot): """Yields a controlled-RZ
gate and SWAP gate on the input qubits.""" yield cirq.CZ(q0, q1)\*\*rot
yield cirq.SWAP(q0,q1)

Finally, we use this helper function to write the entire circuit, which
is done in the function below. First, we define a 2 x 2 grid of qubits
and label them a through d . In many quantum computing systems there are
constraints one which qubits can interact with each other. For example
perhaps only nearest-neighbor qubits can interact. Then we cannot apply
the standard QFT circuit described above. Instead, a modified QFT
circuit including SWAP operations needs to be applied, as illustrated in
Figure 8.3. This is the circuit we will implement in our example. We
apply a series of Hadamard and control rotation operators as specified
by the diagram. In this example we perform the quantum Fourier transform
on the .1; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0; 0/ vector, which
means acting with the QFT circuit on the ground state j0000i. def
generate\_2x2\_grid\_qft\_circuit(): """Returns a QFT circuit on a 2 x 2
planar qubit architecture. Circuit adopted from
https://arxiv.org/pdf/quant-ph/0402196.pdf. """ \# Define a 2\*2 square
grid of qubits a, b, c, d = \[cirq.GridQubit(0, 0), cirq.GridQubit(0,
1), cirq.GridQubit(1, 1), cirq.GridQubit(1, 0)\] \# Create the Circuit
circuit = cirq.Circuit.from\_ops( cirq.H(a), cz\_and\_swap(a, b, 0.5),
cz\_and\_swap(b, c, 0.25),

SECTION 8.5 Shor’s Algorithm

117

cz\_and\_swap(c, d, 0.125), cirq.H(a), cz\_and\_swap(a, b, 0.5),
cz\_and\_swap(b, c, 0.25), cirq.H(a), cz\_and\_swap(a, b, 0.5),
cirq.H(a), strategy=cirq.InsertStrategy.EARLIEST ) return circuit

Finally, we can run this circuit by calling the main function: if
**name** == ’**main**’: main()

The output of this program is shown below: FinalState \[0.25+0.j
0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j
0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j 0.25+0.j\]

Figure 8.4 delineates the process of applying QFT.

8.5

Shor’s Algorithm

RSA Cryptography Suppose Alice would like to send a private message to
Bob via the internet. Alice’s message could very well be intercepted by
a malicious eavesdropper, Eve, along its journey. This is embarrassing,
yet harmless, if Alice is sending Bob a note, but it is an issue if
Alice is sending Bob her credit card number. How can we send messages
securely via the internet? Cryptography is the study of the making and
breaking of secret codes. Cryptography refers to the writing of secret
codes, while cryptanalysis refers to the breaking of those codes. RSA is
a cryptographic protocol used widely across many platforms for the
secure transfer of information via the internet. The abbreviation RSA
refers to Rivest, Shamir and Adelman, three pioneers in its development
\[239\]. The core conjecture of the RSA protocol is that multiplying two
large prime numbers is a trapdoor function; multiplying two large prime
numbers is easy, yet finding the two factors after the multiplication
has occurred is hard.

118

CHAPTER 8 The Canon: Code Walkthroughs

Figure 8.4: QFT and measurement

Source: \[204\]

Later in this chapter, we’ll see that a fault-tolerant quantum computer
will have the capacity to surmount the difficulty posed by the
factorization process which puts the entire RSA scheme at risk \[254\]!
This leads us to post-quantum cryptography, a fascinating field at the
intersection of mathematics, physics and computer science. In 1994,
Peter Shor published his landmark paper establishing a quantum algorithm
for the prime factorization of numbers \[254\]. The problem of factoring
a number into primes reduces to finding a factor, since if you can find
one factor, you can use it to divide the original number and consider
the smaller factors. Eventually, using this divide (literally) and
conquer strategy, we can completely factor the number into primes.

SECTION 8.5 Shor’s Algorithm

119

His technique to find a factor of any number n is to find the period, r,
of a certain function f and then use the knowledge of the period of said
function to find a factor of the number.

The Period of a Function Periodic functions are functions whose outputs
enjoy a “periodic” nature. In other words, after having seen a
particular output, we should expect to see the same output after some
period (often to be thought of as a period of time). Most of the fun of
periodic functions lies in determining what that period is, i.e. how
“long” we have to wait until we see the same output! Periodic functions
are not so unfamiliar and are encountered already in the early stages of
trigonometry and the study of the “circular” functions cosine, sine,
etc. To see this, play around with the trigonometric functions in the
following exercise: Exercise Perhaps the first examples of periodic
functions we encounter are the trigonometric functions cosine and sine.
Verify that the function x. / WD cos 2 3   has the property that
x.0/ D 1. Discover the “next” value of  for which x.t / equals 1.
Verify also that the function y. / WD si n 2 3  has the property that
y.0/ D 0. Discover the “next” value of  such that y./ D 0. How often
should we expect the value of x. / to be equal to 1? How often should
we expect the value of y. / to be equal to 0? What is the period of
x./? Of y./? Can you come up with a geometric reason for why this is?
8.4

Shor realized that to find a factor of any number n he could first find
the period, r, of a certain function f and then use the knowledge of the
period of said function to find a factor of the number. To get an idea
of what the period of a function might be, consider raising some number,
like 2, to higher and higher powers, and then taking the result modulo a
product of two prime numbers such as 91 D 13  7. For example, we have:

120

CHAPTER 8 The Canon: Code Walkthroughs

20 (mod 91/ 21 (mod 91/ 22 (mod 91/ 23 (mod 91/ 24 (mod 91/ 25 (mod 91/
26 (mod 91/ 27 (mod 91/ 28 (mod 91/ :: :

1 2 4 8 16 32 64 37 74 :: :

We see that the numbers cannot grow forever due to the modulo operation.
For example, 26 (mod 91/ D 64 and the next highest power 27 (mod 91/ D
37. Exercise Figure out if the powers of 2 ever cycle back to the number
1 in the table above. More precisely: find the smallest number r beyond
0 such that 2r (mod 91/ D 1 8.5

Persistence pays off here. If you tried the above exercise, you found
that, yes, 212 (mod 91/ D 1, and that 12 is the smallest number beyond 0
that makes this happen. Was it even obvious that it would return to 1?
We refer to the number 12 as the period of the function defined by f .x/
WD 2x (mod 91/ In general, for a function defined by f .x/ WD ax (mod n/
for some a 2 f1; 2; :::; n 1g relatively prime to n, the period of the
function f .x/ is the smallest value r of x greater than 0 such that f
.r/ D 1 once again. In other words, since at x D 0 a0 (mod n/ D 1 we
must find the next value r of x that again satisfies ax (mod n/ D 1

SECTION 8.5 Shor’s Algorithm

121

A number a is relatively prime to n iff4 the greatest common divisor of
a and n is equal to 1, written gcd.a; n/ D 1. We refer to these
functions as modular functions. The smallest value r of x greater than 0
satisfying f .x/ WD ax (modn/ is also referred to as the order of the
element a in the group .Z=nZ/ , which denotes the multiplicative group
whose underlying set is the subset of numbers in f1; 2; :::; n 1g
relatively prime to n, and whose binary operation is multiplication
modulo n, as above. Exercise Check that .Z=nZ/ , whose underlying set
of elements is the subset of numbers in f1; 2; :::; n 1g relatively
prime to n and whose binary operation is multiplication modulo n, is
actually a group! For any number n, how many elements does the group
.Z=nZ/ have? Can you find a pattern relating the number of elements in
.Z=nZ/ to the number n? 8.6

The fascinating point we make now is that the difficulty in finding the
period of the function f .x/ D 2x (mod 91/ is not unique to the human
experience. Even a classical computer would have a difficult time
finding the period of this function. Peter Shor realized that we can
exploit quantum computing to quickly find the period of such a function
\[254\]. We will now explain how the period of a function can be used as
an input to the factorization algorithm that would crack RSA
cryptography.

Period of a Function as an Input to a Factorization Algorithm Suppose we
are asked to factor some number n, and that we know how to find the
period of any modular function, as described above. Remember that the
problem of factoring n reduces to the simpler problem of finding any
factor of n. So, let’s see how we could leverage our ability to find the
period of a modular function to find a factor of n: 1. Choose a random
number a such that a &lt; n. 2. Compute gcd.a; n/ using the extended
Euclidean algorithm. 3. If gcd.a; n/ ¤ 1, i.e., a and n are not
relatively prime, a is already a nontrivial factor of n, and so we are
done. 4. Otherwise, find the period r of the modular function f .x/ WD
ax (modn/ r

5.  If r is an odd number, or if a 2 D number and start over. 4 Note:

1 (modn/, choose a new random

we abbreviate if and only if as iff throughout the book.

122

CHAPTER 8 The Canon: Code Walkthroughs r

6.  Otherwise, classical number theory guarantees that gcd.a 2 C 1; n/
    and r gcd.a 2 1; n/ are both nontrivial factors of n. Exercise

8.7

Run the above algorithm to factor the number n D 21.

A successful approach to the exercise above is the following: 1. begin
with a D 2, since 2. gcd.a; n/ D gcd.2; 21/ D 1, 3. (Step 3 is omitted,
since gcd.a; n/ D gcd.2; 21/ D 1), 4. the period of the modular function
f .x/ WD 2x (mod 21/ is found to be r D 6 and 5. r D 6 is neither an odd
number, nor does it satisfy the equation r

a2 D

1 (mod)n;

6.  r

6

gcd.a 2 C1; n/ D gcd.2 2 C1; 21/ D gcd.8C1; 21/ D gcd.9; 21/ D 3 and r

gcd.a 2

6

1; n/ D gcd.2 2

1; 21/ D gcd.23 1; 21/ D gcd.7; 21/ D 7

are the two nontrivial factors of n D 21. We now see that being able to
find the period of any modular function is the key to factoring. When we
use a quantum computer, we can build a circuit that finds the period
quite easily. This cirquit uses the quantum Fourier transform (QFT),
described earlier in this book. Shor was inspired by Simon’s algorithm
and BV in his development of this algorithm. He built on the use of the
QFT by BV and the period finding of Simon’s approach to then arrive at
his number-factoring algorithm.5 Here is the circuit diagram for Shor’s
algorithm: j0i



:: : j0i

H :: : H

j0i

H



j1i

=n

U a2

5 Please

 QFT2n1





:: :

 0

1

U a2



2n 1

U a2

see this book’s GitHub site for an example of code for Simon’s
algorithm.

SECTION 8.5 Shor’s Algorithm

123

Let us now do a walkthrough of Shor’s algorithm using Cirq. The code for
this walkthrough is available on the book’s website. We first import the
libraries we will use for this walkthrough. import fractions import math
import random import numpy as np import sympy from typing import
Callable, List, Optional, Sequence, Union import cirq

Classical order finding A function for classically computing the order r
of an element a 2 Z=nZ is provided below. This function simply computes
the sequence a2 mod n; a3 mod n; a4 mod n; :: : until an integer r is
found such that ar D 1 mod n. Since jZ=nZj D '.n/, this algorithm for
order finding has time complexity O.'.n// which is inefficient.
(Specifically, the time complexity is roughly O.2L=2 / where L is the
number of bits in n.) def classical\_order\_finder(a: int, n: int) -&gt;
Optional\[int\]: """Computes smallest positive r such that a**r mod n ==
1.""" \# Make sure a is both valid and in Z/nZ if a &lt; 2 or a &gt;= n
or math.gcd(a, n) &gt; 1: raise ValueError(f"Invalid a={a} for modulus
n={n}.") \# Determine the order r, x = 1, a while x != 1: x = (a**r) % n
r += 1 return r

An example of computing r for a given a 2 Z=nZ and given n is shown in
the code block below. """Example of (classically) computing the order of
an element.""" n = 15 \# The multiplicative group is \[1, 2, 4, 7, 8,
11, 13, 14\]

124

CHAPTER 8 The Canon: Code Walkthroughs

a = 8 r = classical\_order\_finder(a, n) \# Check that the order is
indeed correct print(f"a\^r mod n = {a}\^{r} mod {n} = {a\*\*r % n}")

The output of this code block is: a\^r mod n = 8\^4 mod 15 = 1

Quantum order finding The quantum computing portion of Shor’s algorithm
accomplishes the order finding. Quantum order finding is essentially
quantum phase estimation with a unitary U that computes the modular
exponential function fa .z/ for some randomly chosen a 2 Z=nZ. The full
details of how U is computed in terms of elementary gates can be complex
to unravel, especially on a first reading. In this tutorial, we’ll use
arithmetic operations in Cirq which can implement such a unitary U
without fully delving into the details of elementary gates. Below we
first show a simple example of an arithmetic operation in Cirq
(addition) then discuss the operation we care about (modular
exponentiation).

Quantum arithmetic operations in Cirq Here we discuss an example of
defining an arithmetic operation in Cirq. This operation adds the value
of the input register into the target register. More specifically, this
operation acts on two qubit registers as jaii jbit 7! jaii ja C b mod Nt
it :

(8.8)

Here, the subscripts i and t denote input and target register,
respectively, and Nt is the dimension of the target register. To define
this operation, called Adder, we inherit from the pre-defined class
cirq.ArithmeticOperation and override the four methods shown below. The
main method is the apply method which defines the arithmetic. Here, we
simply state the expression as aCb instead of the more accurate aCb mod
Nt above — the cirq.ArithmeticOperation class is able to deduce what we
mean by simply a C b since the operation must be reversible. """Example
of defining an arithmetic (quantum) operation in Cirq.""" class
Adder(cirq.ArithmeticOperation): """Quantum addition.""" def
**init**(self, target\_register, input\_register):

SECTION 8.5 Shor’s Algorithm

125

self.input\_register = input\_register self.target\_register =
target\_register def registers(self): return self.target\_register,
self.input\_register def with\_registers(self, *new\_registers): return
Add(*new\_registers) def apply(self, target\_value, input\_value):
return target\_value + input\_value

Now that we have the class defined, we can use it in a circuit. The cell
below creates two qubit registers, then sets the first register to be
j10i (in binary) and the second register to be j01i (in binary) via X
gates. Then, we use the Adder operation, then measure all the qubits.
Since 10 C 01 D 11 (in binary), we expect to measure j11i in the target
register every time. Additionally, since we do not alter the input
register, we expect to measure j10i in the input register every time. In
short, the only bitstring we expect to measure is 1011. """Example of
using an Adder in a circuit.""" \# Two qubit registers qreg1 =
cirq.LineQubit.range(2) qreg2 = cirq.LineQubit.range(2, 4) \# Define the
circuit circ = cirq.Circuit( cirq.ops.X.on(qreg1\[0\]),
cirq.ops.X.on(qreg2\[1\]), Adder(input\_register=qreg1,
target\_register=qreg2), cirq.measure\_each(*qreg1),
cirq.measure\_each(*qreg2) ) \# Display it print("Circuit:\n")
print(circ) \# Print the measurement outcomes
print("\n\nMeasurement outcomes:\n") print(cirq.sample(circ,
repetitions=5).data)

The output of this code block is shown below: Circuit: 0:
---X---\#3------------------------------------------M--| 1:
-------\#4------------------------------------------M--| 2:
-------&lt;**main**.Adder object at 0x7fb5bb147be0&gt;---M---

126

CHAPTER 8 The Canon: Code Walkthroughs

| 3: ---X---\#2------------------------------------------M---

Measurement outcomes:

0 1 2 3 4

0 1 1 1 1 1

1 0 0 0 0 0

2 1 1 1 1 1

3 1 1 1 1 1

In the output, we first see the circuit which shows the initial X gates,
the Adder operation, then the final measurements. Next, we see the
measurement outcomes which are all the bitstring 1011 as expected. It is
also possible to see the unitary of the adder operation, which we do
below. Here, we set the target register to be two qubits in the zero
state, i.e. j00i. We specify the input register as the integer one which
corresponds to the qubit register j01i. """Example of the unitary of an
Adder operation.""" cirq.unitary(
Adder(target\_register=cirq.LineQubit.range(2), input\_register=1)
).astype(np.int32)

The output is: array(\[\[0, 0, 0, 1\], \[1, 0, 0, 0\], \[0, 1, 0, 0\],
\[0, 0, 1, 0\]\], dtype=int32)

We can understand this unitary as follows. The i th column of the
unitary is the state ji C 1 mod 4i. For example, if we look at the 0th
column of the unitary, we see the state ji C 1 mod 4i D j0 C 1 mod 4i D
j1i. If we look at the 1st column of the unitary, we see the state ji C
1 mod 4i D j1 C 1 mod 4i D j2i. Similarly for the last two columns.

Modular exponential arithmetic operation We can define the modular
exponential arithmetic operation in a similar way to the simple addition
arithmetic operation, shown below. For the purposes of understanding
Shor’s algorithm, the most important part of the following code block is
the apply method which defines the arithmetic operation.

SECTION 8.5 Shor’s Algorithm

127

class ModularExp(cirq.ArithmeticOperation): """Quantum modular
exponentiation. This class represents the unitary which multiplies base
raised to exponent into the target modulo the given modulus. More
precisely, it represents the unitary V which computes modular
exponentiation a**e mod n: V|y&gt;|e&gt; = |y \* a**e mod n&gt; |e&gt; 0
&lt;= y &lt; n V|y&gt;|e&gt; = |y&gt; |e&gt; n &lt;= y where y is the
target register, e is the exponent register, a is the base and n is the
modulus. Consequently, V|y&gt;|e&gt; = (U\*\*e|r&gt;)|e&gt; where U is
the unitary defined as U|y&gt; = |y \* a mod n&gt; 0 &lt;= y &lt; n
U|y&gt; = |y&gt; n &lt;= y """ def **init**( self, target:
Sequence\[cirq.Qid\], exponent: Union\[int, Sequence\[cirq.Qid\]\],
base: int, modulus: int ) -&gt; None: if len(target) &lt;
modulus.bit\_length(): raise ValueError(f’Register with {len(target)}
qubits is too small ’ f’for modulus {modulus}’) self.target = target
self.exponent = exponent self.base = base self.modulus = modulus def
registers(self) -&gt; Sequence\[Union\[int, Sequence\[cirq.Qid\]\]\]:
return self.target, self.exponent, self.base, self.modulus def
with\_registers( self, \*new\_registers: Union\[int,
Sequence\[’cirq.Qid’\]\], ) -&gt; cirq.ArithmeticOperation: if
len(new\_registers) != 4: raise ValueError(f’Expected 4 registers
(target, exponent, base, ’ f’modulus), but got {len(new\_registers)}’)
target, exponent, base, modulus = new\_registers if not
isinstance(target, Sequence): raise ValueError( f’Target must be a qubit
register, got {type(target)}’) if not isinstance(base, int): raise
ValueError( f’Base must be a classical constant, got {type(base)}’)

128

CHAPTER 8 The Canon: Code Walkthroughs if not isinstance(modulus, int):
raise ValueError( f’Modulus must be a classical constant, got
{type(modulus)}’) return ModularExp(target, exponent, base, modulus)

def apply(self, *register\_values: int) -&gt; int: assert
len(register\_values) == 4 target, exponent, base, modulus =
register\_values if target &gt;= modulus: return target return (target *
base\*\*exponent) % modulus def *circuit\_diagram\_info*( self, args:
cirq.CircuitDiagramInfoArgs, ) -&gt; cirq.CircuitDiagramInfo: assert
args.known\_qubits is not None wire\_symbols: List\[str\] = \[\] t, e =
0, 0 for qubit in args.known\_qubits: if qubit in self.target: if t ==
0: if isinstance(self.exponent, Sequence): e\_str = ’e’ else: e\_str =
str(self.exponent) wire\_symbols.append(
f’ModularExp(t\*{self.base}\*\*{e\_str} % {self.modulus})’) else:
wire\_symbols.append(’t’ + str(t)) t += 1 if isinstance(self.exponent,
Sequence) and qubit in self.exponent: wire\_symbols.append(’e’ + str(e))
e += 1 return
cirq.CircuitDiagramInfo(wire\_symbols=tuple(wire\_symbols))

In the apply method, we see that we evaluate (target \*
base\*\*exponent) % modulus. The target and the exponent depend on the
values of the respective qubit registers, and the base and modulus are
constant — namely, the modulus is n and the base is some a 2 Z=nZ. Now
we can see an example of the modular exponential unitary — or at least
part of it! The total number of qubits we will use is 3.L C 1/ where L
is the number of bits needed to store the integer n to factor. The size
of the unitary which implements the modular exponential is thus 43.LC1/
. For a modest n D 15, the unitary requires storing 230 floating point
numbers in memory which is out of reach of most current standard
laptops.

SECTION 8.5 Shor’s Algorithm

129

"""Create the target and exponent registers for phase estimation, and
see the number of qubits needed for Shor’s algorithm. """ n = 15 L =
n.bit\_length() \# The target register has L qubits target =
cirq.LineQubit.range(L) \# The exponent register has 2L + 3 qubits
exponent = cirq.LineQubit.range(L, 3 \* L + 3) \# Display the total
number of qubits to factor this n print(f"To factor n = {n} which has L
= {L} bits, we need 3L + 3 = {3 \* L + 3} qubits.")

The output of this code block is: To factor n = 15 which has L = 4 bits,
we need 3L + 3 = 15 qubits.

As with the simple adder operation, this modular exponential operation
has a unitary which we can display (memory permitting) as follows.
"""See (part of) the unitary for a modular exponential operation.""" \#
Pick some element of the multiplicative group modulo n a = 5 \# Display
(part of) the unitary. Uncomment if n is small enough \#
cirq.unitary(ModularExp(target, exponent, a, n))

Using the modular exponential operation in a circuit The quantum part of
Shor’s algorithm is just phase estimation with the unitary U
corresponding to the modular exponential operation. The following cell
defines a function which creates the circuit for Shor’s algorithm using
the ModularExp operation we defined above. """Function to make the
quantum circuit for order finding.""" def
make\_order\_finding\_circuit(a: int, n: int) -&gt; cirq.Circuit:
"""Returns quantum circuit which computes the order of a modulo n. The
circuit uses Quantum Phase Estimation to compute an eigenvalue of the
unitary U|y&gt; = |y \* a mod n&gt; 0 &lt;= y &lt; n U|y&gt; = |y&gt; n
&lt;= y """ L = n.bit\_length() target = cirq.LineQubit.range(L)
exponent = cirq.LineQubit.range(L, 3 \* L + 3) return cirq.Circuit(

130

CHAPTER 8 The Canon: Code Walkthroughs cirq.X(target\[L - 1\]),
cirq.H.on\_each(*exponent), ModularExp(target, exponent, a, n),
cirq.QFT(*exponent, inverse=True), cirq.measure(\*exponent,
key=’exponent’),

)

We can visualize this circuit as follows. """Example of the quantum
circuit for period finding.""" n = 15 x = 7 circuit =
make\_order\_finding\_circuit(a, n) print(circuit)

As previously described, we put the exponent register into an equal
superposition via Hadamard gates. The X gate on the last qubit in the
target register is used for phase kickback. The modular exponential
operation performs the sequence of controlled unitaries in phase
estimation, then we apply the inverse QFT to the exponent register and
measure to read out the result. To illustrate the measurement results,
we can sample from a smaller circuit. """Measuring Shor’s period finding
circuit.""" circuit = make\_order\_finding\_circuit(a=5, n=6) res =
cirq.sample(circuit, repetitions=8) print("Raw measurements:")
print(res) print("\nInteger in exponent register:") print(res.data)

The output of this code block is: Raw measurements: exponent=00001010,
00000000, 00000000, 00000000, 00000000, 00000000, 00000000, 00000000,
00000000 Integer in exponent register: exponent 0 0 1 0 2 0 3 0 4 256 5
0 6 256 7 0

SECTION 8.5 Shor’s Algorithm

131

We interpret each measured bitstring as an integer, but what do these
integers tell us? In the next section we look at how to classically
post-process to interpret them.

Classical post-processing The integer we measure is close to s=r where r
is the order of a 2 Z=nZ and 0  s &lt; r is an integer. We use the
continued fractions algorithm to determine r from s=r then return it if
the order finding circuit succeeded, else we return None. def
process\_measurement(result: cirq.Result, a: int, n: int) -&gt;
Optional\[int\]: """Interprets the output of the order finding circuit.
Specifically, it determines s/r such that exp(2 pi is/r) is an
eigenvalue of the unitary U|y&gt; = |ay mod n&gt; 0 &lt;= y &lt; n
U|y&gt; = |y&gt; n &lt;= y then computes r (by continued fractions) if
possible, and returns it. Args: result: trial result obtained by
sampling the output of the circuit built by
make\_order\_finding\_circuit Returns: r, the order of a modulo n or
None. """ \# Read the output integer of the exponent register
exponent\_as\_integer = result.data\["exponent"\]\[0\]
exponent\_num\_bits = result.measurements\["exponent"\].shape\[1\]
eigenphase = float(exponent\_as\_integer / 2**exponent\_num\_bits) \#
Run the continued fractions algorithm to determine f = s / r f =
fractions.Fraction.from\_float(eigenphase).limit\_denominator(n) \# If
the numerator is zero, the order finder failed if f.numerator == 0:
return None \# Else, return the denominator if it is valid r =
f.denominator if a**r % n != 1: return None return r

The next code block shows an example of creating an order finding
circuit, executing it, then using the classical postprocessing function
to determine

132

CHAPTER 8 The Canon: Code Walkthroughs

the order. Recall that the quantum part of the algorithm succeeds with
some probability. If the order is None, the code needs to be run again.
"""Example of the classical post-processing.""" \# Set n and a here n =
6 a = 5 print(f"Finding the order of a = {a} modulo n = {n}\n")
measurement = cirq.sample(circuit, repetitions=1) print("Raw
measurements:") print(measurement) print("\nInteger in exponent
register:") print(measurement.data) r =
process\_measurement(measurement, a, n) print("\nOrder r =", r) if r is
not None: print(f"a\^r mod n = {a}\^{r} mod {n} = {a\*\*r % n}")

The output of a successful run of this code block is shown below:
Finding the order of a = 5 modulo n = 6 Raw measurements: exponent=1, 0,
0, 0, 0, 0, 0, 0, 0 Integer in exponent register: exponent 0 256 Order r
= 2 a\^r mod n = 5\^2 mod 6 = 1

Quantum order finder We can now define a streamlined function for the
quantum version of order finding using the functions we have previously
written. The quantum order finder below creates the circuit, executes
it, and processes the measurement result. def quantum\_order\_finder(a:
int, n: int) -&gt; Optional\[int\]: """Computes smallest positive r such
that a\*\*r mod n == 1. Args: a: integer whose order is to be computed,
must be greater than one and belong to the multiplicative group of
integers modulo n (which consists of positive integers relatively prime
to n), n: modulus of the multiplicative group. Returns:

SECTION 8.5 Shor’s Algorithm

133

Smallest positive integer r such that a\*\*r == 1 mod n or None if the
algorithm failed. The algorithm fails when the result of the Quantum
Phase Estimation is inaccurate, zero or a reducible fraction. Raises:
ValueError when x is 1 or not an element of the multiplicative group of
integers modulo n. """ \# Check that the integer a is a valid element of
the multiplicative group modulo n if a &lt; 2 or n &lt;= a or
math.gcd(a, n) &gt; 1: raise ValueError(f’Invalid a={a} for modulus
n={n}.’) \# Create the order finding circuit circuit =
make\_order\_finding\_circuit(a, n) \# Sample from the order finding
circuit measurement = cirq.sample(circuit) \# Return the processed
measurement result return process\_measurement(measurement, a, n)

This completes our quantum implementation of an order finder.

The complete factoring algorithm We can use this quantum order finder
(or the classical order finder) to complete Shor’s algorithm. In the
following code block, we add a few pre-processing steps which 1. Check
if n is even, 2. Check if n is prime, 3. Check if n is a prime power,
all of which can be done efficiently. Additionally, we add the last
necessary post-processing step which uses the order r to compute a
non-trivial factor p of n. This is achieved by computing y D ar=2 mod n
(assuming r is even), then computing p D gcd.y 1; n/. """Functions for
factoring from start to finish.""" def find\_factor\_of\_prime\_power(n:
int) -&gt; Optional\[int\]: """Returns non-trivial factor of n if n is a
prime power, else None.""" for k in range(2, math.floor(math.log2(n)) +
1): c = math.pow(n, 1 / k) c1 = math.floor(c) if c1**k == n: return c1
c2 = math.ceil(c) if c2**k == n: return c2

134

CHAPTER 8 The Canon: Code Walkthroughs

return None

def find\_factor( n: int, order\_finder: Callable\[\[int, int\],
Optional\[int\]\] = quantum\_order\_finder, max\_attempts: int = 30 )
-&gt; Optional\[int\]: """Returns a non-trivial factor of composite
integer n. Args: n: Integer to factor. order\_finder: Function for
finding the order of elements of the multiplicative group of integers
modulo n. max\_attempts: number of random a’s to try, also an upper
limit on the number of order\_finder invocations. Returns: Non-trivial
factor of n or None if no such factor was found. Factor k of n is
trivial if it is 1 or n. """ \# If the number is prime, there are no
non-trivial factors if sympy.isprime(n): print("n is prime!") return
None \# If the number is even, two is a non-trivial factor if n % 2 ==
0: return 2 \# If n is a prime power, we can find a non-trivial factor
efficiently c = find\_factor\_of\_prime\_power(n) if c is not None:
return c for \_ in range(max\_attempts): \# Choose a random number
between 2 and n - 1 a = random.randint(2, n - 1) \# Most likely a and n
will be relatively prime c = math.gcd(a, n) \# If a and n are not
relatively prime, we got lucky and found a non-trivial factor if 1 &lt;
c &lt; n: return c \# Compute the order r of a modulo n using the order
finder r = order\_finder(a, n) \# If the order finder failed, try again
if r is None: continue \# If the order r is even, try again

SECTION 8.6 Grover’s Search Algorithm

135

if r % 2 != 0: continue \# Compute the non-trivial factor y = a\*\*(r //
2) % n assert 1 &lt; y &lt; n c = math.gcd(y - 1, n) if 1 &lt; c &lt; n:
return c print(f"Failed to find a non-trivial factor in {max\_attempts}
attempts.") return None

The function find\_factor uses the quantum\_order\_finder by default, in
which case it is executing Shor’s algorithm. As previously mentioned,
due to the large memory requirements for classically simulating this
circuit, we cannot run Shor’s algorithm for n  15. However, we can use
the classical order finder as a substitute. """Example of factoring via
Shor’s algorithm (order finding).""" \# Number to factor n = 184573 \#
Attempt to find a factor p = find\_factor(n,
order\_finder=classical\_order\_finder) q = n // p print("Factoring n =
pq =", n) print("p =", p) print("q =", q)

The output of this code block is: Factoring n = pq = 184573 p = 487 q =
379

We can easily check that n D pq, as claimed.

8.6

Grover’s Search Algorithm

In 1996, Lov Grover demonstrated that we can obtain a quadratic speedup
in algorithmic unstructured search on a quantum computer compared with a
classical one \[130\]. While this is not exponential speedup, it is
still significant. The search problem can be set up as follows. Let say
we have a dataset of n numbers and where there is one number which we
are searching for

136

CHAPTER 8 The Canon: Code Walkthroughs

which we will call n . We set up this search challenge as a algorithmic
search protocol which means that the method by which we know we have
found the number we want is to act upon that number with a certain
function; if the output of the function is 1 we have found our number;
if the output is 0 we have not yet found our number. If we had to search
for one unique number n amongst n numbers then we would have to search
on average n2 times and an upper bound of the worst case time complexity
would be O.n/. However, on a quantum computer we can achieve a better
result; we can find our desired unique element with a p time complexity
of O n with Grover’s algorithm. Furthermore, Bennett et al. showed that
any such algorithm which solves an algorithmic search problem running on
a quantum computer would query the oracle at best p O. n/; Grover’s
algorithm is therefore optimal \[31\]. Grover’s algorithm is more
involved than DJ and BV. Here are the steps of the algorithm: 
Initialize to Uniform Superposition: We initialize the input register
with a state of superposition in which all entries are equally likely.
If we have, for example, four numbers in our dataset we can initialize
the state of our quantum register of two qubits as follows 1 1 1 1 j00i
C j01i C j10i C j11i 2 2 2 2 (If we had eight elements in our dataset we
would need three qubits, etc). As you can see, since the amplitudes are
all equal, the probability of yielding any of the states upon
measurement at this point in the circuit is equal. As we recall, the
probability of finding the state upon measurement of the superposition
of states is given by Born’s rule, i.e., the square of the modulus of
the amplitude. In this case, since each amplitude is 12 , therefore each
state has a probability of 14 or 25%. So we must act upon this equal
superposition in some way that increases the amplitude of the state
vector which represents our desired number n while decreasing the other
amplitudes and we must do so in a way that still satisfies Born’s rule
of normalizing to a total probability of one. Let us recall that
according to Born’s rule, if we have the state j iD

j i D ˛ j0i C ˇ j1i then the amplitudes ˛ and ˇ must satisfy the
following condition j˛j2 C jˇj2 D 1

SECTION 8.6 Grover’s Search Algorithm

137

 Phase Inversion: In this step we will apply a unitary operator to the
superposition of all states and flip the sign of the amplitude in front
of the state which represents n , the number we are searching for. We
call this operator the oracle since we can consider it as a black box
function.  Inversion About the Mean (or Amplitude Amplification): In
this step we apply another unitary operator which takes each amplitude
and adjusts it so that if it was y amount above the mean, now it is y
amount below the mean or vice-versa. We call this operator the Grover
diffusion operator. Recall from the phase inversion step that we
inverted the sign of the amplitude of the state vector associated with
n so when we now invert about the mean, we flip this particular
amplitude way above the mean. To be more rigorous, it flips it p2n over
the mean. We then iterate, repeating phase inversion and inversion about
the mean so that this amplitude keeps getting larger, while the other
amplitudes get progressively smaller.  Measurement: When we measure
after a series of iterations, the probability of collapsing the
superposition to our desired result is now quite p high. At most we have
to iterate n times; we now see how Grover’s p algorithm has a worst case
time complexity of O. n/. As with other algorithms we have examined, we
prepare our data input qubits in state j0i and our output qubit in state
j1i. We then apply H to all data input qubits in order to initialize
them in an equal superstition state and also apply a Hadamard to the
output qubit. We then apply the unitary oracle operator followed by
iterations of the diffusion operator. Finally, we perform the
measurement and find our answer. Here is an example circuit diagram of
Grover’s algorithm with two input qubits: j0i

H

j0i

H

j1i

H

oracle

H

X

H

X

 H

H

X

H

X

H

Below are two examples of Grover’s algorithm – the comments in the code
give the reader guidance on which step is being implemented. Note that
in these simple examples, the code only implements one iteration of the
diffusion operator. Once larger quantum computers are available on the
cloud, we will post code examples on the companion online site of more
realistic implementations with larger datasets. See also \[56\] and
\[57\] for a generalization

138

CHAPTER 8 The Canon: Code Walkthroughs

Figure 8.5: Plotting Grover’s algorithm as it closes in on the target

Source: Wikimedia

of Grover’s algo and can be classified as an amplitude amplification
algorithm. See also Yoder, et al. for a dicussion of fixed point quantum
search \[306\] code source: \[81\] """Grover’s algorithm in Cirq""" \#
Imports import random import cirq

def set\_io\_qubits(qubit\_count): """Add the specified number of input
and output qubits.""" input\_qubits = \[cirq.GridQubit(i, 0) for i in
range(qubit\_count)\] output\_qubit = cirq.GridQubit(qubit\_count, 0)
return (input\_qubits, output\_qubit)

def make\_oracle(input\_qubits, output\_qubit, x\_bits): """Implement
function {f(x) = 1 if x==x’, f(x) = 0 if x!= x’}.""" \# Make oracle. \#
for (1, 1) it’s just a Toffoli gate \# otherwise negate the zero-bits.
yield(cirq.X(q) for (q, bit) in zip(input\_qubits, x\_bits) if not bit)
yield(cirq.TOFFOLI(input\_qubits\[0\], input\_qubits\[1\],
output\_qubit)) yield(cirq.X(q) for (q, bit) in zip(input\_qubits,
x\_bits) if not bit)

def make\_grover\_circuit(input\_qubits, output\_qubit, oracle):

SECTION 8.6 Grover’s Search Algorithm

139

"""Find the value recognized by the oracle in sqrt(N) attempts.""" \#
For 2 input qubits, that means using Grover operator only once. c =
cirq.Circuit() \# Initialize qubits. c.append(\[ cirq.X(output\_qubit),
cirq.H(output\_qubit), cirq.H.on\_each(\*input\_qubits),\]) \# Query
oracle. c.append(oracle) \# Construct Grover operator.
c.append(cirq.H.on\_each(*input\_qubits))
c.append(cirq.X.on\_each(*input\_qubits))
c.append(cirq.H.on(input\_qubits\[1\]))
c.append(cirq.CNOT(input\_qubits\[0\], input\_qubits\[1\]))
c.append(cirq.H.on(input\_qubits\[1\]))
c.append(cirq.X.on\_each(*input\_qubits))
c.append(cirq.H.on\_each(*input\_qubits)) \# Measure the result.
c.append(cirq.measure(\*input\_qubits, key=’result’)) return c

def bitstring(bits): return ’’.join(str(int(b)) for b in bits)

def main(): qubit\_count = 2 circuit\_sample\_count = 10 \#Set up input
and output qubits. (input\_qubits, output\_qubit) =
set\_io\_qubits(qubit\_count) \#Choose the x’ and make an oracle which
can recognize it. x\_bits = \[random.randint(0, 1) for \_ in
range(qubit\_count)\] print(’Secret bit sequence: {}’.format(x\_bits))
\# Make oracle (black box) oracle = make\_oracle(input\_qubits,
output\_qubit, x\_bits) \# Embed the oracle into a quantum circuit
implementing Grover’s algorithm. circuit =
make\_grover\_circuit(input\_qubits, output\_qubit, oracle)
print(’Circuit:’) print(circuit) \# Sample from the circuit a couple
times. simulator = cirq.Simulator() result = simulator.run(circuit,
repetitions=circuit\_sample\_count)

140

CHAPTER 8 The Canon: Code Walkthroughs

frequencies = result.histogram(key=’result’, fold\_func=bitstring)
print(’Sampled results:\n{}’.format(frequencies)) \# Check if we
actually found the secret value. most\_common\_bitstring =
frequencies.most\_common(1)\[0\]\[0\] print(’Most common bitstring:
{}’.format(most\_common\_bitstring)) print(’Found a match: {}’.format(
most\_common\_bitstring == bitstring(x\_bits)))

if **name** == ’**main**’: main()

We now run the code and obtain this as an example output: """ ===
EXAMPLE OUTPUT === Secret bit sequence: \[1, 0\] Sampled results:
Counter({’10’: 10}) Most common bitstring: 10 Found a match: True """

Grover’s Algorithm in Qiskit source: \[228\] \#initialization import
matplotlib.pyplot as plt import numpy as np \# importing Qiskit from
qiskit import IBMQ, Aer, assemble, transpile from qiskit import
QuantumCircuit, ClassicalRegister, QuantumRegister from
qiskit.providers.ibmq import least\_busy \# import basic plot tools from
qiskit.visualization import plot\_histogram n = 2 grover\_circuit =
QuantumCircuit(n) def initialize\_s(qc, qubits): """Apply a H-gate to
’qubits’ in qc""" for q in qubits: qc.h(q) return qc grover\_circuit =
initialize\_s(grover\_circuit, \[0,1\]) grover\_circuit.draw()
grover\_circuit.cz(0,1) \# Oracle

SECTION 8.6 Grover’s Search Algorithm grover\_circuit.draw() \#
Diffusion operator (U\_s) grover\_circuit.h(\[0,1\])
grover\_circuit.z(\[0,1\]) grover\_circuit.cz(0,1)
grover\_circuit.h(\[0,1\]) grover\_circuit.draw() sv\_sim =
Aer.get\_backend(’statevector\_simulator’) qobj =
assemble(grover\_circuit) result = sv\_sim.run(qobj).result() statevec =
result.get\_statevector() from qiskit\_textbook.tools import
vector2latex vector2latex(statevec, pretext="|\\psi\\rangle =")
grover\_circuit.measure\_all() qasm\_sim =
Aer.get\_backend(’qasm\_simulator’) qobj = assemble(grover\_circuit)
result = qasm\_sim.run(qobj).result() counts = result.get\_counts()
plot\_histogram(counts)

3-Qubit Grover’s Algo See \[113\] for a discussion of this algorithm.
source: \[228\] qc = QuantumCircuit(3) qc.cz(0, 2) qc.cz(1, 2)
oracle\_ex3 = qc.to\_gate() oracle\_ex3.name = "U$_\omega$"

def diffuser(nqubits): qc = QuantumCircuit(nqubits) \# Apply
transformation |s&gt; -&gt; |00..0&gt; (H-gates) for qubit in
range(nqubits): qc.h(qubit) \# Apply transformation |00..0&gt; -&gt;
|11..1&gt; (X-gates) for qubit in range(nqubits): qc.x(qubit) \# Do
multi-controlled-Z gate qc.h(nqubits-1) qc.mct(list(range(nqubits-1)),
nqubits-1) \# multi-controlled-toffoli qc.h(nqubits-1) \# Apply
transformation |11..1&gt; -&gt; |00..0&gt; for qubit in range(nqubits):
qc.x(qubit) \# Apply transformation |00..0&gt; -&gt; |s&gt; for qubit in
range(nqubits): qc.h(qubit)

p  100 2

142

CHAPTER 8 The Canon: Code Walkthroughs

We will return the diffuser as a gate
=====================================

U\_s = qc.to\_gate() U\_s.name = "U$_s$" return U\_s

n = 3 grover\_circuit = QuantumCircuit(n) grover\_circuit =
initialize\_s(grover\_circuit, \[0,1,2\])
grover\_circuit.append(oracle\_ex3, \[0,1,2\])
grover\_circuit.append(diffuser(n), \[0,1,2\])
grover\_circuit.measure\_all() grover\_circuit.draw()

qasm\_sim = Aer.get\_backend(’qasm\_simulator’)
transpiled\_grover\_circuit = transpile(grover\_circuit, qasm\_sim) qobj
= assemble(transpiled\_grover\_circuit) results =
qasm\_sim.run(qobj).result() counts = results.get\_counts()
plot\_histogram(counts)

See \[228\] for an example of using Grovers’ algorithm for a Sudoku
puzzle.

Summary In this chapter, we have explored the set of canonical quantum
algorithms. These breakthroughs from the 1980’s and 1990’s established
the potential for quantum advantage. While we still do not have the
hardware to run Shor’s and Grover’s algorithms with meaningful scale,
they are powerful reminders of what is to come. In the next chapter we
will cover a range of quantum computing methods for NISQ regime quantum
computers. We will also explore the emerging understanding of the
unification of the various algos we discussed in this chapter. While
search, factoring and simulation may seem to be very different types of
algos, we can unify them in a common framework of quantum singular value
transforms (QSVT) which we shall explore in the next chapter.

CHAPTER

9 Quantum Computing Methods In this section we will walk through a range
of quantum computing programs that can be run on NISQ processors. We
will cover methods in optimization, chemistry, machine learning and
other areas.

9.1

Variational Quantum Eigensolver

Let us first examine a variational quantum eigensolver (VQE) \[218\]. We
can use a VQE to find the eigenvalues of a large matrix that represents
the Hamiltonian of a system. In many cases, we are looking for the
lowest eigenvalue, which represents the ground state energy of the
system. We can also use VQE and VQE-type algorithms to calculate
additional eigenvalues, which represent excited state energies \[193,
144\]. VQE is a good example of a hybrid classical/quantum approach to
solving a problem (for more on VQEs see \[218, 293, 211, 288, 256\]).
While the VQE was initially developed to find ground states of
Hamiltonians, we can use it to find the minimum of any given objective
function that we can express in a quantum circuit. This broadens the
application space significantly for this variational method. See also
\[67\] for a broad review of variational quantum algorithms. In
variational methods, we start with a best guess, or ansatz, for the
ground state. More specifically we parameterize a quantum state j ./i
where  is a set of parameters. The problem that VQE solves is as
follows: Given a Hamiltonian H , conventionally coming from a physical
system such as molecular hydrogen or water, approximate the ground state
energy (minimum eigenvalue of H ) by solving the following optimization
problem © The Author(s), under exclusive license to Springer Nature
Switzerland AG 2021 J. D. Hidary, Quantum Computing: An Applied
Approach, https://doi.org/10.1007/978-3-030-83274-2\_9

143

144

CHAPTER 9 Quantum Computing Methods

min h ./j H j . /i 

(9.1)

By the variational principle of quantum mechanics, the quantity h ./j H
j ./i can never be smaller than the ground state energy. So, by
minimizing this quantity, we get an approximation of the ground state
energy. In the VQE algorithm, j ./i is prepared on a quantum computer,
so the ansatz is typically developed from parametrized quantum gates;
for example, the rotation gates R .'/ where  is a Pauli operator, as
well as other “static” quantum gates like CNOT or controlled-Z. For the
purposes of VQE, we will assume our Hamiltonian is written as the sum of
tensor products of Pauli operators weighted by constant coefficients as
per \[193\]. m X H D ci Hi (9.2) i D1

Note that the tensor products of Pauli operators form a basis for
Hermitian matrices, so in principle any Hamiltonian can be expressed in
this way. However, this may lead to a number of terms exponential in the
system size. For this general case, different representations are
crucial for limiting the number of terms in the Hamiltonian and thus
limiting the number of resources required for the quantum algorithm. For
the present discussion, we will restrict our attention to Hamiltonians
of the form (9.2) where m grows at most polynomially in the system size
— that is, m D O.nk / — which is a reasonable assumption for many
physical systems of interest. The VQE algorithm computes expectation
values of each term Hi using a quantum circuit, then adds the total
energy classically. The classical optimizer changes the values of the
ansatz wavefunction to minimize the total energy. Once an approximate
minimum is found, the VQE returns the ground state energy as well as its
eigenstate. Another application of VQEs is error-mitigation. McClean et
al. explore this aspect of VQEs: Here, we provide evidence for the
conjecture that variational approaches can automatically suppress even
non-systematic decoherence errors by introducing an exactly solvable
channel model of variational state preparation. Moreover, we show how
variational quantum-classical approaches fit in a more general

SECTION 9.1 Variational Quantum Eigensolver

145

hierarchy of measurement and classical computation that allows one to
obtain increasingly accurate solutions with additional classical
resources \[191\]. We recommend the reader explore the use of subspace
expansion to achieve error-mitigation in the growing body of literature
on this subject \[190\]. Below, we show a program implementing VQE for a
simple Hamiltonian using pyQuil and the Grove library \[129\].1 Let us
walk through this program in steps and explain each part. First, we
import the necessary packages and connect to the quantum virtual machine
(QVM). \# Imports import numpy as np import matplotlib.pyplot as plt
from scipy.optimize import minimize from pyquil.quil import Program
import pyquil.api as api from pyquil.paulis import sZ from pyquil.gates
import RX, X, MEASURE from grove.pyvqe.vqe import VQE

We then set up an ansatz, which in this case is the rotation matrix
around the x-axis with a single parameter. \# Function to create the
ansatz def small\_ansatz(params): """Returns an ansatz Program with one
parameter.""" return Program(RX(params\[0\], 0)) \# Show the ansatz with
an example value for the parameter print("Ansatz with example value for
parameter:") print(small\_ansatz(\[1.0\]))

The output of this portion of the program showing the ansatz as a pyQuil
circuit is shown below. Ansatz with example value for parameter: RX(1.0)
0

Next, we set up a Hamiltonian; as we stated above, any Hamiltonian can
be expressed as a linear combination of tensor products of Pauli
operators, as these form a basis for Hermitian matrices. In practice,
Hamiltonians must first 1 Note that in this book we show code examples
in a range of QC frameworks; check the book’s online site for code
examples in other libraries as one can implement these methods and
algorithms in each of the frameworks.

146

CHAPTER 9 Quantum Computing Methods

be converted to qubit operators so that expectation values can be
measured using the quantum computer. If there are m non-trivial,
distinct terms in the Hamiltonian (9.2), then there are m distinct
expectation values to compute. Each quantum circuit in VQE computes one
expectation value, so there are m distinct quantum circuits to run. For
simplicity of instruction, we consider the simple case of one Pauli
operator H D Z (note that in this section H refers to a Hamiltonian and
not the Hadamard operator). We create an instance of the VQE algorithm
using the VQE class imported from Grove and compute the expectation
value for an example angle in the ansatz. \# Show the ansatz with an
example value for the parameter print("Ansatz with example value for
parameter:") print(small\_ansatz(\[1.0\])) \# Create a Hamiltonion H =
Z\_0 hamiltonian = sZ(0) \# Make an instance of VQE with a Nelder-Mead
minimizer vqe\_inst = VQE(minimizer=minimize,
minimizer\_kwargs={’method’: ’nelder-mead’}) \# Check the VQE manually
at a particular angle - say 2.0 radians angle = 2.0 print("Expectation
of Hamiltonian at angle = {}".format(angle))
print(vqe\_inst.expectation(small\_ansatz(\[angle\]), hamiltonian,
10000, qvm))

To get a picture of the landscape of the optimization problem, we can
sweep over a set of values in the range Œ0; 2/. Here, since we have
only one parameter in our ansatz, this is computationally inexpensive to
do. For larger ansatzes with more parameters, implementing a grid search
over all possible values is not feasible, and so classical optimization
algorithms must be used to find an approximate minimum. \# Loop over a
range of angles and plot expectation without sampling angle\_range =
np.linspace(0.0, 2.0 \* np.pi, 20) exact =
\[vqe\_inst.expectation(small\_ansatz(\[angle\]), hamiltonian, None,
qvm) for angle in angle\_range\] \# Plot the exact expectation
plt.plot(angle\_range, exact, linewidth=2) \# Loop over a range of
angles and plot expectation with sampling sampled =
\[vqe\_inst.expectation(small\_ansatz(\[angle\]), hamiltonian, 1000,
qvm) for angle in angle\_range\] \# Plot the sampled expectation

SECTION 9.1 Variational Quantum Eigensolver

147

Figure 9.1: Expectation value of the simple Hamiltonian H D Z at all
angles  2 Œ0; 2/ in the wavefunction ansatz j ./i D Rx ./ j0i

plt.plot(angle\_range, sampled, "-o") \# Plotting options
plt.xlabel(’Angle \[radians\]’) plt.ylabel(’Expectation value’)
plt.grid() plt.show()

The plot that this section of the program produces is shown in Figure
9.1. Here, we can visually see that the minimum energy (in arbitrary
units) of the Hamiltonian appears around the angle  D  in the
wavefunction ansatz. As mentioned, for larger Hamiltonians that require
more parameters in the ansatz, enumerating the expectation values for
all angles is not feasible. Instead, an optimization algorithm must be
used to traverse the optimization landscape and find, ideally, the
global minima. An example of the Nelder-Mead optimization algorithm,
implemented in the SciPy Optimize package, is shown below. \# Do the
minimization and return the best angle initial\_angle = \[0.0\] result =
vqe\_inst.vqe\_run(small\_ansatz, hamiltonian, initial\_angle, None,
qvm=qvm) print("\nMinimum energy =", round(result\["fun"\], 4))
print("Best angle =", round(result\["x"\]\[0\], 4))

The output for this final part of the program is Minimum energy = -1.0
Best angle = 3.1416

148

CHAPTER 9 Quantum Computing Methods

As can be seen, the optimizer is able to find the correct angle  D 
for the global minimum energy E D h j H j i D 1:0 (in arbitrary units).

VQE with Noise The VQE algorithm is designed to make effective use of
near-term quantum computers. It is therefore important to analyze its
performance in a noisy environment such as a NISQ processor. Above, we
used the noiseless QVM to simulate circuits in VQE. Now, we can consider
a QVM with a particular noise model and run the VQE algorithm again. A
code block setting up a noisy QVM in pyQuil — and demonstrating it is in
fact noisy — is shown below. Note that this program is an extension of
the previous program and assumes all packages are still imported. \#
Create a noise model which has a 10% chance of each gate at each
timestep pauli\_channel = \[0.1, 0.1, 0.1\] noisy\_qvm =
api.QVMConnection(gate\_noise=pauli\_channel) \# Check that the
simulator is indeed noisy p = Program(X(0), MEASURE(0, 0)) res =
noisy\_qvm.run(p, \[0\], 10) print(res)

The example output of this program (measuring the j1i state)
demonstrates that the simulator is indeed noisy — otherwise, we would
never see the bit 0 measured! "Outcome of NOT and MEASURE circuit on
noisy simulator:" \[\[0\], \[1\], \[1\], \[1\], \[0\], \[1\], \[1\],
\[1\], \[1\], \[0\]\]

Now that we have a noisy simulator, we can run the VQE algorithm under
noise. Here, we modify the classical optimizer to start with a larger
simplex so we don’t get stuck at an initial minimum. Then, we visualize
the same landscape plot (energy vs. angle) as before, but now in the
presence of noise. \# Update the minimizer in VQE to start with a larger
initial simplex vqe\_inst.minimizer\_kwargs = {"method": "Nelder-mead",
"options": {"initial\_simplex": np.array(\[\[0.0\], \[0.05\]\]),
"xatol": 1.0e-2} } \# Loop over a range of angles and plot expectation
with sampling

SECTION 9.1 Variational Quantum Eigensolver

149

Figure 9.2: Results of running VQE on a simulator with Pauli channel
noise.

sampled = \[vqe\_inst.expectation(small\_ansatz(\[angle\]), hamiltonian,
1000, noisy\_qvm) for angle in angle\_range\] \# Plot the sampled
expectation plt.plot(angle\_range, sampled, "-o") \# Plotting options
plt.title("VQE on a Noisy Simulator") plt.xlabel("Angle \[radians\]")
plt.ylabel("Expectation value") plt.grid() plt.show()

An example plot produced by this part of the program is shown in Figure
9.2. Here, we note that the landscape generally has the same shape but
is slightly distorted. The minimum value of the curve still occurs close
to the optimal value of  D , but the value of the energy here is
vertically shifted — the minimum energy here is approximately 0:6 (in
arbitrary units) whereas in the noiseless case the minimum energy was
1:0. However, since the minimum value still occurs around  D , VQE
displays some robustness to noise. The optimal parameters can still be
found, and the vertical offset in the minimum energy can be accounted
for in classical postprocessing. Pauli channel noise is not the only
noise model we can consider. In the book’s online site, this VQE program
also demonstrates a noisy simulator with measurement noise. We find that
the VQE is robust to measurement noise in the same sense as above — the
landscape curve has the same general

150

CHAPTER 9 Quantum Computing Methods

shape and the minimum value occurs again near  D . Our focus here is
on VQE, but further background on noisy quantum computations can allow
one to rigorously prove theorems about the noise resilience of
variational quantum algorithms. Topics related to noise such as Kraus
operators (a standard representation of noisy quantum channels) and
purification (writing a mixed state  as the partial trace of a pure
state j i over the environment,  D TrE j ih j) can be found in
additional resources such as \[102, 206, 238\]. For another approach to
VQE, see \[110\].

More Sophisticated Ansatzes As mentioned, larger Hamiltonians may
require an ansatz with more parameters to more closely approximate the
ground state wavefunction. In pyQuil, we can increase the number of
parameters in our program by adding more gates as follows: \# Function
for an anstaz with two parameters def smallish\_ansatz(params):
"""Returns an ansatz with two parameters.""" return
Program(RX(params\[0\], 0), RZ(params\[1\], 0)) print("Ansatz with two
gates and two parameters (with example values):")
print(smallish\_ansatz(\[1.0, 2.0\])) \# Get a VQE instance vqe\_inst =
VQE(minimizer=minimize, minimizer\_kwargs={’method’: ’nelder-mead’}) \#
Do the minimization and return the best angle initial\_angles = \[1.0,
1.0\] result = vqe\_inst.vqe\_run(smallish\_ansatz, hamiltonian,
initial\_angles, None, qvm=qvm) print("\nMinimum energy =",
round(result\["fun"\], 4)) print("Best angle =",
round(result\["x"\]\[0\], 4))

In the program above, we create an ansatz with two gates and two
parameters, print it out, then run the VQE algorithm with this ansatz.
An example outcome of the program is "Ansatz with two gates and two
parameters (with example values):" RX(1.0) 0 RZ(2.0) 0 Minimum energy =
-1.0 Best angle = 3.1416

SECTION 9.2 Quantum Chemistry

151

Here, we see that the minimizer is able to find the exact ground state
energy with the new ansatz. This is expected — since we know we can
minimize the expectation of the Hamiltonian with only one Rx gate, the
second Rz gate is superfluous. For larger, non-trivial Hamiltonians,
however, this may not be the case, and more parameters may be needed. In
this section, we use simple trial ansatzes for clarity of presentation.
In general, choosing both an appropriate ansatz and good initial
starting point for the parameters of the ansatz are critical for
successful VQE implementations. Randomly generated ansatzes are likely
to have gradients that vanish for large circuit sizes \[189\], thus
making the optimization over parameters exceedingly difficult, if not
practically impossible. For these reasons, structured ansatzes such as
unitary coupled cluster or QAOA (see Section 9.3) — as opposed to
parameterized random quantum circuits — are used in practice.

9.2

Quantum Chemistry

We will now explore an application of quantum chemistry, or more
generally quantum simulation.2 Early work on quantum simulation was done
by Lloyd \[174\], and more recent developments include \[37, 177, 21,
265\]. In quantum simulation we seek to model the dynamic evolution of
the wavefunction under some Hamiltonian H as per Schrödinger’s equation
i

@j i DHj i @t

(9.3)

where we have set \~ D 1. It is easy to write the time evolution
operator U.t / D exp . iH t /

(9.4)

which evolves the initial state j .0/i to a final state at time t via j
.t /i D U.t /j .0/i

(9.5)

However, it is generally very difficult to classically compute the
unitary time evolution operator U.t/ by exponentiating the Hamiltonian
of the system, even if the Hamiltonian is sparse. The problem is so
important that many techniques for approximating the time evolution have
emerged, such as the Suzuki-Trotter formula \[206\], also referred to as
Trotterization. Techniques also emerged 2 Note:

this use of the term "quantum simulation" is distinct from the use of a
program to simulate the actions of a quantum computer as discussed in
chapter 6.

152

CHAPTER 9 Quantum Computing Methods

to represent the Hamiltonian in a quantum computer such as qubitization
(see \[178\]). Quantum simulation on a QC give us the opportunity to
more easily compute unitary time evolution. Quantum simulation is useful
in the same respect that classical simulation of time-dependent
processes is useful. Namely, it allows us to analyze the behavior of a
complex physical system, compute observable properties, and use both of
these to make new predictions or compare them with experimental results.
As an example, O’Malley et al. demonstrated the use of VQE and quantum
simulation with QPE to calculate the potential energy surface of
molecular hydrogen \[211\]. Quantum simulation of molecular Hamiltonians
is useful for quantum chemistry applications. In the following program,
we use Cirq in conjuction with OpenFermion — an open-source package for
quantum chemistry that has integration with Cirq \[192\]3 — to show how
we can simulate the evolution of an initial state under a Hamiltonian.
In the sample code used here for pedagogic purposes we randomly generate
the Hamiltonian and its initial state; we recommend against this in real
world conditions for reasons outlined in McClean et al. \[189\]. See
also \[146\] for a broader discussion of running quantum chemistry
models on NISQ computers and \[127\] for a discussion of Hartree-Fock on
a NISQ superconducting quantum computer. We now walk through the program
in steps. First, we import the necessary packages and define a few
constants for our simulation. Namely, we define the number of qubits n,
the final simulation time t, and a seed for the random number generator
which allows for reproducible results. \# Imports import numpy import
scipy import cirq import openfermion import openfermioncirq \# Set the
number of qubits, simulation time, and seed for reproducibility
n\_qubits = 3 simulation\_time = 1.0 random\_seed = 8317

In the code block below, we generate a random Hamiltonian in matrix
form. In order to run any quantum circuits with this Hamiltonian, it
first must be written in terms of quantum operators. The next few lines
of code use the functionality in OpenFermion to do this. 3 Note

Cirq.

that the package OpenFermion-Cirq is used as a bridge between
OpenFermion and

SECTION 9.2 Quantum Chemistry

153

Generate the random one-body operator
=====================================

T = openfermion.random\_hermitian\_matrix(n\_qubits, seed=random\_seed)
print("Hamiltonian:", T, sep="\n") \# Compute the OpenFermion
"FermionOperator" form of the Hamiltonian H =
openfermion.FermionOperator() for p in range(n\_qubits): for q in
range(n\_qubits): term = ((p, 1), (q, 0)) H +=
openfermion.FermionOperator(term, T\[p, q\])
print("\nFermion operator:") print(H)

The output of this portion of the program is Hamiltonian: \[\[
0.53672126+0.j -0.26033703+3.32591737j
1.34336037+1.54498725j\]\[-0.26033703-3.32591737j -2.91433037+0.j
-1.52843836+1.35274868j\] \[ 1.34336037-1.54498725j
-1.52843836-1.35274868j 2.26163363+0.j \]\] Fermion operator:
(0.5367212624097257+0j) \[0\^ 0\] +
(-0.26033703159240107+3.3259173741375454j) \[0\^
(1.3433603748462144+1.544987250567917j) \[0\^ 2\]
(-0.26033703159240107-3.3259173741375454j) \[1\^
(-2.9143303700812435+0j) \[1\^ 1\] +
(-1.52843836446248+1.3527486791390022j) \[1\^ 2\]
(1.3433603748462144-1.544987250567917j) \[2\^ 0\]
(-1.52843836446248-1.3527486791390022j) \[2\^ 1\] (2.261633626116526+0j)
\[2\^ 2\]

1\] + + 0\] + + + +

The first section displays the Hamiltonian in matrix form, then the next
section displays the matrix in OpenFermion operator form. Here, the
OpenFermion notation \[p\^ q\] is used to indicate the product of
fermionic creation and  annihilation operators ap aq on sites p and q,
respectively, which satisfy the canonical commutation relations fap ;
aq g D ıpq

(9.6)

fap ; aq g D 0

(9.7)

Now that we have our Hamiltonian in a usable form, we can begin
constructing our circuit. As is common in quantum simulation algorithms
\[206\], we first rotate to the eigenbasis of the Hamiltonian. This is
done by (classically) diagonalizing the Hamiltonian, then using
OpenFermion to construct a circuit that performs this basis
transformation. \# Diagonalize T and obtain basis transformation matrix
(aka "u") eigenvalues, eigenvectors = numpy.linalg.eigh(T)

154

CHAPTER 9 Quantum Computing Methods

basis\_transformation\_matrix = eigenvectors.transpose() \# Initialize
the qubit register qubits = cirq.LineQubit.range(n\_qubits) \# Rotate to
the eigenbasis inverse\_basis\_rotation = cirq.inverse(
openfermioncirq.bogoliubov\_transform(qubits,
basis\_transformation\_matrix) ) circuit =
cirq.Circuit.from\_ops(inverse\_basis\_rotation)

Now we can add the gates corresponding to evolution of the Hamiltonian.
Since we are in the eigenbasis of the Hamiltonian, this corresponds to a
diagonal operator of Pauli-Z rotations, where the rotation angle is
proportional to the eigenvalue and final simulation time. Finally, we
change bases back to the computational basis. \# Add diagonal phase
rotations to circuit for k, eigenvalue in enumerate(eigenvalues): phase
= -eigenvalue \* simulation\_time
circuit.append(cirq.Rz(rads=phase).on(qubits\[k\])) \# Finally, change
back to the computational basis basis\_rotation =
openfermioncirq.bogoliubov\_transform( qubits,
basis\_transformation\_matrix ) circuit.append(basis\_rotation)

The time evolution operator is now constructed in our quantum circuit.
Below, we first obtain a random initial state. Note that this is program
is for demonstration purposes. In real world scenarios we will want to
use a number of non-random techniques to determine the initial state: \#
Initialize a random initial state initial\_state =
openfermion.haar\_random\_vector( 2 \*\* n\_qubits,
random\_seed).astype(numpy.complex64)

Now we compute the time evolution numerically using matrix
exponentiation and then simulate it with a QC simulator. After obtaining
the final state using both methods, we compute the fidelity (overlap
squared) of the two and print out the value. \# Numerically compute the
correct circuit output hamiltonian\_sparse =
openfermion.get\_sparse\_operator(H) exact\_state =
scipy.sparse.linalg.expm\_multiply( -1j \* simulation\_time \*
hamiltonian\_sparse, initial\_state )

SECTION 9.2 Quantum Chemistry

155

Use Cirq simulator to apply circuit
===================================

simulator = cirq.google.XmonSimulator() result =
simulator.simulate(circuit, qubit\_order=qubits,
initial\_state=initial\_state) simulated\_state = result.final\_state \#
Print final fidelity fidelity = abs(numpy.dot(simulated\_state,
numpy.conjugate(exact\_state)))\*\*2 print("\nfidelity =",
round(fidelity, 4))

The output of this section of the code fidelity = 1.0

indicates that our quantum circuit evolved the initial state exactly the
same as the analytic evolution! Of course, for larger systems the
analytic evolution cannot be computed, and we have to rely solely on a
quantum computer. This small proof of principle calculation indicates
the validity of this method. Lastly, we mention that Cirq has the
functionality to compile this quantum circuit for Google’s Xmon
architecture quantum computers, as well as IBM’s quantum computers. The
code snippet below shows how this is done: \# Compile the circuit to
Google’s Xmon architecture xmon\_circuit =
cirq.google.optimized\_for\_xmon(circuit) print("\nCircuit optimized for
Xmon:") print(xmon\_circuit) \# Print out the OpenQASM code for IBM’s
hardware print("\nOpenQASM code:") print(xmon\_circuit.to\_qasm())

Below, we include the OpenQASM code generated by Cirq for this circuit.
The complete circuit diagram and remaining output of this code can be
seen by executing this program, which can be found on the book’s GitHub
site. // Generated from Cirq v0.4.0 OPENQASM 2.0; include "qelib1.inc";

// Qubits: \[0, 1, 2\] qreg q\[3\];

u2(pi*-1.0118505646, pi*1.0118505646) q\[2\]; u2(pi*-1.25, pi*1.25)
q\[1\]; u2(pi*-1.25, pi*1.25) q\[0\];

156

CHAPTER 9 Quantum Computing Methods

cz q\[1\],q\[2\]; u3(pi*-0.1242949803, pi*-0.0118505646,
pi*0.0118505646) q\[2\]; u3(pi*0.1242949803, pi*-0.25, pi*0.25) q\[1\];
cz q\[1\],q\[2\]; u3(pi*-0.3358296941, pi*0.4881494354,
pi*-0.4881494354) q\[2\]; u3(pi*-0.5219350773, pi*1.25, pi*-1.25)
q\[1\]; cz q\[0\],q\[1\]; u3(pi*-0.328242091, pi*0.75, pi*-0.75) q\[1\];
u3(pi*-0.328242091, pi*-0.25, pi*0.25) q\[0\]; cz q\[0\],q\[1\];
u3(pi*-0.2976584908, pi*0.25, pi*-0.25) q\[1\]; u3(pi*-0.7937864503,
pi*0.25, pi*-0.25) q\[0\]; cz q\[1\],q\[2\]; u3(pi*-0.2326621647,
pi*-0.0118505646, pi*0.0118505646) q\[2\]; u3(pi*0.2326621647, pi*-0.25,
pi*0.25) q\[1\]; cz q\[1\],q\[2\]; u3(pi*0.8822298425, pi*0.4881494354,
pi*-0.4881494354) q\[2\]; u3(pi*-0.2826706001, pi*0.25, pi*-0.25)
q\[1\]; cz q\[0\],q\[1\]; u3(pi*-0.328242091, pi*0.75, pi*-0.75) q\[1\];
u3(pi*-0.328242091, pi*-0.25, pi*0.25) q\[0\]; cz q\[0\],q\[1\];
u3(pi*-0.3570821075, pi*0.25, pi*-0.25) q\[1\]; u2(pi*-0.25, pi*0.25)
q\[0\]; rz(pi*0.676494835) q\[0\]; cz q\[1\],q\[2\]; u3(pi*0.1242949803,
pi*0.9881494354, pi*-0.9881494354) q\[2\]; u3(pi*-0.1242949803, pi*0.75,
pi*-0.75) q\[1\]; cz q\[1\],q\[2\]; u2(pi*-0.0118505646,
pi*0.0118505646) q\[2\]; u2(pi*-0.25, pi*0.25) q\[1\];
rz(pi*-0.4883581348) q\[1\]; rz(pi*0.5116418652) q\[2\];

9.3

Quantum Approximate Optimization Algorithm (QAOA)

While the previous two quantum computing methods were geared towards
physics and chemistry applications, the quantum approximate optimization
algorithm (QAOA) is geared towards general optimization problems. Farhi
et al. introduced QAOA to handle these kinds of problems \[104, 105\].
See also \[106\] for work on adiabatic algorithms which preceded QAOA.
Here, the goal is to maximize or minimize a cost function C.b/ D

m X ˛D1

C˛ .b/

(9.8)

SECTION 9.3 Quantum Approximate Optimization Algorithm (QAOA)

157

written as a sum of m clauses C˛ .b/ on bitstrings b 2 f0; 1gn , or
equivalently spins zi 2 f 1; C1gn as there is a bijective map between
the bitstrings and spins.4 MaxCut is an example of a problem for which
we can use QAOA on a regular graph \[104\]; the cost function can be
written in terms of spins as C.z/ D

1X .1 2

zi zj /

(9.9)

hi;j i

Here, the sum is over edges hi; j i in a graph, and each clause .1 zi zj
/ contributes a non-zero term to the cost iff the spins zi and zj are
anti-aligned (i.e., have different values). A more general case of this
problem considers arbitrary weights wij between each edge \[309\]. This
amounts to saying that clauses with larger weights wij contribute a
higher cost. We’ll consider this case in the text that follows. By
promoting each spin to a Pauli-Z operator (which has eigenvalues ˙1),
the cost can be written as a cost Hamiltonian C  HC D

1X wij .I 2

z.i / z.j / /

(9.10)

hi;j i

.i /

where I is the identity operator and z denotes a Pauli-Z operator on
the i th spin. This cost Hamiltonian can easily be seen to be diagonal
in the computational basis. This is the general input to the quantum
approximate optimization algorithm, as we discuss below. The
prescription for QAOA is as follows. Given a cost Hamiltonian HC  H of
the form (9.8), define the unitary operator U.HC ; / WD e

i HC

D

m Y

e

i C˛

(9.11)

˛D1

which depends on the parameter . Note that the second line follows
because each clause C˛ is diagonal in the computational basis, hence ŒC˛
; Cˇ  D 0 for all ˛; ˇ 2 f1; :::; mg. Further note that this can be
interpreted, in light of the previous section, as simulating (i.e.,
evolving with) the cost Hamiltonian HC for a time . We can restrict the
“time” to be between 0 and 2, however, since C has integer values.
Thus, we can equally think of the parameter as an angle of rotation. 4
Bits

b and spins z are related by the bijective mapping z D 1 2b () b D .1
Thus, any problem on bits can be framed as a problem on spins and vice
versa.

z/=2

158

CHAPTER 9 Quantum Computing Methods

Next, define the operator B  HB , known as a mixer Hamiltonian, which
is conventionally taken to be B  HB D

n X

x.j /

(9.12)

j D1 .j /

where x operator

is a Pauli-X operator on spin j . From this, we form the unitary U.HB ;
ˇ/ WD e

iˇB

D

n Y

e

.j /

iˇ x

(9.13)

j D1

Note that the second equality follows because all terms in the
Hamiltonian .j / commute with one another. We can view the term e iˇ x
as a rotation about the x axis on spin j by angle 2ˇ. Thus, we can
restrict 0  ˇ &lt; . With these definitions, we can state the steps of
the quantum part of the QAOA: 1. Start with an initial state that is an
equal superposition over all bitstrings (spins) X 1 jsi D p jbi (9.14)
2n b2f0;1gn by applying a Hadamard to each qubit H ˝n j0i˝n . 2. Evolve
with the cost Hamiltonian by implementing U.HC ; / for an angle . 3.
Evolve with the mixer Hamiltonian by implementing U.HB ; ˇ/ for an angle
ˇ. 4. Repeat steps (2) and (3) p times with different parameters i ; ˇi
at each step i D 1; :::; p to form the state j ; ˇi WD

p Y

U.HB ; ˇi /U.HC ;

i /jsi

(9.15)

i D1

5.  Measure in the computational basis to compute the expectation of HC
    in this state: Fp . ; ˇ/ WD h ; ˇjHC j ; ˇi (9.16)
6.  Use a (classical) optimization algorithm to (approximately) compute
    the maximum or minimum value of Fp . ; ˇ/. Alternatively, if you
    have other methods to determine the optimal angles, you may use
    these.

SECTION 9.3 Quantum Approximate Optimization Algorithm (QAOA)

159

7.  Sample from the output distribution of the circuit (9.15) to get a
    set of bitstrings b. The most probable bitstrings encode the
    approximate optima for the cost function. The full circuit diagram
    for the quantum circuit in the QAOA is shown below. j0i

H

j0i

H ei

1 HC

e iˇ1 X



e iˇ1 X



j0i

H

e iˇ1 X



j0i

H

e iˇ1 X



e iˇp X ei

p HC

e iˇp X e iˇp X e iˇp X

The adiabatic theorem states that a system remains in its eigenstate
even when subject to a perturbation, as long as that perturbation is
slow and gradual enough and there is a gap between the eigenvalue of
that state and the rest of the eigenvalues of the system (its spectrum)
\[48, 49, 148\]. In other words if we have a system in a measured state
and that state has enough of gap from other possible states of the
system, then if we perturb the system slowly enough, it will not jump to
another eigenstate. It can be shown using the adiabatic theorem that lim
max Fp . ; ˇ/ D max C.b/:

p!1

;ˇ

b

(9.17)

That is, given enough parameters ; ˇ, we can be sure that the exact
solution of the problem is attainable. The parameter p can thus be
considered a hyperparameter. One form of approximation in the quantum
approximate optimization algorithm is the finite cutoff for p. Another
form of approximation is the ability of the classical optimizer to find
the optimum. However, in particular cases there are provable performance
guarantees for p D 1 layers. For example, for p D 1 on 3-regular graphs,
the QAOA always finds a cut that is at least 0.6924 times the size of
the optimal cut \[104\]. Proving more worst-case or average-case
performance guarantees is an interesting line of research on the
analytic side of QAOA, and developing better classical optimization
algorithms is an interesting area on the heuristic side of QAOA.

Example Implementation of QAOA To get a better idea of how QAOA works,
we now turn to an implementation. In this example, we consider the
transverse field Ising model as a cost Hamiltonian:

160

CHAPTER 9 Quantum Computing Methods

HC D

X

Jij z.i / z.j /

X

hi x.i /

(9.18)

i

hi;j i

For simplicity of presentation, we set the transverse field coefficients
to zero (hi D 0) and set each interaction coefficient to one (Jij D 1).
The Hamiltonian can be modified in a straightforward way to generalize
it, but these details are not important in a first encounter with QAOA.
Another reason for this is that this system is trivial to solve
analytically — thus, we can compare the solution found by QAOA to the
exact solution. By making these simplifications, our cost Hamiltonian
has the form X HC D z.i / z.j / (9.19) hi;j i

The graph (i.e., the arrangement of spins) we will consider is in a
nearest neighbors configuration on a 2D grid. We thus need a way to
implement the unitary operator Y U.HC ; / WD e iHC D e i Zi Zj (9.20)
hi;j i .i /

For simplicity, from here on we will substitute Zi for z . In order to
implement this entire unitary, we need a sequence of gates for
implementing each e i Zi Zj term, where i and j are neighbors in the
graph. It will be convenient to rescale and consider implementing the
unitary e i  Zi Zj . To understand how to do this, note that the
operator Z ˝ Z is diagonal in the computational basis, hence e i Z˝Z is
just the exponential of each diagonal element (multiplied by i ) 2 i 3
e 0 0 0 6 0 e i 0 0 7 7 exp.i Z ˝ Z/ D 6 (9.21) i  4 0 0 e 0 5 0 0 0
ei  To get some intuition about how to implement this operator in terms
of standard gates, note that the controlled-Z gate is diagonal with C.Z/
D diag.1; 1; 1; 1/. Writing 1 D e i  , we see that C.Z/ D diag.1; 1; 1;
e i  /, hence 2 3 1 0 0 0 60 1 0 0 7 7 C.Z / D 6 (9.22) 40 0 1 0 5 0 0
0 ei 

SECTION 9.3 Quantum Approximate Optimization Algorithm (QAOA)

161

This gives us one diagonal term in the final unitary (9.21) that we want
to implement. To get the other terms, we can apply X operators on the
appropriate qubits. For example, 2 3 2 3 1 0 0 0 1 0 0 0 60 1 0 6 0 7 0
07 7 .I ˝ X / D 60 1 7 .I ˝ X/ 6 (9.23) i  40 0 1 5 4 0 0 0 e 05 0 0 0
ei  0 0 0 1 We can continue in this fashion to get all four diagonal
elements, then get the full unitary (9.21) by simply multiplying them
together (using the fact that the product of diagonal matrices is
diagonal). In the Cirq code below, we write a function which gives us a
circuit for implementing the unitary e i  Zi Zj . We then test our
function by printing out the circuit for an example set of qubits i and
j with an arbitrary value of and ensuring that the unitary matrix of
this circuit is what we expect. \# Imports import numpy as np import
matplotlib.pyplot as plt import cirq \# Function to implement a ZZ gate
on qubits a, b with angle gamma def ZZ(a, b, gamma): """Returns a
circuit implementing exp(-i \pi \gamma Z\_i Z\_j).""" \# Get a circuit
circuit = cirq.Circuit() \# Gives the fourth diagonal component
circuit.append(cirq.CZ(a, b)\*\*gamma) \# Gives the third diagonal
component circuit.append(\[cirq.X(b), cirq.CZ(a,b)\*\*(-1 \* gamma),
cirq.X(b)\]) \# Gives the second diagonal component
circuit.append(\[cirq.X(a), cirq.CZ(a,b)\*\*-gamma, cirq.X(a)\]) \#
Gives the first diagonal component circuit.append(\[cirq.X(a),
cirq.X(b), cirq.CZ(a,b)\*\*gamma, cirq.X(a), cirq.X(b)\]) return circuit
\#26.s.one \# Make sure the circuit gives the correct matrix qreg =
cirq.LineQubit.range(2) zzcirc = ZZ(qreg\[0\], qreg\[1\], 0.5)
print("Circuit for ZZ gate:", zzcirc, sep="\n") print("\nUnitary of
circuit:", zzcirc.to\_unitary\_matrix().round(2), sep="\n")

162

CHAPTER 9 Quantum Computing Methods

The output of this code is as follows: Circuit for ZZ gate: 0:
---@-----------@------------X---@--------X---X---@-------X--| | | | 1:
---@^0.5---X---@^-0.5---X-------@^-0.5-------X---@^0.5---X--Unitary of
circuit: \[\[0.+1.j 0.+0.j 0.+0.j \[0.+0.j 0.-1.j 0.+0.j \[0.+0.j 0.+0.j
0.-1.j \[0.+0.j 0.+0.j 0.+0.j

0.+0.j\] 0.+0.j\] 0.+0.j\] 0.+1.j\]\]

As we can see by comparing with (9.21), this circuit indeed implements
the desired unitary operator. Note that the circuit is not optimal — a
trivial simplification is removing sequential X operators on qubit 0,
and other optimizations are possible. Such optimizations will not
concern us here, however. In the next block of code, we define a 2x2
grid of qubits. ncols = 2 nrows = 2 qreg = \[\[cirq.GridQubit(i,j) for j
in range(ncols)\] for i in range(nrows)\]

Then we write functions for implementing the operators U.HC ; / and U.HB
; ˇ/. \# Function to implement the cost Hamiltonian def
cost\_circuit(gamma): """Returns a circuit for the cost Hamiltonian."""
circ = cirq.Circuit() for i in range(nrows): for j in range(ncols): if i
&lt; nrows - 1: circ += ZZ(qreg\[i\]\[j\], qreg\[i + 1\]\[j\], gamma) if
j &lt; ncols - 1: circ += ZZ(qreg\[i\]\[j\], qreg\[i\]\[j + 1\], gamma)
return circ \# Function to implement the mixer Hamiltonian def
mixer(beta): """Generator for U(H\_B, beta) layer (mixing layer)""" for
row in qreg: for qubit in row: yield cirq.X(qubit)\*\*beta

These functions allow us to construct the entire QAOA circuit. The
function below builds this circuit for an arbitrary number p of
parameters. \# Function to build the QAOA circuit def qaoa(gammas,
betas):

SECTION 9.3 Quantum Approximate Optimization Algorithm (QAOA)

163

"""Returns a QAOA circuit.""" circ = cirq.Circuit()
circ.append(cirq.H.on\_each(\*\[q for row in qreg for q in row\])) for i
in range(len(gammas)): circ += cost\_circuit(gammas\[i\])
circ.append(mixer(betas\[i\])) return circ

Now that we can build our QAOA circuit for a given set of parameters, we
can compute the expectation of the cost Hamiltonian in the final state
(9.16). For simplicity we use Cirq’s ability to access the wavefunction
to compute this expectation rather than sampling from the circuit
itself. The following function shows how we can access the wavefunction
after applying a circuit: def simulate(circ): """Returns the
wavefunction after applying the circuit.""" sim = cirq.Simulator()
return sim.simulate(circ).final\_state

The next function evaluates the expectation using the wavefunction: def
energy\_from\_wavefunction(wf): """Computes the energy-per-site of the
Ising Model from the wavefunction.""" \# Z is a (n\_sites x 2**n\_sites)
array. Each row consists of the \# 2**n\_sites non-zero entries in the
operator that is the Pauli-Z matrix on \# one of the qubits times the
identites on the other qubits. The (i*n\_cols + j)th \# row corresponds
to qubit (i,j). Z = np.array(\[(-1)**(np.arange(2**nsites) &gt;&gt; i)
for i in range(nsites-1,-1,-1)\]) \# Create the operator corresponding
to the interaction energy summed over all \# nearest-neighbor pairs of
qubits ZZ\_filter = np.zeros\_like(wf, dtype=float) for i in
range(nrows): for j in range(ncols): if i &lt; nrows-1: ZZ\_filter +=
Z\[i\*ncols + j\]*Z\[(i+1)\*ncols + j\] if j &lt; ncols-1: ZZ\_filter +=
Z\[i\*ncols + j\]\*Z\[i\*ncols + (j+1)\] \# Expectation value of the
energy divided by the number of sites return -np.sum(np.abs(wf)\*\*2 \*
ZZ\_filter) / nsites

Finally, for convenience, we define a function that computes the
energy/cost directly from a set of parameters. This function uses the
parameters to

164

CHAPTER 9 Quantum Computing Methods

build a circuit, then gets the wavefunction of the final state and
lastly computes the energy/cost using the previous function. def
cost(gammas, betas): """Returns the cost function of the problem."""
wavefunction = simulate(qaoa(gammas, betas)) return
energy\_from\_wavefunction(wavefunction)

These functions provide the set up for QAOA, and we could now optimize
the parameters to minimize the cost. For instructional purposes, we
implement QAOA with p D 1 layers and perform a grid search, plotting the
2D cost landscape for each parameter and ˇ. The function for the grid
search over a range of parameters is given below: def
grid\_search(gammavals, betavals): """Does a grid search over all
parameter values.""" costmat = np.zeros((len(gammavals), len(betavals)))
for (i, gamma) in enumerate(gammavals): for (j, beta) in
enumerate(betavals): costmat\[i, j\] = cost(\[gamma\], \[beta\]) return
costmat

Finally, here is the code for using this function within the main script
and plotting the cost landscape: \# Get a range of parameters gammavals
= np.linspace(0, 1.0, 50) betavals = np.linspace(0, np.pi, 75) \#
Compute the cost at all parameter values using a grid search costmat =
grid\_search(gammavals, betavals) \# Plot the cost landscape
plt.imshow(costmat, extent=(0, 1, 0, np.pi), origin="lower",
aspect="auto") plt.colorbar() plt.show()

The output of this section of the program is shown in Figure 9.3. As we
can see, there is a significant amount of symmetry in the cost
landscape. This phenomena is typical in variational quantum algorithms.
Apart from the symmetry which arises naturally from the Ising
Hamiltonian, the symmetric and periodic form of the cost landscape
arises from symmetries in the ansatz circuit. Exploiting these
symmetries can help lead classical optimization algorithms to a good
solution more quickly.

SECTION 9.3 Quantum Approximate Optimization Algorithm (QAOA)

165

3.0 0.4 2.5 0.2

2.0

0.0

1.5 1.0

0.2

0.5 0.0 0.0

0.4 0.2

0.4

0.6

0.8

1.0

Figure 9.3: Cost landscape of the Ising Hamiltonian computed from one
layer of QAOA

We can now obtain a set of optimal parameters by taking the coordinates
of a minimum in our cost landscape. The following short block of code
does this and prints out the numerical value of the cost at these
parameters. \# Coordinates from the grid of cost values gamma\_coord,
beta\_coord = np.where(costmat == np.min(costmat)) \# Values from the
coordinates gamma\_opt = gammavals\[gamma\_coord\[0\]\] beta\_opt =
betavals\[beta\_coord\[0\]\]

Now that we have the optimal parameters, we can run the QAOA circuit
with these parameters and measure in the computational basis to get
bitstrings that solve our original optimization problem. The function
below runs the circuit and returns the measurement results. def
get\_bit\_strings(gammas, betas, nreps=10000): """Measures the QAOA
circuit in the computational basis to get bitstrings.""" circ =
qaoa(gammas, betas) circ.append(cirq.measure(\*\[qubit for row in qreg
for qubit in row\], key=’m’)) \# Simulate the circuit sim =
cirq.Simulator() res = sim.run(circ, repetitions=nreps) return res

166

CHAPTER 9 Quantum Computing Methods

Finally, we use this function to sample from the circuit at the optimal
parameters found above. Then, we parse the output and print out the two
most common bitstrings sampled from the circuit. \# Sample to get bits
and convert to a histogram bits = get\_bit\_strings(\[gamma\_opt\],
\[beta\_opt\]) hist = bits.histogram(key="m") \# Get the most common
bits top = hist.most\_common(2) \# Print out the two most common
bitstrings measured print("\nMost common bitstring:")
print(format(top\[0\]\[0\], "\#010b")) print("\nSecond most common
bitstring:") print(bin(top\[1\]\[0\]))

A sample output of this portion of the code follows: Most common
bitstring: 0b000000000 Second most common bitstring: 0b111111111

These bitstrings are exactly the ones we would expect to minimize our
cost function! Recall the Ising Hamiltonian we considered, which when
written classically has the form X C.z/ D zi zj (9.24) hi;j i

where zi D ˙1 are spins. For our bitstring output, b D 0 corresponds to
spin up (z D 1) and b D 1 corresponds to spin down (z D 1). Since
opposite spins zi ¤ zj will produce a term with a positive contribution
(don’t forget the overall minus sign in front!) in the sum, the minimum
value of the cost function occurs when all spins are aligned. That is,
zi D zj for all i; j . The bitstrings that we measured correspond to all
spins aligned down or all spins aligned up, respectively. Thus, these
bitstrings indeed produced the minimum value for our cost function, and
QAOA was able to successfully optimize the cost. For larger optimization
problems with more complex cost functions, more layers in the QAOA
ansatz (i.e., p &gt; 1) may become necessary. More layers means more
parameters in the variational quantum circuit, which leads to a harder
optimization problem. Such an optimization problem could not be solved
by a mere grid search over values, as this quickly becomes intractable.

SECTION 9.4 Machine Learning on Quantum Processors

167

Figure 9.4: Data types and processor types

Rather, gradient-based or gradient-free optimization algorithms must be
used to compute an approximately optimal set of parameters. The complete
program for this implementation of QAOA is available on the book’s
online site.

9.4

Machine Learning on Quantum Processors

Several groups are exploring the use of QC for machine learning; it is
natural to ask whether QC affords us any advantage in this area. Speedup
is not the only advantage we should consider in quantum machine learning
(QML). There may be opportunities to use a QC to process data directly
from a quantum sensor that retains the full range of quantum information
from that sensor. Figure 9.4 points to the potential of matching quantum
data with quantum processing. Having a classifier on the QC directly
analyzing the datastream for patterns may be better than piping the data
to a classical computer. A number of groups have published in this area,
including: 1. Alan Aspuru-Guzik and colleagues have explored quantum
machine learning as well as hybrid classical-quantum models \[64, 241\].

168

CHAPTER 9 Quantum Computing Methods

2.  The Rigetti team has worked on unsupervised machine learning on a
    classical-quantum hybrid approach \[212\].
3.  Farhi and Neven laid out an approach to classification with neural
    networks on a quantum processor (QNNs) \[109\].
4.  Wittek and Gogolin explored Markov logic networks on quantum
    platforms \[299\].
5.  See \[251\] for a discussion of supervised learning on quantum
    computers.
6.  See \[39, 281, 282\] for additional work in QML and \[298\] for an
    online course in QML.
7.  See \[251\] for a discussion of supervised learning on quantum
    computers.
8.  See \[7\] for a review of quantum neural networks. A standard
    benchmark problem in machine learning is MNIST classification. Here,
    we show how this can be done with a quantum machine learning model.
    To do so, we follow an example in TensorFlow-Quantum (TFQ), a
    library which allows machine learning practitioners to add quantum
    circuits as layers in neural networks created with TensorFlow. Using
    TFQ to illustrate, we show how to:  Encode the data in a quantum
    state  Process the data through a quantum circuit (quantum neural
    network)  calculate a loss function  minimize the loss function to
    accurately classify images Our first task is to encode the
    (classical) MNIST image data in a quantum state. For completeness,
    we show the packages we will use below. \# Imports import tensorflow
    as tf import tensorflow\_quantum as tfq import import import import
    import

cirq sympy numpy as np seaborn as sns collections

import matplotlib.pyplot as plt

TensorFlow has common datasets built-in; below, we load up the MNIST
dataset, which consists of images of handwritten digits (0-9).
(x\_train, y\_train), (x\_test, y\_test) =
tf.keras.datasets.mnist.load\_data()

SECTION 9.4 Machine Learning on Quantum Processors

169

Figure 9.5: Example full-resolution (left) and downscaled (right) MNIST
dataset image.

Each image is a 28  28 matrix (two-dimensional array) of floating point
values in the range Œ0; 255. Our first step of the encoding is to map
this range to Œ0; 1 so the values are more easily stored in a quantum
computer. x\_train, x\_test = x\_train\[..., np.newaxis\] / 255.0,
x\_test\[..., np.newaxis\] / 255.0

For simplicity, let’s consider the classification task of distinguishing
between 3’s and 6’s. def filter\_36(x, y): keep = (y == 3) | (y == 6) x,
y = x\[keep\], y\[keep\] y = y == 3 return x,y

x\_train, y\_train = filter\_36(x\_train, y\_train) x\_test, y\_test =
filter\_36(x\_test, y\_test)

Our dataset now only contains images of 3’s and 6’s. The last
“preprocessing” step is to downscale the images, as 28  28 is too large
for NISQ computers. A size of 4  4 is more reasonable. x\_train\_small
= tf.image.resize(x\_train, (4,4)).numpy() x\_test\_small =
tf.image.resize(x\_test, (4,4)).numpy()

An example of a full-resolution and downscaled image is shown in Figure
9.5. Now that the “pre-processing” is done, we get to the fun part:
encoding the image data into a quantum circuit. There are many
strategies to do so, and several aspects of the learning procedure can
vary depending on the encoding. Here, we use the following strategy:
each pixel (floating point value in the range Œ0; 1) of the image will
correspond to one qubit. If the pixel is below

170

CHAPTER 9 Quantum Computing Methods

0:5, we represent it as the j0i state; otherwise, we represent it as the
j1i state. (Intuitively, this can be thought of as making the image
black and white.) THRESHOLD = 0.5 x\_train\_bin =
np.array(x\_train\_small &gt; THRESHOLD, dtype=np.float32) x\_test\_bin
= np.array(x\_test\_small &gt; THRESHOLD, dtype=np.float32)

def convert\_to\_circuit(image): """Encode truncated classical image
into quantum datapoint.""" values = np.ndarray.flatten(image) qubits =
cirq.GridQubit.rect(4, 4) circuit = cirq.Circuit() for i, value in
enumerate(values): if value: circuit.append(cirq.X(qubits\[i\])) return
circuit

x\_train\_circ = \[convert\_to\_circuit(x) for x in x\_train\_bin\]
x\_test\_circ = \[convert\_to\_circuit(x) for x in x\_test\_bin\]

At this point, for each image in the dataset, we have a corresponding
quantum circuit. In TFQ, all circuits must be converted to tensors.
x\_train\_tfcirc = tfq.convert\_to\_tensor(x\_train\_circ)
x\_test\_tfcirc = tfq.convert\_to\_tensor(x\_test\_circ)

Now that the encoding is done, we have to design a quantum neural
network (QNN) to propagate the encoded data through a series of
trainable (parameterized) quantum gates. Just like the encoding step,
there are many ways to design the QNN. Here, we follow the construction
of Farhi \[109\] and implement the following layered circuit ansatz.
class CircuitLayerBuilder(): def **init**(self, data\_qubits, readout):
self.data\_qubits = data\_qubits self.readout = readout def
add\_layer(self, circuit, gate, prefix): for i, qubit in
enumerate(self.data\_qubits): symbol = sympy.Symbol(prefix + ’-’ +
str(i)) circuit.append(gate(qubit, self.readout)\*\*symbol)

demo\_builder = CircuitLayerBuilder(data\_qubits =
cirq.GridQubit.rect(4,1), readout=cirq.GridQubit(-1,-1)) circuit =
cirq.Circuit() demo\_builder.add\_layer(circuit, gate = cirq.XX,
prefix=’xx’)

SECTION 9.4 Machine Learning on Quantum Processors

171

Figure 9.6: A single layer circuit ansatz used for the quantum neural
network classifying MNIST images, as in \[109\]. The top qubit, indexed
( 1; 1), is the “readout qubit” that is measured at the end of the
circuit to get a prediction. The remaining qubits are the “data qubits”
which store the encoded MNIST image. Each two-qubit XX gate is
parameterized by a unique angle (the ith angle is labeled “xx-i”) which
is optimized over in the training phase.

At this point, the circuit has a two-qubit XX gate between the readout
qubit and all data qubits. Each XX gate is parameterized by an
independent angle, and we use the naming convention “xx-i” for the i th
angle. This particular circuit is shown in Figure 9.6. Next, we create
the full model. This model includes the data encoding and the QNN —
which we have discussed — as well as the final readout step. To
understand the readout step, consider the following: after propagating
the encoded data point through the QNN, we have some evolved quantum
state, and we need to get a label (here “the image is a 3” or “the image
is a 6”) from it. So, we need some way to map a quantum state to a
label. This is the purpose of the readout step. For binary
classification like we are considering here, a very natural thing to do
is measure a single qubit because this produces a binary outcome. We
adopt this strategy here and measure a single qubit (which we have
previously called the “readout qubit”). In particular, we will measure
the expectation of Pauli-Z on the readout qubit which produces a value
in the range Œ 1; 1. If the value is above zero, we assign it to one
class; else we assign it to the other class. def
create\_quantum\_model(): """Create a QNN model circuit and readout
operation to go along with it.""" data\_qubits = cirq.GridQubit.rect(4,
4) \# a 4x4 grid. readout = cirq.GridQubit(-1, -1) \# a single qubit at
\[-1,-1\] circuit = cirq.Circuit()

172

CHAPTER 9 Quantum Computing Methods

Prepare the readout qubit.
==========================

circuit.append(cirq.X(readout)) circuit.append(cirq.H(readout)) builder
= CircuitLayerBuilder( data\_qubits = data\_qubits, readout=readout) \#
Then add layers (experiment by adding more). builder.add\_layer(circuit,
cirq.XX, "xx1") builder.add\_layer(circuit, cirq.ZZ, "zz1") \# Finally,
prepare the readout qubit. circuit.append(cirq.H(readout)) return
circuit, cirq.Z(readout)

model\_circuit, model\_readout = create\_quantum\_model()

Now that we have the full quantum model, we can use it in TensorFlow
just like any other model. \# Build the Keras model. model =
tf.keras.Sequential(\[ \# The input is the data-circuit, encoded as a
tf.string tf.keras.layers.Input(shape=(), dtype=tf.string), \# The PQC
layer returns the expected value of the readout gate, range \[-1,1\].
tfq.layers.PQC(model\_circuit, model\_readout),\])

The last step before training the model is to define the loss function.
Since our readout value is in the range Œ 1; 1, the hinge loss is a
natural choice. def hinge\_accuracy(y\_true, y\_pred): y\_true =
tf.squeeze(y\_true) &gt; 0.0 y\_pred = tf.squeeze(y\_pred) &gt; 0.0
result = tf.cast(y\_true == y\_pred, tf.float32) return
tf.reduce\_mean(result)

y\_train\_hinge = 2.0 \* y\_train - 1.0 y\_test\_hinge = 2.0 \* y\_test
- 1.0

Note that we also map the labels to the range Œ 1; 1 in the last two
lines to use the hinge loss. Now we can compile the model with a loss
function, optimizer, and metric. model.compile(
loss=tf.keras.losses.Hinge(), optimizer=tf.keras.optimizers.Adam(),

SECTION 9.4 Machine Learning on Quantum Processors

173

metrics=\[hinge\_accuracy\], )

And finally train the model. EPOCHS = 3 BATCH\_SIZE = 32 NUM\_EXAMPLES =
len(x\_train\_tfcirc) x\_train\_tfcirc\_sub =
x\_train\_tfcirc\[:NUM\_EXAMPLES\] y\_train\_hinge\_sub =
y\_train\_hinge\[:NUM\_EXAMPLES\] qnn\_history = model.fit(
x\_train\_tfcirc\_sub, y\_train\_hinge\_sub, batch\_size=32,
epochs=EPOCHS, verbose=1, validation\_data=(x\_test\_tfcirc,
y\_test\_hinge) ) qnn\_results = model.evaluate(x\_test\_tfcirc,
y\_test)

In this example, we achieved 89.5% (hinge) accuracy. While this is not
up to par with state of the art classical machine learning models, it’s
not bad for a simple quantum model! The important part is to understand
each major step — pre-processing, data encoding, quantum neural network,
readout, and training — that makes up the quantum model. Can you change
one or more of these steps to improve the accuracy and get better
results? For this type of classification problem, it remains to be seen
whether a QNN has an advantage over a classical model. More generally,
advantages in quantum machine learning seem to be elusive in the early
stages of this field. For example, a quantum algorithm for
recommendation systems was proposed and assessed to have an exponential
speedup over the best known classical algorithm at the time of that work
\[151\]. The general idea of a recommendation system is as follows:
Given an incomplete preference matrix P of m users and their feedback on
n products, output a good recommendation for a particular user. Here,
“incomplete” means that entries of the matrix are missing — that is, not
every user has provided feedback for every product. Prior to the
proposed quantum algo for a recommendation system, the best classical
algorithm had a runtime that scaled linearly in the matrix dimension mn.
The quantum recommendation algorithm scales polylogarithmically in mn,
specifically as O.poly./polylog.mn// where  is the condition number of
P . However, a new classical algorithm, inspired by the quantum one,
also achieved polylogarithmic scaling in the

174

CHAPTER 9 Quantum Computing Methods

matrix dimension \[273\]. We say therefore that the quantum algo has
been “dequantized.” See the section on dequantization later in this
chapter for additional discussion of this important topic. Much research
continues to be done in quantum machine learning; see, for example,
\[138, 250, 283\], to explore the possibilities and prospects for this
relatively young field.

9.5

Quantum Phase Estimation

Quantum phase estimation (QPE), also known as the phase estimation
algorithm (PEA), is an algorithm for determining the eigenvalues of a
unitary operator. QPE was initially proposed by Kitaev \[152\] (see also
\[83\] for a discussion of QPE). Eigenvalue problems, which have the
form Ax D x m

m

(9.25)

m

where A 2 C2 2 , x 2 C2 and  2 C, are ubiquitous throughout
mathematics and physics. In mathematics, applications range from graph
theory to partial differential equations. In physics, applications
include computing the ground state energy — the smallest eigenvalue of
the Hamiltonian of the system — for nuclei, molecules, materials and
other physical systems. Moreover, principal component analysis (PCA), an
algorithm for reducing the dimensionality of feature vectors in machine
learning, has an eigenvalue problem at its core. The applications of
(9.25) range across a wide spectrum of disciplines. In the quantum case,
we are concerned with finding the eigenvalues of a unitary operator U .
It follows immediately by the definition of unitarity (U  U D I ) that
eigenvalues of a unitary operator have modulus one: jj D 1. Thus, any
eigenvalue  of a unitary operator can be written in the form  D e 2
i'

(9.26)

where 0  '  1 is called the phase. This is the same phase that appears
in the name of the algorithm — quantum phase estimation. By estimating
', we get an estimate of the eigenvalue  via the equation above.
Suppose ' can be written exactly using n bits5 5 This is the case where
' is rational. The general case of ' being irrational (requiring
infinitely many bits) is similar, but for simplicity we won’t cover it
here. See \[206\] for an explanation.

SECTION 9.5 Quantum Phase Estimation

' D 0:'1 '2    'n

175

(9.27)

This is a binary decimal representation of the phase '. Here, each 'k
for k D 1; :::; n is a binary digit 'k 2 f0; 1g. We can write this
equivalently as 'D

n X

'k 2

k

(9.28)

kD1

The key to understanding QPE is to consider the action of controlling
the unitary operator on an eigenstate j i. Explicitly, let U be a
unitary operator which we take as input to the QPE algorithm such that U
j i D j i

(9.29)

Suppose for now we have the eigenstate j i. This is not a requirement
for QPE — in fact, it makes the algorithm trivial, for if we knew j i we
could just implement U j i on the quantum computer — it just simplifies
the explanation. Now, suppose we prepare the equal superposition state
(ignoring normalization factors) in the first register and the
eigenstate of U in the second register .j0i C j1i/ ˝ j i D j0ij i C j1ij
i (9.30) Now, as mentioned, we implement a controlled-U operation on
this state, which produces the following state: j0ij i C j1iU j i D j0ij
i C e 2 i 0:'1 'n j1ij i D .j0i C e 2 i 0:'1 'n j1i/ ˝ j i Note
that the second register goes unchanged. Since j i is an eigenstate of U
, it is unaffected by the controlled operation. Why did we do this then?
We encoded the information about the phase into the first region.
Specifically, the state in the first register picked up the relative
phase e 2 i 0:'1 'n . k Phase estimation now tells us to implement
controlled-U 2 operations for integers k D 0; :::; n 1. We already
performed the k D 0 case above. Consider now the effect of U 2 ; in
particular, U 2 j i D 2 j i D e 2 i.2'/ j i D e 2 i 0:'2 'n j i

(9.31)

In the last step, we used the fact that e 2 i'1 D 1 for any '1 2 f0;
1g. Thus, by preparing the equal superposition state in the first
register, the eigenstate j i in the second register (9.30), then
performing a controlled-U 2 operation, we get the state

176

CHAPTER 9 Quantum Computing Methods

j0ij i C j1iU 2 j i D j0ij i C e 2 i 0:'2 'n j1ij i In general,
using this same idea, we can see that k

k

k '/

U 2 j i D 2 j i D e 2 i.2

j i D e 2 i 0:'kC1 'n

(9.32)

1.  Hence, we can transform (9.30) under a controlled-U 2

for k D 0; :::; n as

k

k

j0ij i C j1ij i 7 ! j0ij i C j1iU 2 j i D .j0i C e 2 i 0:'kC1 'n
j1i/ ˝ j i (9.33) Equation (9.33) is at the heart of the QPE algorithm.
In particular, the algorithm says to implement this operation
iteratively for k D 0; :::; n 1, using n qubits in the top register with
the eigenstate j i in the bottom register. The full circuit for QPE is
shown below: j0i

H

j0i

H

 

QFT

:: : j0i j i

:: :



H U2

0

U2

1



U2

n 1

k

After implementing the series of controlled-U 2 operations, the top
register is in the state .j0i C e 2 i0:'1 'n j1i/ ˝ .j0i C e 2 i
0:'2 'n j1i/ ˝    ˝ .j0i C e 2 i 0:'n j1i/ (9.34) To extract the
phase information from this state, we use the inverse Fourier transform,
which transforms this state to a product state j'1 i ˝ j'2 i ˝    ˝
j'n i

(9.35)

By measuring in the computational basis, we thus learn the bits '1 ; '2
; :::; 'n , which allow us to construct ' D 0:'1    'n and the
eigenvalue  D e 2 i'

(9.36)

177

SECTION 9.5 Quantum Phase Estimation

Implemention of QPE We now turn to an example implementation of QPE
using Cirq. Here, we consider computing the eigenvalues of the unitary U
DX ˝Z

(9.37)

We can see that the eigenvalues of U are, of course, ˙1. We will see
that QPE returns these eigenvalues as well. First, we import the
necessary packages \# Imports import numpy as np import cirq

and then define a helper function for converting from bitstrings in
binary decimal notation to numeric values: def binary\_decimal(string):
"""Returns the numeric value of 0babc... where a, b, c, ... are bits.
Examples: 0b10 --&gt; 0.5 0b01 --&gt; 0.25 """ val = 0.0 for (ind, bit)
in enumerate(string\[2:\]): if int(bit) == 1: val += 2\*\*(-1 -ind)
return val

Now we define the number of qubits in the bottom register of the QPE
circuit, create the unitary matrix and classically diagonalize it. We
will use these eigenvalues to compare to the ones found by QPE. \#
Number of qubits and dimension of the eigenstate m = 2 \# Get a unitary
matrix on two qubits xmat = np.array(\[\[0, 1\], \[1, 0\]\]) zmat =
np.array(\[\[1, 0\], \[0, -1\]\]) unitary = np.kron(xmat, zmat) \# Print
it to the console print("Unitary:") print(unitary) \# Diagonalize it
classically evals, \_ = np.linalg.eig(unitary)

178

CHAPTER 9 Quantum Computing Methods

The output of this portion of the code follows: Unitary: \[\[ 0 0 1
0\]\[ 0 0 0 -1\] \[ 1 0 0 0\]\[ 0 -1 0 0\]\]

Now that we have our input to QPE, we can begin building the circuit. As
described above, we define the number of qubits in our top register to
determine the accuracy of the eigenvalues found. Here, we set this
number and define two registers of qubits. Next, we create a circuit and
apply the Hadamard gate to each qubit in the top (readout) register. \#
Number of qubits in the readout/answer register (\# bits of precision) n
= 2 \# Readout register regA = cirq.LineQubit.range(n) \# Register for
the eigenstate regB = cirq.LineQubit.range(n, n + m) \# Get a circuit
circ = cirq.Circuit() \# Hadamard all qubits in the readout register
circ.append(cirq.H.on\_each(\*regA))

The next step in the QPE algorithm is to implement the series of
controlled k U 2 operations. We show how this can be done in Cirq for
arbitrary two-qubit unitaries written as matrices. First, we create a
TwoQubitMatrixGate from the unitary matrix, then make a controlled
version. \# Get a Cirq gate for the unitary matrix ugate =
cirq.ops.matrix\_gates.TwoQubitMatrixGate(unitary) \# Controlled version
of the gate cugate = cirq.ops.ControlledGate(ugate)

Now that we have the controlled-U gate, we can implement the sequence of
transforms with the following code block: \# Do the controlled U^{2^k}
operations for k in range(n): circ.append(cugate(regA\[k\],
\*regB)**(2**k))

SECTION 9.5 Quantum Phase Estimation

179

The last step in QPE is to implement the inverse quantum Fourier
transform and measure all qubits in the computational basis. This is
done in the following code block. \# Do the inverse QFT for k in range(n
- 1): circ.append(cirq.H.on(regA\[k\])) targ = k + 1 for j in
range(targ): exp = -2\*\*(j - targ) rot = cirq.Rz(exp) crot =
cirq.ControlledGate(rot) circ.append(crot(regA\[j\], regA\[targ\]))
circ.append(cirq.H.on(regA\[n - 1\])) \# Measure all qubits in the
readout register circ.append(cirq.measure(\*regA, key="z"))

Now that we have built our QPE circuit, we can run it and process the
results. The code below simulates the circuit and grabs the top two most
frequent measurement outcomes. We can obtain '1 and '2 from each of
these to compute our eigenvalues. \# Get a simulator sim =
cirq.Simulator() \# Simulate the circuit and get the most frequent
measurement outcomes res = sim.run(circ, repetitions=1000) hist =
res.histogram(key="z") top = hist.most\_common(2)

Even though we do not start the second register in an eigenstate of the
unitary U , we can think of starting the second register in a linear
combination of its eigenstates since the eigenstates of U form an
orthonormal basis; in other words, any vector can be expressed as a
linear combination of the eigenstates for some coefficients. In
particular, we started the second register in the ground state j0i,
which we can write as X j0i D cj jj i (9.38) j

where jj i are the eigenstates of U . The most probable measurement
outcomes are thus those with large jcj j D jh0jj ij. Now that we have
the most frequently measured bitstrings, we can convert these to
numerical values of the phase ' and then to eigenvalues. The code below
performs these operations and prints out the eigenvalues computed by QPE
and the eigenvalues computed by the classical matrix diagonalization
algorithm.

180

CHAPTER 9 Quantum Computing Methods

Eigenvalues from QPE
====================

estimated = \[np.exp(2j \* np.pi \* binary\_decimal(bin(x\[0\]))) for x
in top\] \# Print out the estimated eigenvalues
print("\nEigenvalues from QPE:") print(set(sorted(estimated, key=lambda
x: abs(x)**2))) \# Print out the actual eigenvalues
print("\nActual eigenvalues:") print(set(sorted(evals, key=lambda x:
abs(x)**2)))

The output of this code, shown below, reveals that QPE finds the correct
eigenvalues within numerical roundoff precision. Eigenvalues from QPE:
{(1+0j), (-1+1.2246467991473532e-16j)} Actual eigenvalues: {1.0, -1.0}

The complete program for this implementation can be found on the book’s
online website. One can change the unitary matrix to compute eigenvalues
and compare them to the ones found classically. Additionally, one can
change the number of qubits in the top register n to get more bits of
precision for more complex unitary operators.

9.6

Solving Linear Systems

The problem of solving a linear system of M equations with N variables
is ubiquitous in mathematics, science and engineering. The formal
statement of the problem is as follows: Given an M  N matrix A and a
solution vector b, find a vector x such that Ax D b

(9.39)

Linear algebra tells us how to solve this problem classically in the
case that A is invertible:6 x D A 1b (9.40) However, although we can
write down the solution immediately, numerically computing x is
intractable for large matrices. 6 Please

consult Part III: Toolkit for a review of these mathematical concepts.

SECTION 9.6 Solving Linear Systems

181

Explicitly computing the inverse of A is generally the most costly
method. In practice, most general-purpose numerical solvers use Gaussian
elimination and back-substitution, which runs in O.N 3 / time. In this
discussion we restrict ourselves to square matrices, i.e., M D N .
Faster classical algorithms are possible: if the matrix A has sparsity s
and condition number , solving the system to accuracy  can be done by
the conjugate gradient algorithm in O.N s log.1=// time, which is a
considerable speedup compared with O.N 3 /. The quantum version of
solving systems of linear equations — called the quantum linear systems
problem (QLSP) \[87\] — is similar to the classical approach. Let A be
an N  N Hermitian matrix with unit determinant. Let b and x be N
-dimensional vectors such that x D A 1 b. Define the quantum states jbi
and jxi on n D log2 N qubits P bi jii jbi D P i (9.41) jj i bi ji ijj2
and

P xi ji i jxi D P i jj i xi ji ijj2

(9.42)

Here, bi is the i th component of b, and similarly for xi . The goal of
the QLSP is as follows: given access to the matrix A (whose elements are
accessed by an oracle) and the state jbi, output a state jxi N such that
jjjxi N jxijj2   (9.43) with probability greater than 1=2. A quantum
algorithm for solving the QLSP in time O.log.N /s 2  2 =/ was
discovered by Harrow, Hassidim and Lloyd \[135\]. The algorithm is
commonly known as the HHL algorithm after its developers. Note that the
order of HHL is logarithmic, however, this is not always the case in
practice. As Aaronson has pointed out: ...the HHL algorithm solves Ax =
b in logarithmic time, but it does so with four caveats...each of which
can be crucial in practice. To make a long story short, HHL is not
exactly an algorithm for solving a system of linear equations in
logarithmic time. Rather, it’s an algorithm for approximately preparing
a quantum superposition of the form jxi, where x is the solution to a
linear system Ax = b, assuming the ability to rapidly prepare

182

CHAPTER 9 Quantum Computing Methods

the state jxi, and to apply the unitary transformation e iAt , and using
an amount of time that grows roughly like s.log.n//=, where n is the
system size,  is the system’s condition number, s is its sparsity and 
is the desired error \[4\]. In the remainder of this section, we explain
the mathematics of HHL and then turn to an example implementation. HHL
uses several quantum algorithms we have discussed — such as Hamiltonian
and quantum phase estimation — as subroutines.

Description of the HHL Algorithm The HHL algorithm uses three registers
of qubits, which we denote as A for ancilla, W for work, and IO for
input/output. The input to the algorithm is the quantum state jbi,
defined above, which is input to the IO register. The other registers
start off in the j0i state, so the entire initial state input to HHL can
be written j 0 i WD j0iA ˝ j0iW ˝ jbiIO (9.44) We are also given the
matrix A as input. There should be no confusion between the matrix and
the register, for we will refer to the former as “matrix A” and the
latter as “register A.” There are three main steps to the algorithm: 1.
Quantum phase estimation with the unitary UA WD e iAt , controlled by
the W register and UA applied to the IO register. 2. Pauli-Y rotation
for a particular angle  (discussed below) on the A register controlled
by the W register. 3. Implement the first step in reverse (known as
uncomputation) on the W register. If the A register is measured and one
post-selects on the j1iA outcome, then the state of the IO register will
be close to jxi. We now walk through the steps to show this. Let the
matrix A be written in its eigenbasis X AD j juj ihuj j (9.45) j

For simplicity, we assume for the moment that jbi is one of the
eigenvectors of A. That is, jbi D juj i for some index j . This
assumption will be relaxed momentarily. We can assume A is Hermitian
without loss of generality, since if A is not Hermitian, we can form a
Hermitian matrix

SECTION 9.6 Solving Linear Systems

183

  0 A Q A WD A 0 Q Since A is Hermitian, the operator and perform HHL
with A. UA WD e iAt

(9.46)

is unitary and has eigenvalues e i j t and eigenstates juj i. After the
first step of HHL, QPE brings us to the state j

1i

WD j0iA ˝ jQ j iW ˝ juj iIO

(9.47)

Here, Q j is a binary representation of j up to a set precision. Note
that we used our assumption jbi D juj i when writing the result of QPE.
We now implement the second step of QPE, a controlled-Y rotation e iY
for the angle C  D arccos (9.48) Q Here, C is a hyperparameter set by
the user of the algorithm. In the example implementation below, we
discuss setting the value of C . After this rotation controlled on the O
register, we have the state v u u C2 C j 2 i WD t1 j0iA ˝ jQ j iW ˝ juj
iIO C j1iA ˝ jQ j iW ˝ juj iIO 2 Q Q j j

(9.49) We now relax the assumption that jbi is an eigenstate of A. That
is, we relax the assumption that jbi D juj i for some j . Note that we
can write without any assumptions, however, that X jbi D ˇj juj i (9.50)
j

where ˇj D huj jbi are complex coefficients. We can write this because A
is Hermitian and so its eigenstates form an orthonormal basis. We now
perform the above analysis (9.45) — (9.49) with jbi expressed in the
eigenbasis (9.50). Doing so, we end up with the state 2v 3 u N 2 X u C C
j 3 i WD ˇj 4t1 j0i C j1i 5 ˝ jQ j iW ˝ juj iIO (9.51) Q2 A Q j A j
D1

j

184

CHAPTER 9 Quantum Computing Methods

The next step of HHL is to uncompute the W register. Doing so sends Q
jj iO ! j0iO . Since this state is the all zeros state, we can omit it
and write the state after uncomputing as 2v 3 u N 2 X u C C j 4 i WD ˇj
4t1 j0iA C j1iA 5 ˝ juj iIO (9.52) Q 2 Q j j

j D1

This state is in a very useful form, though it may take a careful look
to see why. The reason is that A

1

N X ˇj jbi D juj i j

(9.53)

j D1

Thus, if we measure the A register and post-select on the j1iA outcome,
then (9.52) becomes (ignoring the A register) N X ˇj j 5 i WD juj iIO 
jxi: Q j

(9.54)

j D1

Thus, the IO register contains an approximation to jxi D A 1 jbi. Note
that this solves the quantum linear systems problem exponentially faster
than the best known classical algorithm. Like Shor’s algorithm and QPE,
HHL is a demonstration of potential quantum advantage. However, note
that only a quantum description of the solution vector is output from
HHL. For applications that need a full classical description of x, this
may not be satisfactory. Quantum state tomography — which is the
measurement and characterization of the wavefunction of a quantum system
— can be used to read out each amplitude of jxi, but this takes time
that scales exponentially in the number of qubits. Fortunately, there
exists a number of applications where only certain features of the
solution x need to be computed, for example the total weight of some
subset of the indices. Now that we have walked through the HHL
algorithm, let us turn to an example implementation written in Cirq:

Example Implementation of the HHL Algorithm In this implementation7 , we
consider for simplicity a 2  2 system of linear equations. In
particular, the matrix A we consider is 7 Adapted

from https://github.com/quantumlib/Cirq/blob/master/examples/hhl.py

185

SECTION 9.6 Solving Linear Systems



4:302134 AD 0:235318

6:015934  10 9:343883  10

8i 1i

0:235318 C 9:343861  10 0:583865 C 6:015934  10

1i



8i

(9.55) and we take the vector jbi as jbi D Œ0:64510

0:47848i 0:35490

0:47848i T

(9.56)

Our goal is to use HHL to compute Pauli expectation values hxj jxi
where  2 fX; Y; Zg. We can easily compute these analytically (after
classically solving the system) to be hxjX jxi D 0:144130 hxjY jxi D
0:413217 hxjZjxi D

0:899154

We will compare the expectation values obtained by HHL to these
expectation values. In our program, we first import the packages we will
use: import math import numpy as np import cirq

and then build up the HHL circuit. Here, we define classes which are new
gates in Cirq by inheriting from cirq.Gate or related objects. First, we
create a gate representing UA D e iAt which we will use in the QPE
steps: class HamiltonianSimulation(cirq.EigenGate,
cirq.SingleQubitGate): """A gate that implements e\^iAt. If a large
matrix is used, the circuit should implement actual Hamiltonian
simulation, for example by using the linear operators framework in Cirq.
""" def **init**(self, A, t, exponent=1.0): """Initializes a
HamiltonianSimulation. Args: A : numpy.ndarray Hermitian matrix that
defines the linear system Ax = b. t : float Simulation time.
Hyperparameter of HHL. """ cirq.SingleQubitGate.**init**(self)
cirq.EigenGate.**init**(self, exponent=exponent)

186

CHAPTER 9 Quantum Computing Methods self.A = A self.t = t ws, vs =
np.linalg.eigh(A) self.eigen\_components = \[\] for w, v in zip(ws,
vs.T): theta = w\*t / math.pi P = np.outer(v, np.conj(v))
self.eigen\_components.append((theta, P))

def \_with\_exponent(self, exponent): return
HamiltonianSimulation(self.A, self.t, exponent) def
\_eigen\_components(self): return self.eigen\_components

Next, we implement the series of controlled unitary operations in QPE,
known as the phase kickback portion of the circuit (please refer to
chapter 8 for a discussion of phase kickback): class
PhaseKickback(cirq.Gate): """A gate for the phase kickback stage of
Quantum Phase Estimation. Consists of a series of controlled e\^iAt
gates with the memory qubit as the target and each register qubit as the
control, raised to the power of 2 based on the qubit index. """ def
**init**(self, num\_qubits, unitary): """Initializes a PhaseKickback
gate. Args: num\_qubits : int The number of qubits in the readout
register + 1. Note: The last qubit stores the eigenvector; all other
qubits store the estimated phase, in big-endian. unitary : numpy.ndarray
The unitary gate whose phases will be estimated. """
super(PhaseKickback, self) self.\_num\_qubits = num\_qubits self.U =
unitary def num\_qubits(self): """Returns the number of qubits."""
return self.\_num\_qubits def *decompose*(self, qubits): """Generator
for the phase kickback circuit.""" qubits = list(qubits)

SECTION 9.6 Solving Linear Systems

187

memory = qubits.pop() for i, qubit in enumerate(qubits): yield
cirq.ControlledGate(self.U**(2**i))(qubit, memory)

Next, we create a quantum Fourier transform gate, the third and final
component of QPE: class QFT(cirq.Gate): """Quantum gate for the Quantum
Fourier Transformation. Note: Swaps are omitted here. These are
implicitly done in the PhaseKickback gate by reversing the control qubit
order. """ def **init**(self, num\_qubits): """Initializes a QFT
circuit. Args: num\_qubits : int Number of qubits. """ super(QFT, self)
self.\_num\_qubits = num\_qubits def num\_qubits(self): return
self.\_num\_qubits def *decompose*(self, qubits): processed\_qubits =
\[\] for q\_head in qubits: for i, qubit in
enumerate(processed\_qubits): yield cirq.CZ(qubit,
q\_head)**(1/2.0**(i+1)) yield cirq.H(q\_head)
processed\_qubits.insert(0, q\_head)

Now that we have the three major components of QPE, we can implement the
entire algorithm. As above, we make the QPE instance a gate in Cirq:
class QPE(cirq.Gate): """A gate for Quantum Phase Estimation.""" def
**init**(self, num\_qubits, unitary): """Initializes an HHL circuit.
Args: num\_qubits : int The number of qubits in the readout register.
Note: The last qubit stores the eigenvector; all other qubits store the
estimated phase, in big-endian. unitary : numpy.ndarray The unitary gate
whose phases will be estimated.

188

CHAPTER 9 Quantum Computing Methods

""" super(QPE, self) self.\_num\_qubits = num\_qubits self.U = unitary
def num\_qubits(self): return self.\_num\_qubits def *decompose*(self,
qubits): qubits = list(qubits) yield cirq.H.on\_each(*qubits\[:-1\])
yield PhaseKickback(self.num\_qubits(), self.U)(*qubits) yield
QFT(self.\_num\_qubits-1)(\*qubits\[:-1\])\*\*-1

With the unitary set as UA D e iAt , this instance of QPE will make up
the first part of the HHL algorithm. The next step is to implement the
controlled Pauli-Y rotation, which the following class does: class
EigenRotation(cirq.Gate): """EigenRotation performs the set of rotation
on the ancilla qubit equivalent to division on the memory register by
each eigenvalue of the matrix. The last qubit is the ancilla qubit; all
remaining qubits are in the register, assumed to be big-endian. It
consists of a controlled ancilla qubit rotation for each possible value
that can be represented by the register. Each rotation is an Ry gate
where the angle is calculated from the eigenvalue corresponding to the
register value, up to a normalization factor C. """ def **init**(self,
num\_qubits, C, t): """Initializes an EigenRotation. Args: num\_qubits :
int Number of qubits. C : float Hyperparameter of HHL algorithm. t :
float Parameter. """ super(EigenRotation, self) self.\_num\_qubits =
num\_qubits self.C = C self.t = t self.N = 2\*\*(num\_qubits-1)

SECTION 9.6 Solving Linear Systems

189

def num\_qubits(self): return self.\_num\_qubits def *decompose*(self,
qubits): for k in range(self.N): kGate = self.\_ancilla\_rotation(k) \#
xor’s 1 bits correspond to X gate positions. xor = k \^ (k-1) for q in
qubits\[-2::-1\]: \# Place X gates if xor % 2 == 1: yield cirq.X(q) xor
&gt;&gt;= 1 \# Build controlled ancilla rotation kGate =
cirq.ControlledGate(kGate) yield kGate(\*qubits) def
\_ancilla\_rotation(self, k): if k == 0: k = self.N theta =
2*math.asin(self.C * self.N \* self.t / (2*math.pi * k)) return
cirq.Ry(theta)

Now that we have built up each component of the HHL algorithm, we can
write a function to build the entire circuit, shown below: def
hhl\_circuit(A, C, t, register\_size, \*input\_prep\_gates):
"""Constructs the HHL circuit and returns it. Args: A : numpy.ndarray
Hermitian matrix that defines the system of equations Ax = b. C : float
Hyperparameter for HHL. t : float Hyperparameter for HHL C and t are
tunable parameters for the algorithm. register\_size is the size of the
eigenvalue register. input\_prep\_gates is a list of gates to be applied
to |0&gt; to generate the desired input state |b&gt;. """ \# Ancilla
register ancilla = cirq.GridQubit(0, 0) \# Work register

190

CHAPTER 9 Quantum Computing Methods

register = \[cirq.GridQubit(i + 1, 0) for i in range(register\_size)\]
\# Input/output register memory = cirq.GridQubit(register\_size + 1, 0)
\# Create a circuit circ = cirq.Circuit() \# Unitary e\^{iAt} for QPE
unitary = HamiltonianSimulation(A, t) \# QPE with the unitary e\^{iAt}
qpe = QPE(register\_size + 1, unitary) \# Add state preparation circuit
for |b&gt; circ.append(\[gate(memory) for gate in input\_prep\_gates\])
\# Add the HHL algorithm to the circuit circ.append(\[ qpe(*(register +
\[memory\])), EigenRotation(register\_size+1, C,
t)(*(register+\[ancilla\])), qpe(\*(register + \[memory\]))\*\*-1,
cirq.measure(ancilla)\]) \# Pauli observable display circ.append(\[
cirq.pauli\_string\_expectation( cirq.PauliString({ancilla: cirq.Z}),
key="a" ), cirq.pauli\_string\_expectation( cirq.PauliString({memory:
cirq.X}), key="x" ), cirq.pauli\_string\_expectation(
cirq.PauliString({memory: cirq.Y}), key="y" ),
cirq.pauli\_string\_expectation( cirq.PauliString({memory: cirq.Z}),
key="z" ),\]) return circ

In this function, we define the three qubit registers for HHL and create
an empty circuit. Then we form the unitary UA D e iAt from the input
matrix A for a given time t and form a QPE circuit using that unitary.
The next line implements the state preparation circuit to prepare jbi
from the ground state. Note that while jbi is assumed as input to HHL,
in practice we always need a state preparation circuit.

SECTION 9.6 Solving Linear Systems

191

After this, the HHL circuit is constructed step-by-step; first, we add
the QPE circuit, then the controlled-Y rotation, then the inverse QPE
circuit. Note that we are using the \*\*-1 notation in Cirq which makes
it very easy to get the inverse of a quantum circuit. Finally, we append
Pauli operators to make it easy to compute expectation values. Now that
we have built the circuit for HHL, we can simulate it to run the
algorithm. The following function inputs an HHL circuit, simulates it,
and prints out the expectation values from the input/output (IO)
register after post-selecting the j1i outcome in the ancilla register.
Finally, we write our main function which defines the linear system A,
input state jbi and any hyperparameters needed for the HHL algorithm:
def main(): """Runs the main script of the file.""" \# Constants t =
0.358166 \* math.pi register\_size = 4 \# Define the linear system A =
np.array(\[\[4.30213466-6.01593490e-08j, 0.23531802+9.34386156e-01j\],
\[0.23531882-9.34388383e-01j, 0.58386534+6.01593489e-08j\]\]) \# The
|b&gt; vector is defined by these gates on the zero state \# |b&gt; =
(0.64510-0.47848j, 0.35490-0.47848j) input\_prep\_gates =
\[cirq.Rx(1.276359), cirq.Rz(1.276359)\] \# Expected expectation values
expected = (0.144130 + 0j, 0.413217 + 0j, -0.899154 + 0j) \# Set C to be
the smallest eigenvalue that can be represented by the \# circuit. C =
2\*math.pi / (2\*\*register\_size \* t) \# Print the actual expectation
values print("Expected observable outputs:") print("X =", expected\[0\])
print("Y =", expected\[1\]) print("Z =", expected\[2\]) \# Do the HHL
algorithm and print the computed expectation values print("\nComputed:
") hhlcirc = hhl\_circuit(A, C, t, register\_size, \*input\_prep\_gates)
expectations(hhlcirc) if **name** == "**main**": main()

192

CHAPTER 9 Quantum Computing Methods

The output of this program is shown below: Expected observable outputs:
X = (0.14413+0j) Y = (0.413217+0j) Z = (-0.899154+0j) Computed: X =
(0.14413303+0j) Y = (0.41321677+0j) Z = (-0.89915407+0j)

As can be seen, HHL returns the correct (approximate) expectation values
for each Pauli operator, indicating that the final state jxi N is indeed
close to the solution vector jxi.

9.7

Quantum Random Number Generator

Generating random numbers is crucial for many applications and
algorithms, including Monte Carlo methods and cryptography. While
classical computers generate pseudorandom numbers, the random numbers
generated by quantum computers are guaranteed to be truly random by the
laws of quantum mechanics. In this section, we consider a simple
algorithm for generating truly random numbers on current quantum
processors. The algorithm applies a Hadamard gate to a qubit in the
ground state, then measures the state of the qubit in the computational
basis. As we have seen, the Hadamard gate acting on j0i generates a
superposition of computational basis states with equal amplitudes: 1 H
j0i D p .j0i C j1i/ 2

(9.57)

When this state is measured, there is therefore an equal probability of
obtaining the ground and excited states. This can be exploited
computationally as a random bit generator. Let us now walk through an
example program for generating random bits in Cirq. This program creates
a circuit with one qubit, applies the Hadamard gate and then performs a
measurement; the program then iterates the circuit ten times in the
simulator. """Program for generating random bits in Cirq.""" \# Imports
import cirq

SECTION 9.7 Quantum Random Number Generator

193

Helper function for visualizing output
======================================

def bitstring(bits): return ’’.join(’1’ if e else ’0’ for e in bits) \#
Get a qubit and quantum circuit qbit = cirq.LineQubit(0) circ =
cirq.Circuit() \# Add the Hadamard and measure operations to the circuit
circ.append(\[cirq.H(qbit), cirq.measure(qbit, key="z")\]) \# Simulate
the circuit sim = cirq.Simulator() res = sim.run(circ, repetitions=10)
\# Print the outcome print("Bitstring =",
bitstring(res.measurements\["z"\]))

An example output of this program is shown below: Bitstring = 0011001011

Note that this output can be interpreted in several ways, depending on
the context. One interpretation is a sequence of random bits, while
another is a random bitstring representing, for example, an integer. In
base ten, the integer produced in this example output is 203. In this
sense, the program can be interpreted as a uniform random number
generator in the integer interval Œ0; N / where N is the number of
repetitions of the circuit. It is also possible to generate a random
number in the range Œ0; N / by using n D log2 N qubits. Here, instead of
simulating a circuit with one qubit many times, we apply a Hadamard gate
on each of the n qubits, then measure. Since there are 2n D N possible
bitstrings for n qubits, this will also generate a random bitstring that
can be interpreted as an integer in the range Œ0; N /. A program that
implements this in Cirq is shown below: """Program for generating random
numbers in Cirq.""" \# Imports import cirq \# Number of qubits n = 10 \#
Helper function for visualizing output def bitstring(bits): return
’’.join(’1’ if e else ’0’ for e in bits) \# Get a qubit and quantum
circuit qreg = \[cirq.LineQubit(x) for x in range(n)\]

194

CHAPTER 9 Quantum Computing Methods

circ = cirq.Circuit() \# Add the Hadamard and measure operations to the
circuit for x in range(n): circ.append(\[cirq.H(qreg\[x\]),
cirq.measure(qreg\[x\])\]) \# Simulate the circuit sim =
cirq.Simulator() res = sim.run(circ, repetitions=1) \# Print the
measured bitstring bits = bitstring(res.measurements.values())
print("Bitstring =", bits) \# Print the integer corresponding to the
bitstring print("Integer =", int(bits, 2))

Here, we use n D 10 qubits to generate a random number in the range Œ0;
1024/. An example output of this program is shown below: Bitstring =
1010011100 Integer = 668

Here, the integer is the bitstring in base 10. This program produces
uniform random numbers in the range Œ0; 1024/ and will produce different
integers if run successive times.

9.8

Quantum Walks

Quantum walks have been shown to have computational advantages over
classical random walks \[10, 12, 74, 75, 76, 108, 149\]. In the
classical setting, a particle starts out in some initial position
(vertex) on a graph G D .V; E/ and “walks” to neighboring vertices in a
probabilistic manner; these are classical random walks. The final
probability distribution of finding the particle at a given vertex V —
as well as questions such as “how long does it take the particle to
reach a particular vertex?” — are interesting and useful quantities to
calculate. When certain problems are phrased in terms of random walks,
for example the 2-SAT problem, computing these quantities can lead to
novel solutions that may not have been known previously. The simplest
example of a classical random walk is a one-dimensional walk on a line.
Consider a particle starting at position x.t D 0/ D 0 at time t D 0. At
time t D 1, the particle moves to the right (x.1/ D 1) or left (x.t D 1/
D 1) with equal probability. At time t D 1, we have x.2/ D x.1/ ˙ 1 with
equal probability, and in general x.t / D x.t 1/ ˙ 1

SECTION 9.8 Quantum Walks

195

with equal probability. Because steps are made at only discrete
increments of time t D 1; 2; 3; :::, this is known as a discrete-time
random walk. Continuoustime random walks are another model which we
discuss below. Classical random walks are implemented by generating
pseudo-random number(s) at each time step. The particle’s position is
updated at each iteration according to the outcome of the random number
generator. Alternatively, an array of values representing probabilities
for each position can be stored and updated via a stochastic matrix
which determines the time evolution of the system. In the case of a
discrete-time quantum walk on a line, the idea is similar but the
implementation is different. The quantum walk consists of two registers
of qubits: a position register P and a coin register C . As the name
suggests, the position register tracks the probability distribution for
the particle to be at a particular position j0i, j1i, ..., jN 1i, where
we impose periodic boundary conditions jN i D j0i. The coin register is
used to update the particle’s position at each time step. The update to
the particle’s position is given by the shift operator X X S WD j0ih0jC
˝ ji 1ihi jP C j1ih1jC ˝ ji C 1ihi jP (9.58) i

i

That is, if the coin register is in the j1i state, the particle shifts
to the left, and if the coin register is in the j0i state, the particle
shifts to the right. That is, S j0iC ˝ ji iP D j0iC ˝ ji

1iP

(9.59)

Sj1iC ˝ ji iP D j1iC ˝ ji C 1iP

(9.60)

and The coin is “flipped” by applying a single qubit gate — for example
the Hadamard gate H to produce an equal superposition state, though
“biased” coins can also be used — and then the shift operator is
applied. One step of the quantum walk can thus be written U D S.HC ˝ IP
/

(9.61)

where HC is the Hadamard acting on the coin and IP refers to the
identity acting on the particle. T steps of the walk are given by U T .
In this simplest example of a random walk, numerous differences between
the classical and quantum cases can already be seen. For example,
starting in the initial state j0iC ˝ j0iP will cause the probability
distribution to drift “to the left” — that is, the particle is more
likely to move to the left — whereas

196

CHAPTER 9 Quantum Computing Methods

in the classical case the distribution is symmetric. Starting the
quantum walk in the state j1iC ˝ j0iP will cause the distribution to
drift to the right. The reasons for this are constructive and
destructive interference of amplitudes, a distinctly quantum phenomena
that is not possible in the classical case. Note that the distribution
for quantum walk can be made symmetric — p by starting in the state jCiC
˝ j0iP , for example, where jCi D .j0i C j1i/= 2. This simple example is
instructive for understanding both how quantum walks work and how
quantum walks are different that classical walks. Upon further study,
more differences can be seen. For example, the variance of the classical
distribution for a discrete-time random walk on a line is c2 D T after
T time steps, but in the quantum case it is q2 D T 2 \[150\]. Thus, the
quantum walker propagates quadratically faster than the classical one.
For a review of quantum walks, see \[150\] and \[235\] and the
references therein. For an example of quantum walks applied to graphs,
see \[10\]. Farhi et al. demonstrated speedup for NAND trees with
quantum walks \[103\]. Let us now turn to an example implementation of a
quantum walk to get more experience.

Implementation of a Quantum Walk In this section we provide an example
implementation of a continuous time quantum walk (CTQW). We first
discuss the transition from discrete to continuous classical walk, as
this will reveal how we perform a continuous quantum walk. In a
discrete-time classical walk, probability distributions are stored in a
vector p which is updated via a stochastic matrix p.t C 1/ D M p.t /

(9.62)

This operates only at discrete times. To make it continuous, we rewrite
this equation as a differential equation d p.t / D dt

H p.t/

where H is a time-independent matrix with elements given by 8 ˆ i ¤ j
and .i; j / 2 E &lt; hi jH jj i D 0 i D j and .i; j / 62 E ˆ : di i Dj

(9.63)

(9.64)

Here, is the constant transition rate from vertex i to vertex j and di
is the degree (i.e., number of edges) of vertex i .

SECTION 9.8 Quantum Walks

197

The solution for this differential equation is known to be p.t/ D e H t
p.0/. The step to making this a continuous time quantum walk is to treat
the matrix H as a Hamiltonian which generates the unitary evolution U.t
/ D e

iH t

(9.65)

which is defined for a continuous, not discrete, spectrum of times t.
Let us now turn to the example implementation using pyQuil8 . Here we
perform a continuous time quantum walk on a complete graph with four
vertices (nodes), commonly denoted K4 . A complete graph is one in which
each vertex is connected to all vertices. We first import the packages
we will use for this implementation. We highlight here the use of
networkx, a common Python package for working with graphs. import numpy
as np import networkx as nx import matplotlib.pyplot as plt from
scipy.linalg import expm import pyquil.quil as pq import pyquil.api as
api from pyquil.gates import H, X, CPHASE00

We now create a complete graph on four nodes and visualize it: \# Create
a graph G = nx.complete\_graph(4) nx.draw\_networkx(G)

The output of this portion of the program is shown in Figure 9.7. Note
that each vertex has an edge connecting it to all other vertices. The
spectrum of a complete graph (i.e., the eigenvalues of the adjacency
matrix of a complete graph) is quite simple. It is known from graph
theory that one eigenvalue is equal to N 1 (where N is the number of
nodes) and the remaining eigenvalues are equal to 1. In the following
code block, we get the adjacency matrix of the K4 graph and diagonalize
it to verify the spectrum is what we expect. \# Diagonalize the
adjacency matrix A = nx.adjacency\_matrix(G).toarray() eigvals, \_ =
np.linalg.eigh(A) print("Eigenvalues =", eigvals)

8 This implementation is adapted from open-source code which can be
found at
https://github.com/rigetti/pyquil/blob/master/examples/quantum\_walk.ipynb.

198

CHAPTER 9 Quantum Computing Methods

Figure 9.7: A complete graph on four vertices which we implement a
continuous time quantum walk on. This graph is denoted K4 .

The output of this code block, shown below, verifies our prediction of
the spectrum: Eigenvalues = \[-1. -1. -1. 3.\]

For the CTQW, the usual Hamiltonian is the adjacency matrix A. We modify
it slightly by adding the identity, i.e., we take H D A C I . This will
reduce the number of gates we need to apply, since the eigenvectors with
0 eigenvalue will not acquire a phase. The code below defines our
Hamiltonian: \# Get the Hamiltonian ham = A + np.eye(4)

It turns out that complete graphs are Hadamard diagonalizable. This
means that we can write H D QƒQ (9.66) where Q D H ˝ H and ƒ is the
diagonal matrix of eigenvalues. Let’s check that this works. \# Hadamard
gate hgate = np.sqrt(1/2) \* np.array(\[\[1, 1\], \[1, -1\]\]) \# Form
the matrix Q = H \otimes H to diagonalize the Hamiltonian Q =
np.kron(hgate, hgate) \# Print out the Q\^\dagger H Q to verify it’s
diagonal diag = Q.conj().T.dot(ham).dot(Q) print(diag)

199

SECTION 9.8 Quantum Walks

The output of this portion of the program, shown below, verifies that Q
HQ is indeed diagonal (note that numbers in the first row are
numerically zero): \[\[ \[ \[ \[

4.00000000e+00 0.00000000e+00 0.00000000e+00 0.00000000e+00

-4.93038066e-32 -4.93038066e-32 4.93038066e-32\] 0.00000000e+00
0.00000000e+00 0.00000000e+00\] 0.00000000e+00 0.00000000e+00
0.00000000e+00\] 0.00000000e+00 0.00000000e+00 0.00000000e+00\]\]

The time evolution operator U.t / D e same transformation. In
particular, we have 0 i 4t e B 0 Q e iH t Q D B @ 0 0

iH t

0 1 0 0

is also diagonalized by the

0 0 1 0

1 0 0C C 0A 1

(9.67)

which is exactly a CPHASE00 gate in pyQuil with an angle of 4t . To
elaborate on this further, the CPHASE00, which we’ll denote as C Z00 .'/
below, has the following action on the computational basis: C Z00
.'/j00i D e i' j00i C Z00 .'/j01i D j01i C Z00 .'/j10i D j10i C Z00
.'/j11i D j11i The circuit to simulate the unitary evolution U.t / D e
iH t thus consists of a Hadamard gate on each qubit, C Z00 . 4t /, and
then another Hadamard gate on each qubit. The code snippet below defines
a function for creating this quantum circuit: \# Function for a the
continuous time quantum walk circuit on a complete graph def
k\_4\_ctqw(t): """Returns a program implementing a continuous time
quantum walk.""" prog = pq.Program() \# Change to diagonal basis
prog.inst(H(0)) prog.inst(H(1)) \# Time evolve prog.inst(CPHASE00(-4\*t,
0, 1)) \# Change back to computational basis prog.inst(H(0))
prog.inst(H(1))

200

CHAPTER 9 Quantum Computing Methods

Figure 9.8: Time evolution of the continuous-time quantum and classical
walks on a complete graph with four vertices.

return prog

Let’s compare the quantum walk with a classical random walk. The
classical time evolution operator is e .M I /t where M is the stochastic
transition matrix of the graph. We obtain M from the adjacency matrix of
the graph below: \# Stochastic transition matrix for classical walk M =
A / np.sum(A, axis=0)

We choose as our initial condition j .0/i D j0i, so that the walker
starts on the first node. Therefore, due to symmetry, the probability of
occupying each of the nodes besides j0i is the same. In the code below,
we define the final times to simulate the random walks for and create
arrays to store the probability distributions at each final time: \# Set
up time to simulate for tmax = 4 steps = 40 time = np.linspace(0, tmax,
steps) \# Arrays to hold quantum probabilities and classical
probabilities at each time quantum\_probs = np.zeros((steps, tmax))
classical\_probs = np.zeros((steps, tmax))

SECTION 9.8 Quantum Walks

201

We can now simulate the continuous-time quantum and classical walks for
each final time we have chosen. The code block below performs this
simulation and stores the final probability distributions: \# Do the
classical and quantum continuous-time walks for i, t in enumerate(time):
\# Get a quantum program prog = k\_4\_ctqw(t) \# Simulate the circuit
and store the probabilities wvf = qvm.wavefunction(prog) vec =
wvf.amplitudes quantum\_probs\[i\] = np.abs(vec)\*\*2 \# Do the
classical continuous time walk classical\_ev = expm((M-np.eye(4))\*t)
classical\_probs\[i\] = classical\_ev\[:, 0\]

Finally, the code below plots the probabilities for each node at all
times: \_, (ax1, ax2) = plt.subplots(2, sharex=True, sharey=True)
ax1.set\_title("Quantum evolution") ax1.set\_ylabel("Probability")
ax1.plot(time, quantum\_probs\[:, 0\], label=’Initial node’)
ax1.plot(time, quantum\_probs\[:, 1\], label=’Remaining nodes’)
ax1.legend(loc=’center left’, bbox\_to\_anchor=(1, 0.5))
ax2.set\_title("Classical evolution") ax2.set\_xlabel(’t’)
ax2.set\_ylabel("Probability") ax2.plot(time, classical\_probs\[:, 0\],
label=’Initial node’) ax2.plot(time, classical\_probs\[:, 1\],
label=’Remaining nodes’)

The output of this code block is shown in Figure 9.8. Here, we see
another clear difference between the quantum and classical walks.
Namely, in the classical cases, the probability for being in the initial
node decays exponentially, whereas in the quantum case it oscillates!
This is what we should expect based on our construction of the
Hamiltonians for each case — namely, the quantum cases has an i in the
exponent e iH t which produces oscillatory behavior, while in the
classical case the exponent is real which produces purely exponential
decay.

202

9.9

CHAPTER 9 Quantum Computing Methods

Unification Framework for Quantum Algorithms (QSVT)

Researchers in the field have developed a common framework for the three
major groups of known quantum algorithms: factoring, simulation and
search. This approach is based on the quantum singular value transform
(QSVT) (see \[125\] and \[186\]). The QSVT model recognizes that many
different quantum algos can be represented as sequences of unitary
transforms and using this technique we can represent a range of quantum
algos with block-encoded matrices. As we can see in Figure 9.9, a number
of algorithms have been developed in each of the three main categories
of factoring, simulation and search. Various lines of inquiry in
different branches of quantum algos along with work on pulse sequences
for quantum computing on NMR platforms as well as quantum signal
processing led to the realization that algos across different categories
could all be built from common blocks (see \[170, 61, 306, 177, 125\]).
Chuang \[78\] provides a helpful framework for categorizing the core set
of quantum algos:  Category I: – Factoring \[254\] – Quantum Phase
Estimation \[152, 83\] – Linear Systems \[135\]  Category II: – Quantum
Simulation \[174\] – Quantum Walks \[74\] – Linear Combination of
Unitaries \[37\] – Quantum Signal Processing \[177\]  Category III –
Quantum Search \[130\] – Amplitude Amplification \[56, 57\] – Adiabatic
\[106\] – Fixed Point Amplitude Amplification \[306\] All of the above
algos can be represented in the QSVT framework. Since operators in
quantum computing can be represented as matrices, the goal of the QSVT
approach is to represent the matrix in question as a projected Q and …
to be orthogonal projectors and U to be unitary operator. Let’s take …

SECTION 9.10 Dequantization

Figure 9.9: Unification of quantum algorithms

203

Source: \[78\]

Q …. This encoding is a unitary; we then can encode the matrix A as A WD
…U Q termed symmetric if … D …. A special case of projected unitary
encoding of a quantum operator is Q D … D .j0ih0j/˝a ˝ I (see \[125\]).
In this block encoding where we have … case, A can be represented as the
upper left block of the unitary operator U , like so

˝a

A D h0j



˝a

˝ I U j0i

˝I





 A  () U D  

(9.68)

As in \[125\], we leave out the dimensions projected out by j0ih0j˝a for
convenience; in other words, A and U have different dimensions, unlike
in projected encodings. For further details on the QSVT model and how a
range of standard quantum algos can be built from these blocks, see
\[178, 125, 186\] and this book’s companion website.

9.10

Dequantization

Researchers have also realized that quantum algorithms that were once
thought to represent classical-quantum separation are not in fact
exponentially faster than their classical counterparts. This line of
work began with Tang \[273\] and her dequantization of a quantum algo
for recommendation systems \[151\]. Tang and others went on to
dequantize additional quantum ML algos. Note that when we refer to the
dequantization of a quantum algo, we are not necessarily saying that
this exact algo has no quantum-classical exponential separation, but
that we can identify a classical algo that accomplishes roughly the same

204

CHAPTER 9 Quantum Computing Methods

Figure 9.10: Sparsity-based QSVT and QRAM-based QSVT algos

Source: \[272\]

computational task as its quantum analogue and thus there is no
quantumclassical exponential separation. Often this classical algo is
quantum-inspired and we may not have developed it without first
considering its quantum analogue. Also note that the quantum analogue
may still provide a polynomial speedup in practice. In a talk on this
subject \[272\], Tang distinguishes between QML algos in the category of
QRAM-based QSVT which Tang states are generally subject to
dequantization and those in the category of sparsity-based QSVT which
are unlikely to be dequantized (see also the paper with Chia et al.
\[71\]. Quantum random access memory (QRAM) is a form of memory that can
store quantum states such as states of superposition (see \[126\] and
\[68\]). As we can see in Figure 9.10, examples of algos in the
QRAM-based QSVT category that have been dequantized include the quantum
versions of these algos:  Principal component analysis \[273\] 
Supervised clustering \[273\]  Support vector machines \[91\] 
Semidefinite programming \[72\]  Low-rank matrix decompositions \[272\]
Examples of algos in the sparsity-based QSVT category which are unlikely
to be dequantized include the quantum versions of these algos:  Sparse
linear programming \[135\]  Data fitting \[296\]  Electromagnetic
scattering \[82\]  Topological data analysis \[175\]  Gaussian process
regression \[308\]

SECTION 9.11 Summary

205

We expect to see additional developments in this area over the coming
years as we deepen our understanding of the common frameworks of
different quantum algorithms.

9.11

Summary

In this chapter, we have covered a range of quantum computing methods.
We have seen that a QC can be used for optimization, molecular
simulation, true random number generation and other techniques. For more
algorithms please see and contribute to the Quantum Algorithm Zoo
\[147\]. Also see \[183\] for an overview of several key quantum algos.
We have also covered the QSVT framework and developments in the
dequantization of quantum algos with classical analogues. In the coming
chapter we will turn to further developments in classical-quantum
separation, quantum error correction and the road ahead for quantum
computing.

As the quantum community eagerly seizes the impending opportunity to
experiment with NISQ devices, we must not lose sight of the essential
longer-term goal: hastening the onset of the fault-tolerant era. —John
Preskill

CHAPTER

10

Applications and Quantum Supremacy In this work, we have taken a journey
through the quantum computing landscape; we have explored its
theoretical foundation, discussed the key research and milestones that
advanced the field and covered a range of hardware approaches and
quantum computing methods. On the engineering front, there are still
daunting challenges ahead of us to scale to more than 106 qubits. Once
we achieve fault-tolerant quantum computing, more possibilities open up
for applications. In the current NISQ regime, there is plenty of work to
be done to explore test cases and prepare for the error-corrected
machines.

10.1

Applications

As the quantum computing landscape evolves, a number of QC applications
are becoming clear. Check the online site and see \[199\] and \[224\]
for updates on QC applications.

Quantum Simulation and Chemistry High-performance classical computers
are used today to model new molecular combinations. This work helps
researchers develop new materials, novel pharmaceuticals as well as
compounds for other applications. Quantum computers will likely give us
new capabilities in this domain. Already, the VQE and quantum chemistry
simulation methods discussed in chapter 9 have shown promising results.
See the following for additional examples: \[234, 293, 210\]. See also
\[21\] for work on simulating an SYK model through asymmetric
qubitization for an example of a physics simulation.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_10

207

208

CHAPTER 10 Applications and Quantum Supremacy

Sampling from Probability Distributions We use distribution sampling in
many applications such as pattern recognition and probabilistic
inference. With a quantum computer, we can sample from a much larger
distribution. This is one reason that distribution sampling is being
used to demonstrate quantum supremacy as we describe later in this
chapter.

Linear Algebra Speedup with Quantum Computers There are many application
of linear algebra in industry. Matrix inversion, is a common technique
that can be used, for example, in computing electromagnetic patterns to
design an antenna \[224\]. The HHL technique which we covered in chapter
9 is one method that may prove valuable for these applications.

Optimization There are numerous optimization applications in industry,
including: delivery truck routing, online ad bidding strategies and
mixtures of different chemicals for electric vehicle battery
composition. It is becoming clear that quantum computers can be used to
optimize these kinds of systems.

Tensor Networks One promising area of inquiry is the application of
quantum computation to tensor networks (TNs). This book’s online site
contains references to a number of good introductions to TNs. Various
tensor network architectures such as MERA, MPS, TTNs and PEPS are
proving to be useful tools to explore questions in physics as well as in
other fields such as deep learning networks. Several groups have
demonstrated a range of applications of tensor networks \[284, 295, 247,
285, 140, 196, 240, 195, 124, 289\].

10.2

Quantum Supremacy

The term quantum supremacy, first coined by Preskill in 2012, refers to
a computational task that can be efficiently performed on a quantum
computer beyond the capabilities of state-of-the-art classical
supercomputer can efficiently implement \[223\]. We note immediately —
as the strong term

SECTION 10.2 Quantum Supremacy

209

supremacy can generate confusion — that this refers to any computational
task which meets the criteria, not necessarily a task that is useful.
The algorithm used to demonstrate supremacy does not need to have wide
application, just a clear-cut ability to run efficiently on a quantum
processor compared with a classical computer where the algorithm is
intractable. \[45\]. In this section, we discuss problems which
researchers are considering to demonstrate quantum supremacy. Regardless
of the particular problem used for the demonstration, quantum supremacy
is a landmark achievement in the history of physics and computer
science. While many proof-of-principle quantum computations have been
performed on quantum processors, this will be the first to be executed
at a large enough scale to reveal an experimentally verifiable
computational separation. This has implications for verifying quantum
mechanics through largescale computation. Indeed, we can think of
supremacy experiments as the computational analogue of Bell experiments
\[136\]. Just as Bell experiments refute local hidden variable models,
supremacy experiments on a QC have now refuted the Extended
Church-Turing Thesis (ECTT) which, as discussed in chapter 4, asserts
that any algorithmic process can be simulated efficiently using a
probabilistic Turing machine PTM. This then leads us to the Quantum
Extended Church-Turing Thesis (QECTT). The ability to carefully control
quantum systems in this manner is a crowning achievement of engineering
and experimental physics. In the remainder of the section, we discuss
the some of the computational tasks used in demonstrating quantum
supremacy. We will begin with random circuit sampling which was used in
the paper by Arute, et al. \[19\]. See also \[302\] for a subsequent
implementation of random circuit sampling for demonstration of quantum
supremacy and see \[201\] for a guide to random circuit sampling.

Random Circuit Sampling Sampling from the output distribution of a
quantum circuit is one of the most natural problems to demonstrate
quantum supremacy. To simulate this on a classical computer, one must
perform the linear algebra and matrix computation to determine the final
state of the wavefunction after the execution of the quantum circuit
(written as tensor products of unitary operators). However, a quantum
computer naturally performs this calculation by simply evolving in time
under the physical realizations of the unitary operators. Classical
methods for simulating quantum circuits generally scale exponentially in
the number of qubits. Specifically, for the most general, fully

210

CHAPTER 10 Applications and Quantum Supremacy

Name Kilobyte (KB) Megabyte (MB) Gigabyte (GB) Terabyte (TB) Petabyte
(PB) Exabyte (EB) Zettabyte (ZB)

Number of bytes 210  103 220  106 230  109 240  1012 250  1015 260
 1018 270  1021

Number of qubits nD6 n D 16 n D 26 n D 36 n D 46 n D 56 n D 66

Table 10.1: Table of prefixes and the number of bytes they correspond
to; the last column shows the maximum number of qubits that can be
stored for the given memory, assuming the most general state of a qubit
with amplitudes stored in double precision. One byte is 8 bits.

entangled, state of n qubits, there are 2n complex amplitudes to keep
track of in the wavefunction. Even for moderate values of n, this
quickly reaches current memory limitations on even the most capable
supercomputers. Each amplitude in the wavefunction is generally a
complex number, which entails storing two real floating-point numbers
per amplitude. Suppose that these floating-point numbers are stored in
double precision format, i.e., 8 bytes per floating-point number. Under
these assumptions, the total memory required to store the wavefunction
is 2n amplitudes  2 real numbers/amplitude  23 bytes/real number i.e.,
2nC4 bytes. Recall that one kilobyte is defined as 210 bytes, one
megabyte is 220 bytes, and so on; see Table 10.1. The leading
supercomputers have RAM sizes of petabytes to exabytes.1 Based on our
previous argument for memory requirements of storing wavefunctions, we
can estimate the upper range of quantum circuit simulation for any
particular classical system. This is the fundamental idea of using
quantum circuit sampling as a candidate problem for demonstrating
quantum supremacy \[52, 200\]. There are now multiple methods for
simulating quantum circuits — ranging from explicit construction of the
unitary for the circuit to tensor network contractions — but all of them
suffer from exponential complexity in the number of qubits. Let us now
consider in more detail random circuit sampling as a demonstration
problem of quantum supremacy, following the work of Boixo et al. \[19,
205, 45, 184\]. Here researchers are focused on the computational task
of sampling from the output distribution of random quantum circuits. 1
See

https://www.top500.org/ for an up-to-date list of supercomputers and
their specs.

SECTION 10.2 Quantum Supremacy

211

The particular random circuits considered for supremacy experiments are
constructed via the following rules \[19, 45\]:2 1. Start with a
Hadamard gate on each qubit. 2. Apply controlled-Z (CZ) operators
between neighboring qubits in a twodimensional grid alternating between
horizontal and vertical patterns. Note that in any particular cycle, not
all neighboring qubits will be connected via a CZ, and the number of CZ
gates can be different in different cycles.3 3. Apply single-qubit
operators from the set fX 1=2 ; Y 1=2 ; T g to the qubits which are not
affected by CZ gates according to the following criteria:  If the
previous cycle had a CZ gate on a given qubit, apply a randomly-chosen
non-diagonal unary gate to that qubit if possible.4  If the previous
cycle had a non-diagonal unary gate on a given qubit, apply a T gate to
that qubit if possible.  Apply a T gate to a qubit if there are no
unary gates in the previous cycles on that qubit (except for the initial
Hadamard gate). Note that this rule is an if and not iff. That is, a T
gate may follow another unary gate; the rule simply states that if there
is no unary gate on that qubit in the previous cycles, then we must
place a T gate in the current cycle. The previous two criteria take
precedence over this one.  If none of the above criteria are satisfied
for a given qubit, then a unary gate is not applied to that qubit for
the current cycle. 4. Repeat steps (2) and (3) for a given number of
cycles (which determines the depth). 5. Measure in the computational or
Hadamard (X ) basis. We can now incorporate these rules into a program
for building supremacy circuits. An example program in Cirq
demonstrating this functionality is provided below. import cirq \#
Number of rows in grid of qubits 2 Note that we have incorporated
Boixo’s updated instructions from his GitHub site:
https://github.com/sboixo/GRCS 3 Note that the term cycle in this
context refers to moments in the framework of Cirq. We can think of
cycles or moments as the set of operators that are applied
simultaneously. 4 “If possible" means if the circuit has not ended or if
there is not a CZ gate on that qubit in the current cycle.

212

CHAPTER 10 Applications and Quantum Supremacy

nrows = 4 \# Number of columns in grid of qubits ncols = 4 \# Depth of
CZ gates in supremacy circuit depth = 5 \# Generate the supremacy
circuit supremacy\_circuit =
cirq.experiments.generate\_supremacy\_circuit\_google\_v2\_grid( nrows,
ncols, depth, seed=123) print(supremacy\_circuit)

Here, the number of rows and number of columns are specified for the
twodimensional grid of qubits; the depth, or number of cycles of CZ
gates, is specified to determine the overall depth of the supremacy
circuit. The output of this program is shown in Figure 10.1. Note that
in any particular version or implementation of a random circuit sampler,
the code module may be following rules that are slightly modified from
those stated above. This circuit of n D 16 qubits is easily handled by
classical computers, but, as we have argued, the difficulty of classical
simulation scales exponentially in n. For a sufficiently large number of
qubits n, we outline the steps toward demonstrating quantum supremacy
\[45\]: 1. Generate a supremacy circuit U on n qubits and a given depth
d as per above. 2. Sample from the circuit m times with m  103 106 to
get an output distribution fx1 ; :::; xm g. 3. Compute log 1=pU .xj /
for each j D 1; :::; m with a sufficiently powerful classical computer.
Here, pU .xj / WD jhxj j ij2

(10.1)

where j i D U j0i is the final state of the supremacy circuit. 4.
Compute the quantity m

˛ D H0

1 X 1 log m pU .xj /

(10.2)

1

log.2n /

where H0 D C is the cross-entropy of an algorithm which samples from bit
strings uniformly. (Note that the logarithm is the natural logarithm
here.) Here,  0:577 is Euler’s constant. Once the quantity ˛ is
computed, it is then compared to a similar quantity evaluated on the
output distribution pA of the best classical algorithm A for

SECTION 10.2 Quantum Supremacy

213

Figure 10.1: Quantum supremacy circuit on a grid of qubits generated by
Cirq. The final cycle of Hadamard gates is for measuring in the X basis,
but Z basis measurements may be used as well.

simulating quantum circuits. Note that the cross-entropy difference,
which gives a measure of how well the algorithm A can predict the
outcome of a typical random circuit U , is given by H.pA / D H0

H.pA ; pU /

(10.3)

Now consider the expectation value of H.pA / over an ensemble of random
circuits R and let C hold this value: C WD ER ŒH.pA /

(10.4)

In the Boixo et al. supremacy paper \[45\], it is shown that quantum
advantage is achieved in practice when C ˛1

(10.5)

Note that C ! 0 for large enough circuits, and further that pU .xj / can
no longer be obtained numerically. This implies by definition that the
quantity

214

CHAPTER 10 Applications and Quantum Supremacy

˛ can no longer be measured directly. However, it is possible to
extrapolate ˛ for larger circuits in order to demonstrate quantum
supremacy with random circuit sampling.

Other Problems for Demonstrating Quantum Supremacy While random circuit
sampling is a very natural problem to consider for demonstrating quantum
supremacy, it is not the only one. A survey paper by Harrow and
Montanaro \[136\] provides a helpful discussion of additional major
problems being considered to show quantum-classical separation. The
problem of boson sampling is another candidate for demonstrating quantum
supremacy. Originally proposed in \[5\], boson sampling involves sending
n coincident photons into a randomly generated linear-optical network of
m  n modes (beam splitters); this generates a random unitary rotation.
Detectors are then used to sample from the distribution of photons, a
process which is believed to be classically hard. Boson sampling
experiments have been performed with up to five photons and nine modes
\[263\]. Experimental systems are challenged by non-trivial photon loss
in the optical network. Additionally, developing more efficient
classical sampling techniques is a challenge for quantum supremacy via
boson sampling.5

Quantum Advantage and Beyond Classical Computation Researchers have
coined several terms related to the distinction between classical and
quantum computing, including quantum advantage, beyond classical
computation and quantum-classical separation. The field now recognizes
the following distinctions:  Quantum supremacy: a computational task
which is proven to have superpolynomial separation between classical and
quantum platforms, but is not necessarily a useful task. The random
circuit sampling task is an example (note that recently some have
suggested possible practical uses for random circuit sampling). 
Quantum advantage: a computational task which is useful and has a proven
superpolynomial separation between classical and quantum platforms. See
W. Zeng’s article on terms and measures of quantum-classical computing
distinctions \[307\]. 5 This

is true for any problem, P , used for quantum supremacy. Namely, if
better classical algorithms are developed for P , the threshold for
quantum supremacy with P gets pushed back further.

SECTION 10.3 Quantum Error Correction

Figure 10.2: Quantum computing roadmap

10.3

215

Source: Google

Quantum Error Correction

Context and Importance While today’s quantum computers do not yet have
sufficient qubits to support full quantum error correction (QEC), there
is a growing body of research on QEC with implications for both QC and
beyond. Classical computation admits straightforward error correction
through the replication of a state across many classical bits. The
no-cloning theorem in quantum mechanics, however, prevents us from
taking this direct approach in a quantum computer. A typical approach to
QEC involves a surface code which encodes one logical qubit into a
topological state of several physical qubits \[60, 86, 116\]. When we
measure these physical qubits we can see a pattern called a syndrome
which is the result of a particular sequence of errors; a decoder can
then map the syndrome to a particular error sequence. Such decoding may
be amenable to the use of machine learning (see, for example, \[24\]).
As discussed in the section on VQE, McClean et al. have explored the use
of subspace expansion for error mitigation \[190\]. See the work of Ofek
et al. for a discussion of the break-even point of QEC \[209\]). Error
correction schemes have also emerged from other branches of physics;
several researchers have been investigating QEC approaches that derive
from the duality framework of Anti-de Sitter/Conformal Field Theory
(AdS/CFT) \[15\]. QEC remains an active area of research and is critical
in the scaling quantum computing hardware devices. A complete treatment
of quantum error correction and fault tolerance is the subject of an
entire book itself. In the remainder of this section, we provide a

216

CHAPTER 10 Applications and Quantum Supremacy

pedagogical introduction to the essential elements of quantum error
correction. By mastering this material, you will be well-prepared to
take on dedicated books on the topic and being reading research or
review articles.

Important Preliminaries One of the most important facets of quantum
error correction concerns discrete vs. continuous errors. Consider a
single-qubit state j i D ˛j0i C ˇj1i:

(10.6)

As we have argued previously, there are many more operations one can do
on a qubit compared to a classical bit. This also means that there are
more errors that can occur on a qubit! Concretely, the primary classical
error is a bit-flip error.6 The quantum analogue of this is of course a
Pauli-X error, also loosely called a bit-flip error for obvious reasons:
Xj0i D j1i and X j1i D j0i. However, in the quantum case there is also
the phase-flip error ZjCi D j i and Zj i D jCi, and the combined bit-
and phase-flip error Y D iXZ. The Pauli operators (including identity)
form a basis for 2  2 matrices, so any error E can be written E WD e0 I
C e1 X C e2 Y C e3 Z D e0 0 C e1 1 C e2 2 C e3 3

(10.7)

for complex coefficients e0 ; : : : ; e3 . We note that these
coefficients are continuous and can be in principle infinitesimally
small. How can we hope to correct such continuous, potentially
infinitesimally small errors? The answer is measurements. Suppose the
error E occurs on our qubit j i, leaving us with a superposition of
possible Pauli errors. If we measure an appropriate property of the
state, we collapse the superposition7 into a state with one discrete
error. For concreteness, we can choose our measurement so that j i with
error E 7! i i j i (10.8) upon measurement for some i . Here i is
the i th Pauli operator and i is a complex coefficient. Note the
crucial fact that i can still be continuous but is now irrelevant
because it is a global phase. In this sense, measurement maps a
continuous error E to a discrete error i j i where i 2 f0; 1; 2; 3g. 6
This

is not the only error, however. Another classical error is erasure in
which 0 7! 0 and 1 7! 0. 7 Depending on your favorite interpretation of
quantum mechanics, there are different ways to say this statement, but
they are all mathematically identical here.

SECTION 10.3 Quantum Error Correction

217

The discrete error state i j i is easy to correct as long as we know
what i is. If so, we simply apply the inverse operation, which here
happens to be just i since Pauli operators square to identity. For
example, suppose we measure and find the state to be i j i D Xj i,
i.e., a bit-flip error has occurred. Then, we simply apply the X
operator to get back the original, error-free state j i D XXj i. The
previous discussion highlights some important facts and major ideas in
quantum error correction. In the language of the field, we say we
perform stabilizer measurements and obtain a syndrome. The syndrome
tells us what correction operators to apply to the state to return back
to the original error free state. You may be wondering: Measurement
seems useful to map continuous errors to discrete errors, but doesn’t it
destroy the information in the state? How can we hope to perform
computations if we repeatedly measure? The answer to these questions is
that we encode information in a logical qubit and perform
non-destructive measurements. The following example seeks to introduce
and define these concepts.

Motivating Example: The Repetition Code Error correction has a long
history in classical information theory, and it is helpful to draw on
its ideas. The simplest classical error correcting code is the
repetition code in which 0 7! 000

and

1 7! 111

(10.9)

That is, rather than a single physical bit, we make three copies of it
and form what we call a logical bit. We treat the logical bit as one
unit of information, even though we know it is composed of three
physical bits. The repetition code is very intuitive and occurs in
everyday conversation: if Bob doesn’t hear Alice, he may ask her to
repeat herself. By hearing the phrase more than once, Bob can use the
multiple “copies” of the message to reconstruct her meaning. The idea
with bits is the same. Instead of sending just one physical bit 0 to
Bob, Alice sends the logical bit 000. An error may occur on any of the
physical bits in the logical bit. When Bob receives the message, he
takes a majority vote — i.e., if there are more 0s than 1s, he
interprets the message as 0, and vice versa — and takes this as the
intended message. Note that if Alice sends 000 and two bits flip, for
example Bob receives 101, then the majority vote yields 1 as the
message, which is incorrect. So, there is a logical error in the
repetition code when two or more physical bits flip.

218

CHAPTER 10 Applications and Quantum Supremacy

Suppose each physical bit flips independently with probability p. The
probability of a logical error, pe , is then pe D 3p 2 .1

p/ C p 3 D 3p 2

2p 3 :

(10.10)

The first term 3p 2 .1 p/ is the probability that any two bits flip, and
the second term p 3 is the probability that all three bits flip. We have
an advantage using the repetition code when pe &lt; p, which occurs when
p &lt; 1=2. (This value is found by solving the inequality p &lt; 3p 2
2p 3 .) This example illustrates several concepts used in quantum error
correction: (i) redundantly using multiple physical (qu)bits to form a
logical (qu)bit, and (ii) physical errors vs. logical errors. Let’s see
how these concepts transfer concretely with the quantum version of the
repetition code. As stated earlier, the no-cloning theorem states that
there does not exist a unitary operation which can make multiple copies
of an arbitrary state. So, we cannot simply make three copies of a
physical qubit j i D ˛j0i C ˇj1i to j ij ij i as our logical qubit.
However, the basis states j0i and j1i are orthogonal, and so we can make
copies of them. In particular, we can map j i WD ˛j0i C ˇj1i 7! j N i WD
˛j000i C ˇj111i:

(10.11)

Note that we use the common notation j N i to indicate a logical qubit
instead of a physical qubit. Just like the classical repetition code,
there are three physical qubits in the state j N i WD ˛j000i C ˇj111i,
but we treat this as one unit of quantum information, and so call it a
logical qubit. Formally, a logical qubit is a simply two-dimensional
subspace of a larger (physical) Hilbert space. In this example, the
physical Hilbert space is the space of three physical qubits C2 ˝ C2 ˝
C2 ' C8 , and the logical qubit is the subspace spanned by j000i and
j111i. The basis vectors of a logical subspace are also known as
codewords. As we have seen in the classical repetition code, we are able
to correct errors that occur on one or fewer physical bits. The same
will be true in the quantum case. However, we cannot simply “peek” at
the state to take a majority vote. What we instead do is measure
particular operators which tell us which physical qubit has flipped.
There are four correctable errors which can occur: no physical qubit has
flipped, the first physical qubit has flipped, the second physical qubit
has flipped, or the third physical qubit has flipped. To determine which
error has occurred, we measure the projection operators in Table 10.2.
To understand these operators, suppose a bit-flip error occurred on the
second qubit. This means that our logical qubit is j N e i D Xj N i D
˛j010i C ˇj101i. It is not hard to see that the following holds:

SECTION 10.3 Quantum Error Correction

P0 P1 P2 P3

Operator D j000ih000j C j111ih111j D j100ih100j C j011ih011j D
j010ih010j C j101ih101j D j001ih001j C j110ih110j

219

Syndrome No qubit has flipped The first qubit flipped The second qubit
flipped The third qubit flipped

Table 10.2: Projection operators for the three-qubit repetition code.

h N e jP0 j N e i D 0; h N e jP1 j N e i D 0;

(10.12)

h N e jP2 j N e i D 1;

(10.14)

h N e jP3 j N e i D 0

(10.15)

(10.13)

In words, we measure P2 with probability 1. In the previous example, we
started with the error state and realized what operator we would
measure. In practice we of course do not know the error state, but we
perform the same procedure. Namely, we implement a circuit which
measures P0 , ..., P3 and end up with a syndrome. The syndrome tells us
either no bit has flipped, the first bit has flipped, etc. After this,
we apply the appropriate correction operator. For example, if the
syndrome was that the second bit flipped, we would apply Pauli-X to the
second physical qubit. Analyzing when the quantum repetition code is
advantageous to implement is analogous to analyzing when the classical
repetition code is advantageous to use from above. We assume qubits flip
independently with probability p and again we have advantage in using
the repetition code when p &lt; 1=2. A difference in the quantum case is
that bit-flip errors are not the only errors that can occur! While the
three-qubit repetition code can correct single-qubit bit-flip errors, it
cannot correct arbitrary single-qubit errors. For example, phase-flip
errors are undetectable by this code.8 The first quantum error
correcting code to correct arbitrary single-qubit errors was Shor’s
9-qubit code, which actually concatenates two three-qubit repetition
codes.

The Stabilizer Formalism In the previous sections, we have seen
important elements of error correction. We now introduce the standard
language for talking about codes, namely the stabilizer formalism, which
was introduced by Gottesman in his PhD 8 It is easy to modify the
repetition code to correct for phase-flip errors instead of bit-flip
errors, but we skip this presentation for brevity. The key insight is
that bit-flip and phase-flip errors are related by Z D HXH where H is
the Hadamard gate.

220

CHAPTER 10 Applications and Quantum Supremacy

thesis \[128\]. The stabilizer formalism leans heavily on group theory
(see chapter 12 for background/review) and may seem cumbersome at first,
but it is the de facto standard because it is such a powerful framework.
n n n We say that a state j i 2 C2 is stabilized by operator S 2 C2 2
if S j i D j i. (In other words, if j i is a +1 eigenvector of S .) The
set of all such operators is known as the stabilizer of j i. The
stabilizer is sometimes referred to as the stabilizer group for reasons
we will see shortly, and its elements are referred to as stabilizer
elements. We will use the notation S to represent a stabilizer group.
What does this have to do with error correcting codes? Previously, we
specified a code by its codewords, e.g. j N i D ˛j000i C ˇj111i for the
three-qubit repetition code. In the stabilizer formalism, we specify a
code by its stabilizer group. There is a one-to-one mapping between the
two. The stabilizer group is the set of all operators S such that S j i
D j i for each codeword j i. As an example, the stabilizer group for the
three-qubit repetition code is S D fI; Z1 Z2 ; Z1 Z3 ; Z2 Z3 g. You are
encouraged to check that S j000i D j000i and Sj111i D j111i for each S 2
S. In this simple example, specifying the stabilizer group instead of
codewords does not seem to provide much advantage, but for larger,
non-trivial codes the utility is unquestionable. Now that we have
motivated stabilizers and connected them to our previous understanding
of quantum error correcting codes, let us introduce them formally. The
Pauli group on n qubits is defined as Pn WD fp1 ˝    ˝ n W p 2 f˙i;
˙1g and i 2 fI; X; Y; Zg 8i 2 Œng: (10.16) That is, Pn is n-fold
products of Pauli operators with a phase p. One can show that Pn is a
group, and we encourage the reader to try this exercise. We now define a
stabilizer group as an abelian subgroup of Pn which does not contain I .
Why do we require these two conditions? Remember that we care about the
stabilizer group for the purpose of defining quantum error correcting
codes — the codewords j i are the states such that S j i D j i for all
stabilizer elements S . Suppose that I was a stabilizer element. Then,
any codeword must satisfy I j i D j i, which immediately gives us a
trivial code j i D 0! This explains why we require that I 62 S. What
about the second condition, that S is abelian? Suppose that that S is
non-abelian. Recall that Pauli operators either commute or anti-commute.
Let S1 ; S2 2 S such that S1 S2 D S2 S1 . Then, S1 S2 j i D

S2 S1 j i H) j i D

j i:

(10.17)

SECTION 10.3 Quantum Error Correction

221

The implication follows by definition of a stabilizer: i.e., S1 j i D j
i and S2 j i D j i. Thus we again arrive at a trivial codespace. So, the
conditions that S be abelian and I 62 S ensure the codespace of the
stabilizer is non-trivial. We now introduce the concept of stabilizer
generators. In a previous example, we stated that the stabilizer group
of the three-qubit repetition code is S D fI; Z1 Z2 ; Z1 Z3 ; Z2 Z3g. We
would like to write out the group as succinctly as possible, rather than
list all elements explicitly. To this end, we write S D hZ1 Z2 ; Z2 Z3
i. Here, the elements Z1 Z2 and Z2 Z3 are generators and the notation
hi means “the set generated by all possible products” of generators. We
can generate the the stabilizer elements from these generators as
follows: the identity I is either generator squared, Z1 Z2 is the first
generator, Z1 Z3 is the product of both generators, and Z2 Z3 is the
second generator. Generating sets are not unique. We invite the reader
to verify that hZ1 Z3 ; Z2 Z3 i D fI; Z1 Z2 ; Z1 Z3 ; Z2 Z3g

(10.18)

as well. Notice that for the three-qubit repetition, regardless of which
generators we pick, there are always two of them. Is it a coincidence
that two stabilizer generators defined on three physical qubits leads to
one logical qubit? It is not! One can show that an n-qubit code with k
stabilizer generators has n k logical qubits. The ratio k=n is known as
the rate of the code. We defer the proof of this theorem to other texts
and instead continue to emphasize the concepts through examples. Let us
now see another quantum error correcting code which we will specify
using the stabilizer formalism. The five-qubit code has stabilizer
generators listed below: S1 D XZZXI S2 D IXZZX S3 D XIXZZ S4 D ZXIXZ
Each generator acts on five qubits, so n D 5, and there are k D 4
stabilizer generators. Thus we know that this code defines n k D 1
logical qubit. We invite the reader to verify that S WD hS1 ; S2 ; S3 ;
S4 i is indeed abelian. The five-qubit code can correct arbitrary errors
on any physical qubit. One can show that five is the smallest number of
physical qubits needed in order to correct arbitrary single-qubit
errors, so in this sense the code is optimal.

222

CHAPTER 10 Applications and Quantum Supremacy

So far we have been concerned with how to store information in logical
qubits, but how do we process this information to perform computations?
Similar to how we perform physical operations on physical qubits, we
perform logical operations on logical qubits. Consider the three-qubit
repetition N D j000i. Suppose we want to perform a logical bit-flip code
which has j0i operation XN on this logical qubit. We can do this by
applying X to each physical qubit since N XXXj000i D j111i DW j1i

(10.19)

Thus, the logical operation is XN D XXX . We invite the reader to verify
that we can take the logical phase-flip operation as ZN D ZZZ. We
reasoned above by thinking about actions on codewords — how do we treat
logical operations in the stabilizer formalism? The key is to think
about commutation relations of operators. For physical Pauli operators,
we have fX; Zg D 0 where f; g denotes the anti-commutator. The logical
operations should also obey this rule. We encourage the reader to check
that this is true N D fXXX; ZZZg D 0. This for the three-qubit
repetition code, i.e., fXN ; Zg is only half of the story, however: we
also need logical operations to commute with each stabilizer generator.
The reason for this is by construction — we will soon see that
correctable errors anti-commute with stabilizer generators. So requiring
logical operations to commute with stabilizer generators means that they
are not errors. Continuing with the guiding example of the three-qubit N
S  D 0 for repetition code, we invite the reader to verify that ŒXN ; S
 D ŒZ; each S 2 hZ1 Z2 ; Z2 Z3 i. Back to the five-qubit code, this
provides us with a way to find logical operations without ever knowing
what the codewords are. Namely, we need N D 0 and ŒXN ; S  D ŒZ; N S D
0 to find operations XN and ZN such that fXN ; Zg 9 N for each S 2 S.
Can you find such operators? One choice is X D XXXXX and ZN D ZZZZZ. We
encourage you to verify that these operators satisfy the previously
stated conditions. If you try to analyze these operators on the
codewords of the five-qubit code, listed below for reference, you will
immediately appreciate the advantage of the stabilizer formalism! N D 1
Œj0000i C j10010i C j01001i C j10100i j0i 4 C j01010i j11011i j00110i
j11000i

9 Note

j11101i

j00011i

j11110i

j01111i

j10001i

j01100i

j10111i C j00101i

that the choice of logical operators is generally not unique.

SECTION 10.3 Quantum Error Correction

223

N D 1 Œj1111i C j01101i C j10110i C j01011i j1i 4 C j10101i j00100i
j11001i j00111i j00010i

j11100i

j00001i

j10000i

j01110i

j10011i

j01000i C j11010i

We now have two main pieces of the puzzle: stabilizer generators and
logical operations. What about errors? How do we know which errors a
given code can correct? The answer comes in the following theorem, known
as the Knill-Laflamme conditions: Given a stabilizer code S, set of
errors fEj g is  correctable if Ej Ek 62 N .S/ S for all j and k. Here
N .S/ denotes the normalizer of S in Pn , i.e., the set of all P 2 Pn
such that PSP  2 S for all S 2 S. The proof of this theorem is also
outside the scope of our treatment here but can be found in standard
textbooks on quantum error correction. To complete the discussion on
errors and the last major piece of the puzzle, we introduce the
important concept of code distance. So far, we have seen the three-qubit
repetition code and the five-qubit code, and described them by the
number of physical qubits n and the number of logical qubits k. The
former can only correct single-qubit bit-flip errors, but the latter can
correct arbitrary single-qubit errors. This difference, not captured in
n and k, is the purpose of defining and stating the distance d of a
code. The distance d is defined as the minimum weight error (element) in
N .S/ S, where the weight of a Pauli string is the number of
non-identity terms. For example, the weight of XXI is two. Intuitively,
the larger the distance of a code, the more errors it can correct.
Specifically, a code with distance d D 2t C 1 can correct errors with
weight less than or equal to t. Now that we have defined distance, we
can introduce the standard notation for codes, which is ŒŒn; k; d ,
and use it to summarize the concepts we have seen so far.10 First, we
have motivated and defined the difference between physical qubits and
logical qubits. The number of physical qubits in an ŒŒn; k; d  code is
n, and the number of logical qubits is k. The rate of a code is k=n. We
introduced the stabilizer formalism and saw that the number of
stabilizer generators is n k. For each of the k logical qubits, we
define logical operators XN 1 ; ZN 1 ; :::; XN k ; ZN k which satisfy
fXN i ; ZN i g D 0 for all i and ŒXN i ; ZN j  D 0 for all i ¤ j , and
further that ŒXN i ; S  D ŒZN i ; S  D 0 for each 10 Note

that classical codes are presented with a single square bracket and
quantum codes with two square brackets by convention.

224

CHAPTER 10 Applications and Quantum Supremacy

i 2 Œk and S 2 S. A distance d D 2t C 1 code can correct errors with
weight less than or equal to t. This exposition reveals only the
fundamental concepts of the rich field of quantum error correction.
Further topics include the threshold theorem, magic state distillation
(or simply distillation) and fault tolerance, as well as different
classes of error correction codes. For more on these advanced topics,
see \[62\]. We hope this introductory section will help you delve
further into the field and perhaps develop the new leading quantum error
correction code in the future.

10.4

Doing Physics with Quantum Computers

As we mentioned in the preface of this book, one of the most interesting
potential uses of quantum computers is to probe open questions in
physics. The duality framework of AdS/CFT gives us an initial mapping
between general relativity and quantum mechanics. Susskind and others
have speculated on the use of quantum computers to explore this duality
\[268\]. While we are years away from building QCs of sufficient scale
to run such experiments, it is still useful to consider what we might
learn from such explorations. The key principle here is that in quantum
computing we are not merely modeling a superposition or entangled state
and pointing to it from a classical computer; we are in fact
implementing these states, and as such can ask questions about their
dynamics. See also \[21\] for work on simulating an SYK model through
asymmetric qubitization.

Conclusion We anticipate a fast pace of development in this field — both
in hardware and software — and predict that many more universities and
companies will explore how these platforms can impact their work. We
invite the reader to access the book’s online companion site
http://www.github.com/jackhidary/quantumcomputingbook

for more resources and updates as the field progresses. As we drive to a
fully error-corrected quantum computer, it will certainly be an
interesting journey.

Part III

Toolkit

“To those who do not know mathematics it is difficult to get across a
real feeling as to the beauty, the deepest beauty, of nature ... If you
want to learn about nature, to appreciate nature, it is necessary to
understand the language that she speaks in.” —Richard Feynman

CHAPTER

11

Mathematical Tools for Quantum Computing I 11.1

Introduction and Self-Test

One of the most important discoveries of quantum mechanics in the
twentieth century was the observation by John von Neumann in his
Mathematical Foundations of Quantum Mechanics that all of quantum
mechanics can be described by linear algebra \[286\]. Confident readers
may feel that they need not read this chapter and might instead flip
through it for formulas, equations and the like. We provide readers with
the following provocative questions whose answers we will provide
directly afterward. Exercise Self-Test 1. Is the function

11.1

T WR!R T .x/ WD x C 1 a linear transformation? 2. Does a binary
operation have anything to do with binary code? 3. Which space has a
bigger dimension: R4 or C2 ? 4. Of these expressions: a. h0j1i b. j0ih1j
c. h0j1i j0i © The Author(s), under exclusive license to Springer Nature
Switzerland AG 2021 J. D. Hidary, Quantum Computing: An Applied
Approach, https://doi.org/10.1007/978-3-030-83274-2\_11

227

228

CHAPTER 11 Mathematical Tools for Quantum Computing I

d.  hi jAjj i where A is a matrix and i and j are numbers Which is a
    number? A vector? A matrix?

<!-- -->

5.  Give an example of a Hermitian operator whose eigenvalues are not
    real numbers. The answers:
6.  No, it’s hopelessly not linear.
7.  No, a binary operation is a special type of function.
8.  R4 and C2 have the same dimension over R.
9.  Here is the classification of the four expressions in Dirac
    notation:

<!-- -->

a.  The expression h0j1i is a number. In fact, h0j1i D 0.
b.  The expression j0ih1j is a matrix, specifically, the matrix   1 0
    0 0
c.  The expression h0j1i j0i is a vector. You can see that h0j1i is the
    number 0 and we mentioned earlier in the book that j0i is the vector
      1 j0i WD 0 so we can write  h0j1i j0i D .h0j1i/ j0i D .0/ j0i D
    .0/  D

01 00



 D

0 0

1 0





d.  This is a number. In particular, it’s a clever way to write the
    entry in the i th row and j th column of the matrix A.

<!-- -->

5.  There is no such thing! Hermitian operators always have real
    eigenvalues; try to prove this statement – we will in this section.
    Linear algebra can become very complicated. We don’t want to
    discourage you, rather the opposite! We would like to be your
    ambassadors on a journey into linear algebra and the supporting
    abstract mathematics that underlies quantum computing. We will
    develop all of the prerequisite mathematics and offer several
    examples from the book to relate the tools of linear algebra to
    quantum computing. That being said, feel free to begin wherever it
    is that you feel comfortable.

SECTION 11.2 Linear Algebra

229

2  2

1 2



 2

1 2



1 1

1

(a) Vector in the plane

(b) Length of a vector

(c) Angle subtended by a vector

Figure 11.1

11.2

Linear Algebra

Vectors The vector is one of the central objects of linear algebra.
There are several ways to conceptualize a vector. First, we may think of
a vector as an ordered collection of numbers (a 1-dimensional array).
For example, the following vector is the ordered collection of the
numbers 1 and 2: 

1 2

 (11.2)

A vector can be thought   of as a geometric object as well. For
example, we 1 may plot the vector in the 2-dimensional plane, as in
Figure 11.1a. 2 Thinking geometrically, a vector can have a magnitude
(length) and a direction. For example, by the Pythagorean Theorem, the
vector in Figure 11.1a has length p 12 C 22 (11.3) as indicated by the
depiction in Figure 11.1b. We can describe the direction by giving the
angle subtended by the arc from the x-axis to the head of the arrow, as
in Figure 11.1c. We often denote a vector with a lowercase bold letter,
like v, or, when writing by hand, with an arrow, like Ev. We’ll use the
simple notation v to denote a vector when context makes it clear that v
is a vector.

230

CHAPTER 11 Mathematical Tools for Quantum Computing I

Sometimes, we write a vector more explicitly, like so: 0 1 v1 B v2 C B C
vDB : C @ :: A

(11.4)

vn to indicate the number of entries in the vector. So, this vector has
n entries. Some people like to denote vectors with square brackets, as
below 2 6 6 vD6 4

v1 v2 :: :

3 7 7 7 5

(11.5)

vn but it doesn’t matter which you use. We prefer round brackets in this
discussion. We have already encountered the qubit, the quantum analog of
the classical bit, earlier in the book. We used the example earlier in
the book of a qubit that represents the polarization of light, which can
be vertical or horizontal, or in some superposition of these states. As
discussed in chapter 1, we can denote the state “vertical polarization”
with j0i and the state “horizontal polarization” with j1i, or
equivalently, j"i and j!i. Vectors offer a convenient mathematical
representation for these states. For instance,   we denote the state
“vertical polarization” j0i D j"i by the 1 vector and the state
“horizontal polarization” j1i D j!i by the vector 0   0 . 1

Introduction to Dirac Notation Paul Dirac developed a notation for
vectors as well as vector and matrix operations that we use extensively
in quantum mechanics and quantum computing \[92\]. We refer to a vector
of the form j'i as a “ket” in Dirac’s bra-ket notation. We will describe
additional uses of Dirac notation as we build our mathematical toolkit.
Dirac notation and its uses are then summarized in chapter 14.

SECTION 11.2 Linear Algebra

231

Basic Vector Operations Now that we covered vector notation let’s
discuss what we can do with vectors. There are two quite natural
operations to consider. The first of these is addition. We can add two
vectors in the way you would expect – just add the entries! For example,
we add the vectors     1 0 and 0 1 as follows: 

1 0



 C

0 1



 WD

1C0 0C1



 D

1 1

 (11.6)

The notation “WD” is used to denote equality that is true by definition
and not by happenstance. For example, we would write 1 C 1 D 2 and not 1
C 1 WD 2, since the fact that the sum of 1 and 1 is 2 is not by
definition and is a consequence of other facts. However, we would write
N WD f0; 1; 2; 3; :::g to indicate the set of natural numbers, denoted
N, is equal to the set f0; 1; 2; 3; :::g by definition and not as a
consequence of other facts.  11.7

Exercise

Find the sum of the vectors

1 2



 and

4 2

 .

Note that we cannot add vectors with different numbers of entries. For
example, the expression 0 1   1 @ 0 AC 1 (11.8) 0 0 does not make
sense. A moment’s thought convinces us this should be the case: How
would you reasonably add these?1 Let us now consider the next operation:
a special kind of multiplication called scalar multiplication. This
operation allows for the multiplication of a vector by a number, also
called a scalar because it scales the vector. Scalar multiplication also
works in the way you might expect – just multiply each entry of the
vector by the number. For example, we would multiply the vector   1 by
the scalar 3 as in Equation 11.9. 2 1 Occasionally, computer scientists
“pad” the vector which has fewer entries with extra zeros to make the
addition sensible, but we won’t get into this idea here.

232

CHAPTER 11 Mathematical Tools for Quantum Computing I



4



1 2

5 4







1 2

D



4 2

3 6



C



 

2 1

4 2



4 5

Figure 11.2: Addition of vectors

 3

1 2



 WD

31 32



 D

(11.9) 

11.10

Exercise

Perform the scalar multiplication 4 

5 6



The operations of vector addition and scalar multiplication have natural
geometric interpretations as well. Perhaps you recall the “head to tail”
method of vector addition from a previous course. It turns out that the
vector addition described above algebraically encodes precisely this
approach; see Figure 11.2. Scalar multiplication by a number corresponds
to “scaling” or “stretching” the vector by that number; see Figure 11.3.
After becoming comfortable with each of these operations, wemaymix 1
and match. For example, we can consider multiplying the vector by 0 the
scalar 35 , yielding the vector   3     3 3 1  1 5 5  D D
(11.11) 3 0 0 5 5 0   0 and then multiplying the vector by the scalar
45 , yielding the vector 1    4    4 0 0 0 5  D D (11.12) 4 4 1
5 5 5 1 and then adding the resulting vectors, yielding

SECTION 11.2 Linear Algebra



20 24



 D4

5 6

233



24



5 6



6

5

20

Figure 11.3: Scalar multiplication of a vector



3 5

0



 C

0 4 5



 D

3 5 4 5

 (11.13)

In sum, we refer to the expression      3  3 4 1 0 5  C  D
(11.14) 4 0 1 5 5 5     1 0 as a linear combination of the vectors
and . We’ll revisit linear 0 1 combinations in greater detail later.
Using Dirac notation, we can express this as 3 4 j0i C j1i (11.15) 5 5
Having read some of chapter 3, you might recognize this expression as a
superposition of the states j0i and j1i. The numbers 35 and 45 in the
linear combination above are often called coefficients, or in the
language of quantum mechanics, amplitudes, in the superposition of the
states j0i and j1i. The ˇ ˇ2 ˇ ˇ2 square of their absolute values, ˇ 35
ˇ and ˇ 45 ˇ , are the probabilities of observing each of the states,
j0i and j1i, upon measurement. So, in this example, j1i

234

CHAPTER 11 Mathematical Tools for Quantum Computing I

is more likely to be observed than j0i. Note that in quantum mechanics,
we often use complex numbers as the amplitudes, not real numbers.
Exercise You’re invited to verify expression 11.15 is a bona fide
superposition of states in the sense that, as per Born’s rule, the sum
of the squares of the absolute values of the coefficients (or
amplitudes, in the language of quantum mechanics) 35 and 45 is in fact
1: ˇ ˇ2 ˇ ˇ2 ˇ3ˇ ˇ ˇ ˇ ˇ C ˇ4ˇ D 1 ˇ5ˇ ˇ5ˇ

11.16

Exercise Can you find a superposition of the states j0i and j1i so that
each of the states j0i and j1i has equal probability of measurement? Be
careful, you have to make sure the squares of the coefficients, or
amplitudes, adds up to exactly 1! If you read carefully, you’ll find the
answer in previous chapters.

11.17

11.18

A superposition is a linear combination

This leads to an important observation linking quantum mechanics and
linear algebra: a superposition of states can be represented as a linear
combination of the vectors representing their states.

The Norm of a Vector It is quite natural to ask what the length of a
vector is given the geometric interpretation described above. For
vectors in two-dimensional space, our answer   is given by the
Pythagorean Theorem. To see this, consider the vector 3 . We may plot
this vector in the plane, as in Figure 11.4. 4 So, by the Pythagorean
Theorem, we see that the lengthp of this vector is the square root of
the sum of the squares of the entries, i.e., 32 C 42 D 5.

SECTION 11.2 Linear Algebra

235

4

3 Figure 11.4: Another vector in the plane

 11.19

Exercise

Plot the vector

5 12

 in the plane. What is the length

of this vector?

What about vectors with three entries? Let’s imagine the
three-dimensional analog of our previous about lengths of
two-dimensional vectors. 0 discussion 1 1 Consider the vector @ 2 A. We
may plot this vector in three-dimensional 2 space, as in Figure 11.5.
The computation of the length of this vector reduces to two applications
of the Pythagorean Theorem, and ultimately, in the expression p p p 12 C
22 C 22 D 1 C 4 C 4 D 9 D 3 (11.20) 0 1 1 @ for the length of the vector
2 A. 2 Exercise Convince yourself that the computation of the length of
a three-dimensional vector reduces to two applications of the
Pythagorean theorem using the following technique: Think of a point P in
three-dimensional

11.21

236

CHAPTER 11 Mathematical Tools for Quantum Computing I

z

0

1 1 P D@ 2 A 2 O x

y F

Figure 11.5: Vector in space

space. Now, draw the line segment OP whose endpoints are the origin O
and P . From P drop a perpendicular to the floor. Refer to the point
beneath P on the floor by the name F . Draw the line segment PF whose
endpoints are P and F . Then, draw the line segment OF whose endpoints
are O and F . Now, you have formed a triangle with vertices OP; PF , and
OF . To compute the length of the vector pointing from the origin to the
point P , we must compute the length of the hypotenuse of the triangle
we’ve just created. We can’t do that just yet. We focus attention on the
line segment OF . It is a line segment on the floor, a two-dimensional
space. Thus, we can compute the length of the line segment OF using the
usual Pythagorean Theorem. The length of the line segment PF is simply
the height off of the floor of the point P . So, we know the length of
two of the sides of our triangle. We can find the third using a second
application of the usual Pythagorean Theorem. Draw the picture, and
compare to the one in Figure 11.5!

0 B B So, we should expect that the length of any vector B @

v1 v2 :: :

1 C C C is given by a A

vn generalization of the Pythagorean Theorem to n dimensions as q v21 C
v22 C ::: C v2n

(11.22)

Remarkably, this is the case! You’re invited to think about why. The
reason is similar to the above exercise. Recalling that the square root
is equivalent to the 12 power, and rewriting this expression as

SECTION 11.2 Linear Algebra

q 1 v21 C v22 C ::: C v2n D v21 C v22 C ::: C v2n 2

237

(11.23)

reveals an interesting pattern. What is so special about the number 2?
Why not do this for other numbers? For example, exchange 2 for 3,
yielding q 1 3 v31 C v32 C ::: C v3n D v31 C v32 C ::: C v3n 3 (11.24)
These variations on the theme of the0length 1 of a vector are known as
norms. v1 B v2 C B C More generally, given a vector v D B : C, the Lp
-norm2 of v is given by @ :: A vn 11.25

Definition Lp -norm of a vector p

p

jjvjjp WD v1 C v2 C ::: C vp n

 p1

We call the usual length of a vector the L2 -length to emphasize its
calculation via the L2 norm. Likewise, we refer to the length of a
vector calculated using the Lp norm as the Lp -length. In what follows,
we exclusively consider the L2 norm, and we will make clear when we are
using another norm.

The Dot Product During our discussion of the addition and scalar
multiplication operations we can perform with vectors, the curious
reader might have wondered whether there is a natural way to multiply
two vectors. Interestingly enough, the natural approach where we
multiply the corresponding entries is not desirable. One reason we would
like to avoid this type of multiplication for vectors is that this
“product” of two non-zero  vectors oftenbe zero.3 For example,  can 
1 0 if we take the two non-zero vectors and we would have: 0 1     
   1 0 10 0  D D (11.26) 0 1 01 0 2 We sympathize with the
observant reader who notices that the p value of the norm in the
definition is noted with a subscript. However, when writing Lp , we use
a superscript. 3 Note that this component-wise product is known as the
Hadamard product. While this product is named after Jacques Hadamard, it
has no relation to the Hadamard operator beyond the eponymous
connection.

238

CHAPTER 11 Mathematical Tools for Quantum Computing I

Who cares? One argument for why this is not desirable is that it lacks
geometric interpretation.4 There is a way, however, of multiplying two
vectors with a useful geometric interpretation that we will now explore.
Curiously, the product we will focus our attention on takes two vectors
of the same number of components as input and yields, not a vector, but
rather a number. As stated earlier, we can refer to a number as a scalar
quantity or scalar to remind us that numbers “scale” vectors. To
motivate the definition we are about to 0 give,1let us return to the
notion of the length of a vector. Given v1 B v2 C B C a vector v D B :
C, we determined that its L2 -norm is @ :: A vn jjvjj2 WD v21 C v22 C
::: C v2n

 12

(11.27)

and so the square of its length is the square of its L2 norm jjvjj22

 D

v21

C

v22

C ::: C

v2n

 12

2

D v21 C v22 C ::: C v2n

(11.28)

Inspecting this expression further, we can express jjvjj22 D v21 C v22 C
::: C v2n

(11.29)

v1  v1 C v2  v2 C ::: C vn  vn

(11.30)

equivalently as So

1

jjvjj2 D .v1  v1 C v2  v2 C ::: C vn  vn / 2

(11.31)

Squaring both sides, we have jjvjj22 D v1  v1 C v2  v2 C ::: C vn  vn

(11.32)

At the very least, this instructs how we could multiply a vector by
itself: multiply the corresponding entries by themselves and then sum
these products. 4 Another argument is that in most number systems of
interest, the product of two numbers is zero iff at least one of the
numbers is zero. Number systems enjoying this property are called
integral domains and are an important class of objects in the study of
abstract algebra. We exploit this property of numbers when solving
equations. For example, we solve the equation x 2 1 D 0 by factoring the
left-hand side as x 2 1 D .x C 1/.x 1/, and then realize that the only
way the product .x C 1/.x 1/ could be zero is if either x C 1 D 0 or x 1
D 0. We then conclude x D 1 or x D 1.

SECTION 11.2 Linear Algebra

0 B B More precisely, for a vector v D B @

v1 v2 :: :

239

1 C C C, we’re inspired to define the product A

vn of v with itself v  v by v  v WD v1  v1 C v2  v2 C ::: C vn  vn

(11.33)

This is simply the square of the L2 norm of v! Interesting. So, if we
define our multiplication like this, we recover the square of the
length, or L2 norm of a vector, in the special case that we multiply the
vector by itself. Guided by this example, we define the dot product of
two vectors with an equal number of entries 0 B B uDB @

u1 u2 :: : un

1

0

C B C B C;v D B A @

v1 v2 :: :

1 C C C A

vn

in the manner below. 11.34

Definition The dot product of two vectors u  v WD u1  v1 C u2  v2 C
::: C un  vn

We sometimes refer to the dot product of two vectors as the scalar
product to emphasize that the dot product produces a scalar. 11.35
Exercise The reader is invited to verify that in the case that u D v, we
recover the square of the usual length or L2 , the norm of the vector u.

11.36

Definition The L2 norm of a vector as a dot product v  v D v1  v1 C v2
 v2 C ::: C vn  vn D jjvjj22

So, the multiplication of two vectors that we’ve defined is convenient
geometrically in that multiplying a vector by itself in this fashion
yields a

240

CHAPTER 11 Mathematical Tools for Quantum Computing I

number that can be interpreted as the square of the length of the
vector! We’ll also see later that vectors whose dot product is zero can
be thought of as being orthogonal to one another.5

11.3

The Complex Numbers and the Inner Product

Complex Numbers The more experienced reader might be familiar with
complex numbers. Complex numbers arise naturally when solving equations.
For example, we have no trouble solving the equation x 2 1 D 0. However,
solving the equation x 2 C 1 D 0 is more confusing. If we subtract 1
from both sides, we have the equation x 2 D 1, and we are now faced with
the question of finding a number whose square is negative. There is no
real number whose square is negative, so we introduce a new number,
named i , whose square is 1: i2 D

1

(11.37)

In essence, i is the solution to the equation x 2 C 1 D 0, along with i
, of course (as you should check). We refer to i as the imaginary
number.6 We can then form complex numbers by combining a real part and
an imaginary part, like so: 1 1 0 C i; 1 C i; 2 C 3i; and p C p i 2 2

(11.38)

Note that the complex in complex numbers is due to the fact that these
numbers consist of two constituent parts, and thus form a complex, not
because they’re complicated (although they might be to some). In fact,
every complex number can be uniquely expressed in the form a C bi for
some real numbers a and b, and so we might as well define them as such.
We usually denote complex numbers with symbols like z and w, and for a
complex number of 5 The

reader may wonder what the difference is between the terms orthogonal
and perpendicular. The term orthogonal is more general than the term
perpendicular in that it covers the case where one of the vectors is the
zero vector. In this case, we must use the term orthogonal and not
perpendicular. Let us recall that the dot product of any vector with the
zero vector is zero. However, it doesn’t really make sense to say that a
vector and the zero vector are perpendicular to each other, since there
is really no angle formed between a vector and the zero vector. 6 We,
along with Gauss, lament this unfortunate nomenclature.

SECTION 11.3 The Complex Numbers and the Inner Product

241

a C bi b a Figure 11.6: Complex number in the plane

the form z D a C bi, we refer to the real part as Re.z/ D R.z/ D a and
the imaginary part as I m.z/ D I .z/ D b. The set of real numbers, R,
may be recovered from the set of complex numbers, C, as the numbers a C
bi such that b D 0, i.e., numbers of the form a C 0i D a. In an earlier
chapter, we discussed Born’s Rule which states that the square of the
modulus of the amplitude of a state is the probability of that state
resulting after measurement. Let us now review the concept of modulus
and the need for it in this context. With real numbers, there is no need
to invoke the modulus, since squaring the number automatically makes it
positive. However, when squaring a complex number, the result can be a
negative number. Since it is not possible to have a negative
probability, we require that we apply the modulus first before squaring.
The modulus of a complex number a C bi is defined to be p a2 C b 2
(11.39) Thus, the modulus squared is simply a2 C b 2 , which is always a
real, positive number, which is what we require for a probability in the
measurement of quantum systems. Now that we are armed with complex
numbers, let us examine the properties of vectors whose components are
complex, as in Expression 11.40. 

1Ci 1 i

 (11.40)

It is a bit more difficult to develop a geometric interpretation for
such vectors. How would we plot this vector in space? It has four
dimensions!7 7 We

admit that we have not yet given a definition of dimension. For now, it
is fine to think of dimension in the intuitive sense: a point is
0-dimensional, a line is 1-dimensional, a plane is 2-dimensional, space
is 3-dimensional, etc. We will give a mathematical definition of
dimension later!

242

CHAPTER 11 Mathematical Tools for Quantum Computing I

However, each single complex number has a natural geometric
interpretation as a vector in the plane. To see this,  realize  that
any complex number a a C bi may be identified with the vector , as in
Figure 11.6. b Exercise Where do the real numbers “live” in the complex
plane? Can you draw the real line as it is embedded in the complex
plane?

11.41

The Inner Product as a Refinement of the Dot Product We have discussed
how to determine   the square of the norm, or the square of a the
length, of such a vector : we compute b p 2 a2 C b 2 (11.42)
Naturally, this is how we define the norm of the complex number a C bi
so that it corresponds to the square of the length of its corresponding
vector when plotted in the plane. That is, we define the square of  the
norm  of a complex a number a C bi, which may be thought of as a vector
, as a2 C b 2 . b This definition of the norm of a complex number might
confuse you, and rightfully so! If you are not confused, consider this.
Every number may be thought of as a vector with only one entry. This is
a subtle, but important philosophical point – every number is a vector,
in fact.8 Thinking of a complex   number a C bi then as a vector v D
v1 D a C bi with only one entry and following the definition of the
squared norm of a vector given earlier, we compute the square of the
norm of a C bi via

jjvjj22

q 2 WD v21 D v21 D .a C bi /2 D .a C bi/.a C bi/

D a2 C a  bi C bi  a C .bi /2 D .a2

b 2 / C .2ab/i

(11.43)

(11.44)

remembering that we multiply complex numbers .a C bi/; .c C d i/ using
the usual distributive law of multiplication, and that i 2 D 1. So, for
example, 8 ...

and every vector is a matrix! See the discussion of matrices in Section
12.4.

243

SECTION 11.3 The Complex Numbers and the Inner Product

by the distributive property of multiplication, the product of complex
numbers 1 C 2i and 3 C 4i is .1C2i/.3C4i/ D .13C14i C2i 3C2i 4i / D
13C.14/i C.23/i C.24/i 2 (11.45)

D 13C.14C23/i C.24/. 1/ D .13 24/C.14C23/i D

5C10i (11.46) 2 The reader can regard i as x, replacing any x
encountered in the computation instead with 1. In fact, this is exactly
how algebraists think of this. 11.47

Exercise

Practice multiplying complex numbers by multiplying .3 C 4i /.4 C 5i /

Then, multiply .3 C 4i /.3

4i /:

Does the second multiplication remind you of something we discussed
previously in the Norms section?

In any case, what we have now for the square of the norm jjvjj22 D .a2

b 2 / C .2ab/i

(11.48) a2

b2

does not look at all like what we called the square of the norm C of the
2 2 complex number a C bi. Even more disturbing is that .a b / C .2ab/i
is potentially an imaginary number, since 2ab is likely nonzero (if both
a and b are nonzero). This is disturbing because such an expression
cannot be as easily interpreted as a length and we would like the norm
of a complex number to be interpretable as its length.9 What is going on
here? Let us inspect the expression a2 C b 2 a bit more carefully.
Clever readers (who have done the previous exercise) might recognize
expression 11.49 (check it using the distributive property). 9 Refer to
the later section on Hermitian Operators where we discuss why we can’t
measure with complex numbers.

244

CHAPTER 11 Mathematical Tools for Quantum Computing I

i

R Figure 11.7: The complex plane

a2 C b 2 D .a C bi /.a

bi/

(11.49)

The number a bi is known as the complex conjugate of the number a C bi.
We can also simply call it the conjugate when we’re well-aware that
we’re working with complex numbers. We often denote a complex number by
z, and the conjugate of z by z. For example, if we denote a C bi by z,
then z D a bi. The act of changing a complex number into its conjugate
is known as conjugating. You might wonder how to conjugate a complex
number like 1 i . The answer is 1 C i . That is, plus becomes minus and
vice versa. 11.50

Exercise

Conjugate the following: 3 C 4i; 3

4i; 1

i.  

 What if we have a real number a and think of it as a vector a with
only one entry? Then, the square of the norm of this vector, following
the previous definition, is simply a2 . We may recover the norm of a by
taking (the positive) square root, which makes sense since the length of
a should be simply a, and we do not encounter any difficulties as we did
with complex numbers. One explanation for this peculiarity is that
perhaps we should have been considering real numbers as complex numbers
all along. In fact, a previous exercise asking you to realize the real
line as “living” in the complex plane makes this explicit. You can check
your solution to that exercise by referencing Figure 11.7. What we mean
by this is that a real number a can be thought of as a complex number by
expressing it as a D a C 0i

(11.51)

Writing a as a C 0i reveals that the complex conjugate of a is simply a,
since a C 0i is a 0i D a. Then, the product of a and its complex
conjugate is .a

0i /.a C 0i / D a  a D a2

(11.52)

SECTION 11.3 The Complex Numbers and the Inner Product

245

In other words, our definition of the square of the norm for real
numbers remains the same even if we involve the conjugate! This
observation makes us realize that we should define the square of the
norm of any number, complex or not, as the product of that number with
its conjugate. More precisely, using the previously introduced notation,
jjzjj22 WD zz

(11.53)

We often omit this extensive notation when the context makes clear that
we are using the L2 norm, replacing it with jzj2 D zz. This discussion
of how to define the square of the norm of any number instructs our
definition of the square 0 of1the norm of any vector, complex v1 B v2 C
B C entries or not. For any vector v D B : C, we define the square of
the norm @ :: A vn of v to be: 11.54

Definition Squared norm of a vector jvj2 WD v1  v1 C v2  v2 C ::: C vn
 vn

Exercise You’re encouraged to verify that this definition recovers the
previous definition for vectors whose entries are exclusively real
numbers, and also that it effectively computes the square of the norm of
any real or complex number.

11.55

Generalizing this, we define the inner product of two vectors (again,
with equal number of entries): 0 1 0 1 u1 v1 B u2 C B v2 C B C B C u D B
: C;v D B : C : : @ : A @ : A un to be

vn

246 11.56

CHAPTER 11 Mathematical Tools for Quantum Computing I

Definition Inner product of two vectors hu; vi WD u1 v1 C u2 v2 C ::: C
un vn

Exercise Similarly, you’re invited to verify that this definition
recovers the square of the norm of any real or complex number in the
case u D v is a real or complex number, i.e., for any real or complex
number z, hz; zi D jzj2 . You should also verify that the definition of
the square of the norm is recovered for a vector whose entries are all
real numbers.

11.57

It should be noted that the dot product and the inner product agree only
if the entries of the vectors we are considering are exclusively real
numbers. The inner product generalizes this operation to vectors with
complex entries. Recalling Dirac notation, you will likely notice the
uncanny resemblance of the notations hu; vi and hujvi – the only
difference is the line in the middle! Paul Dirac was probably inspired
by the inner product notation when he decided on his notation. That
being said, if we have two vectors, written in Dirac notation as huj and
jvi, we write their inner product as hujvi WD hu; vi

(11.58)

So, the notation hujvi literally means “the inner product of the vectors
u and v.” So, in what follows, we will assume that our vectors may
include complex entries. We will revisit the inner product from a more
formal and abstract point of view later on in our description of a
Hilbert space.

The Polar Coordinate Representation of a Complex Number We now explore a
remarkable connection between complex numbers and geometry. Every
complex number can be thought of as living in the twodimensional plane
depicted in Figure 11.7. We have discussed how  acomplex number of the
form z WD a C bi may be a thought of as a vector . Thinking of z as a
vector in two-dimensional b space should convince us that it’s
reasonable to assign a complex number an L2 -norm, i.e., a length.
Specifically, the complex number z D a Cbi , thought

247

SECTION 11.3 The Complex Numbers and the Inner Product =2

a C bi p a2 C b 2  

0

3=2

Figure 11.8: Angle subtended by radius

 of as a vector

a b

 , has L2 norm given by the Pythagorean Theorem: p a2 C b 2

(11.59)

Visualizing complex numbers in this fashion should also make it
reasonable to assign a complex number an angle. Specifically, we assign
the complex number a C bi the angle,   , subtended by the arc from the
positive real  a axis to the head of the vector in the counterclockwise
direction, as in b Figure 11.8. We can use some simple trigonometry to
describe this angle. Let’s refer to the angle by  . Then,  lives in
the right triangle depicted in Figure 11.9 and so satisfies the equation
tan. / D

b a

(11.60)

If you’re shaky on trigonometry, remember that the tangent of an angle 
in a right triangle is the opposite over the adjacent. Let’s recall the
inverse tangent function, known by the name tan 1 , or sometimes arctan.
We’ll use

248

CHAPTER 11 Mathematical Tools for Quantum Computing I =2

a C bi b p a2 C b 2  

a

0

3=2

Figure 11.9: Right triangle where the angle lives

the name arctan.10 The role of the inverse tangent function is to take a
number as input and give an angle as output. For example, arctan.y/
means “the angle that makes tangent equal to y.” Since tan./ D

b a

applying arctan to both sides yields the equation   b arctan .tan.//
D arctan a

(11.61)

(11.62)

So, we can express the angle, , in terms of a and b as   b  D arctan
a

(11.63)

All this being said, we can refer to the L2 -norm of the complex number
as its radius, and refer to the angle as its... well, angle. In summary,
a complex number a C bi has a radius 10 tan 1 could be confused with the
reciprocal function of tangent, known as cotangent, 1 which is expressed
.tan/ 1 D tan D cot.

SECTION 11.3 The Complex Numbers and the Inner Product

r WD

p

a2 C b 2

249

(11.64)

and an angle  WD arctan

  b a

(11.65)

We can also describe a complex number by simply giving a radius and
angle. For example, let’s try to figure out which complex number is
described by the radius 1 and the angle  WD 4 radians (45 degrees). If
we write the complex number temporarily as a C bi, our problem reduces
to determining the numbers a and b given the radius r and the angle  .
We know from the previous paragraph that the radius r of a complex
number of the form a C bi is given by p r D a2 C b 2 (11.66) and we know
that the angle  is given by   b  D arctan a

(11.67)

If we now apply tan to both sides of 11.67, we obtain tan./ D Since  D

 4,

tan./ D tan

b a

  4

(11.68)

D1

(11.69)

So, 1 D tan

  4

D tan./ D

b a

(11.70)

and we see that

b (11.71) a Multiplying by a on both sides reveals a D b. Great, so now
we know that a D b! Knowing that a D b, we look toward the equation p r
D a2 C b 2 (11.72) 1D

We are told that the radius r is equal to 1, so we know that p 1 D r D
a2 C b 2

(11.73)

250

CHAPTER 11 Mathematical Tools for Quantum Computing I

and since a D b, we may replace b with a yielding instead p p p 1 D r D
a2 C b 2 D a2 C a2 D 2a2

(11.74)

Squaring both sides yields 1 D 2a2 , and dividing both sides by 2
reveals that 1 2 2 D a . Then, taking the square root of both sides
reveals that: r 1 aD (11.75) 2 It turns out that

r

p 1 1 1 Dp Dp 2 2 2

(11.76)

so we now know that

1 aDbD p (11.77) 2 Fantastic — we now know our complex number a C bi
described by the radius 1 and the angle 4 is actually 1 1 a C bi D p C
p i 2 2

(11.78)

So, we have converted the polar expression of a complex number given by
radius 1 and angle  D 4 to what we refer to as its rectangular
expression p1 C p1 i: 2

2

Definition complex number

11.79

Rectangular (or Cartesian) and polar form of a

In general, we say that a complex number of the form a C bi is given in
rectangular or Cartesian form, and that a complex number described by a
radius r and an angle  as .r; / is given in polar form. Exercise Check
that z D i.e., z has radius 1 and angle 4 .

11.80

p1 2

C

p1 i 2

enjoys the above properties,

p

Exercise Try to convert the Cartesian expression form by determining its
radius and angle.

11.81

3 2

C 12 i to polar

SECTION 11.3 The Complex Numbers and the Inner Product

251

=2

z r D1 D

 4



0

3=2

Figure 11.10: Unit complex number with angle

 4

11.82 Exercise To see that Cartesian expressions can sometimes have
“ugly” polar p expressions, convert 1 C 2i to polar coordinates and
check that the radius is 5 and the angle is arctan 12 , which,
unfortunately, cannot be expressed in any more familiar way.11

Recalling a bit of trigonometry, we could have determined this already!
Given the radius r D 1 and the angle  D 4 radians, we have the picture
in Figure 11.10. Recalling the definition of sine and cosine, we see
that the value for a should be a D r  cos. / (11.83) and the value for
b should be b D r  sin. / We can reformulate a as 11 In

fact, the arctan of any natural number is irrational.

(11.84)

252

CHAPTER 11 Mathematical Tools for Quantum Computing I =2

z r D1 D

 4



cos

 4



sin

 4



p

D

p

D

2 2

0

2 2

3=2

Figure 11.11: The trigonometry of a complex number

a D 1  cos

  4

p 2 D 2

and b as b D 1  sin

 

p

11.87

Exercise

Check that

2 2

D

4 p1 2

(11.85)

p D

2 2

(11.86)

by cross-multiplying.

The above exercise makes us realize we could have determined a and b all
along just having recalled some basic trigonometry! So, we’ve discussed
how a complex number gives rise to a radius and an angle, and
conversely, how a radius and an angle give rise to a complex number. We
realize now that the descriptions are equivalent! Exercise Convince
yourself that giving a complex number in the form a C bi is equivalent
to giving a radius and an angle .r;  /. Recall

11.88

SECTION 11.3 The Complex Numbers and the Inner Product

253

=2

e i D cos. / C i sin. / 1  

0

3=2

Figure 11.12: Euler’s formula

that we say that the form a C bi is rectangular or Cartesian (for
Cartesian coordinates) and that the form .r; / is polar.

We can take this one step further with Euler’s formula (pronounced
“oiler”). Euler’s formula states that a complex number z with radius 1
and angle , i.e., a complex number living on the “unit circle” can be
expressed as z D e i D cos./ C i sin. /

(11.89)

That z D cos./ C i sin./ should not be surprising, as it follows our
previous discussion, but rather that the number e comes into play here.
If you’re not familiar with the number e, check out our explanation in
chapter 13. This formula is one of the most remarkably beautiful
formulas in all of mathematics for many reasons, including the deep
connection it illuminates between complex numbers — a priori, an
algebraic phenomenon — and geometry. We discuss this equation further
and prove its validity in our chapter about additional mathematical
topics. For now, we’d like for you to take away the following idea:

254

CHAPTER 11 Mathematical Tools for Quantum Computing I

11.90

Euler’s formula

A complex number z with radius 1 and angle  can be expressed as z D e
i That being said, if our complex number z has radius r instead of 1,
and angle , we may write as z D re i , following Euler. Exercise
Convince yourself that a complex number z whose radius is r and whose
angle is  can be expressed z D re i using Euler’s formula as above.

11.91

We’ll exploit this idea later to define a special class of
transformations that rotate space by any specified angle!

11.4

A First Look at Matrices

Basic Matrix Operations Having read chapter 3, you encountered matrices,
which a priori resemble rectangular grids of numbers, e.g., the Pauli X
operator x (also known as the NOT operator):   0 1 x D X WD (11.92)
1 0 and the Pauli Z operator z :  z D Z WD

1 0

0 1

 (11.93)

from chapter 3. Matrices might even involve complex numbers, like the
Pauli Y operator y :   0 i y D Y WD (11.94) i 0 We can multiply
matrices by numbers, like you’ve seen with the Hadamard operator from
chapter 3. Just multiply all of the entries by that number, like so:

SECTION 11.4 A First Look at Matrices



1 H WD p 2

1 1

1 1

p1 2 p1 2

 WD p1 2 p1 2

D

p1  2 p1  . 2

1 1

p1 2 p1 2

255

!

1

(11.95)

1/

! (11.96)

We can also add two matrices by adding their corresponding entries, like
so: 

1 2 3 4



 C

5 6 7 8





1C5 2C6 3C7 4C8

WD



 D

6 8 10 12

 (11.97)

A matrix is a representation of a more fundamental object called a
linear transformation. In fact, so is a vector, since we may think of a
vector as an n  1 matrix. The term transformation begs the question
transformation of what? 11.98

Matrices transform space

A matrix does not merely transform a particular vector or set of
vectors; it transforms an entire vector space. To gain an understanding
of how a matrix might be thought of as a transformation of space, we
will consider a few geometric examples. However, before we can explain
these geometric examples, we will need to learn how to multiply a vector
by a matrix. This will seem a bit weird at first, but we will explain
why it’s defined this way later on in this text. Let   e (11.99) f be
a vector and



a b c d

 (11.100)

be a matrix.  We multiply the vector 

a b c d

e f 



 by the matrix

e f



 WD

a b c d

aeCbf ceCd f

 like so:  (11.101)

If you’re observant, you might recognize a  e C b  f resembles the dot
product described earlier. In fact, each of the expressions a  e C b 
f and

256

CHAPTER 11 Mathematical Tools for Quantum Computing I



a b



c  e C d  f (respectively) are literally the dot products of the
vectors       e c e and , and of and (respectively).12 f d f In
other words, for vectors with exclusively real entries, the
multiplication we’ve just defined can be thought of as a sequence of dot
products! Recall the Pauli Z matrix:   1 0 Z WD (11.102) 0 1 and
consider the vector:



0 1

 (11.103)

Recall from the previous description that we write the product of the
matrix   1 0 (11.104) 0 1 and the vector

as





1 0

0 1

0 1





(11.105) 0 1

 ;

(11.106)

and we multiply them as follows        1 0 0 10C01 0 WD D 0 1
1 0  0 C . 1/  1 1

(11.107) 

0 1



We could say then that the matrix has transformed the vector into   0
the vector ! 1   1 11.108 Exercise Figure out where the vector is sent
via this 0   1 transformation. More precisely, multiply the vector by
the matrix 0 12 Actually,

if all of a; b; c; d; e; f are strictly real numbers, then these dot
products are literally the inner products of the vectors.

SECTION 11.4 A First Look at Matrices

257

   1 1 0 and see where the vector ends up! Do you see a relation0 0 1
ship between the transformed vectors and the columns of the matrix? Try
to formulate a conjecture!



In fact, we may use Dirac notation to express the relationship between
the matrix Z and the states j0i and j1i like so: Z jj i D . 1/j jj i

(11.109)

for all j 2 f0; 1g, as you should check!  Exercise

Learn why the NOT operator X D

0 1 1 0



is also   1 known as the “bit flip” operator by showing that
multiplying the vector , 0 which represents   the state j0i, by the
matrix X “flips the state” to j1i, i.e., the 0 vector . 1 11.110

We can likewise multiply two matrices as follows:      a b e f ae
C bg af C bh WD c d g h ce C dg cf C dh

(11.111)

A helpful graphic depicting matrix multiplication is given in Figure
11.13. Exercise Realize that the multiplication of a vector by a matrix
described earlier can in fact be thought of as the multiplication of two
matrices, where we think of the vector as an n  1 matrix. 11.112

Extending the idea of realizing matrix-vector multiplication as simply
matrix-matrix multiplication as described in the exercise above, we can
also multiply matrices of different dimensions. For example, consider
the matrices 0

1 a b @ c d A e f

(11.113)

258

CHAPTER 11 Mathematical Tools for Quantum Computing I

B 2 6 6 6 4

2

A

6 6 6 6 6 6 6 6 6 6 6 6 4

a11

a12

a21

a22

a31

a32

a41

a42

3 b11

b12

b13

b21

b22

b23

7 7 7 5

3 2

3

7 7 7 7 7 7 7 7 7 7 7 7 5

7 7 7 7 7 7 7 7 7 7 7 7 5

6 6 6 6 6 6 6 6 6 6 6 6 4

a11 b12 C a12 b22 a31 b13 C a32 b23 Figure 11.13: Matrix multiplication

and 

g h i j k l

 (11.114)

where the matrix entry i is simply the letter, not the imaginary number
i . Then, we may multiply these matrices like so: 0

1 0   a b ag C bj @ c d A g h i WD @ cg C dj j k l e f eg C fj

1 ah C bk ai C bl ch C d k ci C d l A eh C f k ei C f l (11.115) It
should be noted that the product of a 3  2 matrix and 2  3 matrix
yields a 3  3 matrix! Now that we have seen how to multiply a vector by
a matrix, we can see the method for multiplying two matrices, as
follows:

SECTION 11.4 A First Look at Matrices

p

n n m

259

p

B D m

A

AB

Figure 11.14: Size of the matrix product

1   a b g h i @ ga C hc C ie gb C hd C if A c d WD j k l ja C kc C le
jb C kd C lf e f (11.116) This should be a surprise – we got a 2  2
matrix by multiplying the two matrices in the opposite order! 

11.117



0

Size of the matrix product

In general, if A is an m  n matrix and B is an n  p matrix, then AB is
an m  p matrix. The picture in Figure 11.14 depicts this phenomenon,
exemplified by equations 11.115 and 11.116. So, when multiplying two
matrices, the “inner” dimensions must agree, and the resulting matrix
will have dimensions equal to the “outer dimensions” of the two
matrices. When faced with the following expression     1 0 0 1 1 0
(11.118) 0 1 1 0 0 1 we might wonder how to compute it given that we’ve
not discussed how to multiply three matrices at a time. Well, think of
an analogous scenario. When asked to compute the product 2  3  4 what
do we do? Well, you have probably never met anyone capable of
multiplying three numbers at a time (at least, we have never met anyone
like that). However, we know that it’s fair to do either of the
following things in an effort to compute the product: Either we compute:
.2  3/  4 (11.119) or we compute:

260

CHAPTER 11 Mathematical Tools for Quantum Computing I

2  .3  4/

(11.120)

That is, we either multiply 2 and 3 first, and then multiply the result
(6) by the remaining 4, or we multiply 3 and 4 first, and then multiply
the result (12) by the remaining 2. What is remarkable is that we get
the same answer (24) either way! We can hope that the same is true for
matrices. Explore this idea in the following exercise: Exercise

Recognize    1 0 0 1 1 0 0 1 1 0 0 1     1 0 0 1 as the product
ZXZ of the matrices Z D and X D . 0 1 1 0 Then, compute the product ZXZ
by first computing ZX and then multiplying the result by the remaining Z
on the right. More precisely, compute 11.121



.ZX /Z Then, compute Z.XZ/ and check that you get the same answer either
way! So, you’ve shown that, at least for these three matrices, matrix
multiplication is an associative operation.

We’ll revisit associative operations later on when we discuss the formal
definition of a vector space. We won’t prove that matrix multiplication
is associative in general here. When we say that matrix multiplication
is associative, we mean that for all matrices A; B; C , .AB/C D A.BC /
whenever the product makes sense, i.e., the dimensions agree. In fact,
we won’t bring the issue up again until after we’ve shown that
multiplication of matrices is equivalent to composition of functions, at
which point the fact that matrix multiplication is associative will
become an obvious fact! So, when faced with a product like    1 0 0
1 ZX j0i D j0i (11.122) 0 1 1 0 we first think of the vector on the
right as a 2  1 matrix. We then realize that we may first compute the
product of the two matrices on the left, i.e.,

SECTION 11.4 A First Look at Matrices

 ZX D

1 0

0 1



0 1 1 0



 D

0 1 1 0

261

 (11.123)

then apply the resulting matrix to the vector (2  1 matrix) j0i, like
so:        0 1 0 1 1 0 j0i D D (11.124) 1 0 1 0 0 1 Or we could
iteratively apply the matrices to the vector j0i, first applying the
matrix X      0 1 1 0 X j0i D D D j1i (11.125) 1 0 0 1 then
applying the matrix Z to the resulting vector, like so       
0 1 0 0 0 Z.X j0i/ D Z.j1i/ D Z D D 1 0 1 1 1 (11.126) Either way, we
get the same result! Please note that when applying a sequence of
matrices to a vector, we go from right to left, sometimes said
“inside-out,” so in this case, we apply X first, then Z. However, when
multiplying the matrices, we go from left to right. What we are
realizing is that: 11.127

Multiplying several matrices

The result of applying the composition of two transformations to a space
is equivalent to applying them iteratively. Again, we won’t prove this
here, but we promise, it will become obvious once we’ve established the
correspondence between matrix multiplication (and thus, multiplication
of vectors by matrices) and composition of functions.

The Identity Matrix Thinking of matrices as transformations of space
leads us to believe that there should be a matrix that does not
transform the space at all. In other words, it is natural to ask if
there is a matrix that has no effect on any of the vectors it
multiplies. In two dimensions, the answer is the matrix   1 0 I2 WD
(11.128) 0 1

262

CHAPTER 11 Mathematical Tools for Quantum Computing I

The subscript 2 is there to inform us that this is the identity matrix
for 2dimensional space. We refer to this matrix as the identity matrix
because it preserves the identity of the vectors it acts on.  Let’s 
see that the matrix I2 deserves its name. Let’s multiply the vector 1 by
the matrix I2 to see what we get: 0  I2 

1 0



 WD

1 0 0 1

       1 11C00 1  D D (11.129) 0 01C10 0 

It’s the same vector! We leave it to you to check that the vector

0 1

 is also

preserved under multiplication by I2 .  11.130

Exercise

Verify that the vector

0 1

 is unchanged under multi-

plication by I2 .

However, the matrix just described is the identity matrix for
2-dimensional space. What if we want an identity matrix for
three-dimensional space? No problem – just make the matrix a little
bigger: 0 1 1 0 0 I3 WD @ 0 1 0 A (11.131) 0 0 1 We also call this the
identity matrix, although it is specific to three-dimensional space. 0

1 0 1 0 1 1 0 0 @ A @ A @ 11.132 Exercise Multiply each of the vectors 0
; 1 ; 0 A 0 0 1 by this new identity matrix for three-dimensional space
and check that it deserves its name.

In fact, each dimension has its own identity matrix, as you might now
expect! To build the identity matrix for n-dimensional space, simply
create an n  n matrix with 1’s along the diagonal and 0’s elsewhere,
like so

SECTION 11.4 A First Look at Matrices

0 B B In WD B @

1 0 ::: 0 1 ::: :: :: : : : : : 0 0 0

1 0 0 C C C 0 A 1

263

(11.133)

This matrix has the property that it preserves any vector of
n-dimensions that it acts on, as you should verify.

Transpose, Conjugate and Trace We have now seen that not all matrices
have to be square. For example, consider 0 1   a b g h A WD @ c d A ;
B WD (11.134) i j e f The matrix A has 3 rows and 2 columns and B has 2
rows and 2 columns, so B is square, while A is not. A very natural
operation to consider when thinking of matrices as rectangular grids of
numbers is the transpose. Here are the transposes, denoted AT and B T ,
of the above matrices:     a c e g i T T A WD ; B WD (11.135) b d f
h j What happened? We could describe this operation as turning rows into
columns and vice versa. Visual learners might recognize that transposing
a matrix is reflecting its entries over an imaginary line extending from
the upper left-hand corner of the matrix to the lower right-hand corner.
We can just as well transpose the transposed matrices, i.e., compute .AT
/T and .B T /T . You’re invited to check that .AT /T is just A again in
an exercise below. 11.136

Exercise

Find the transpose of the following matrix: 0 1 1 2 3 B 4 5 6 C B C @ 7
8 9 A 10 11 12

Exercise Check that transposing the already transposed matrix AT yields
A. More precisely, check that .AT /T D A. So, the operation of
transposing inverts itself!

11.137

264

CHAPTER 11 Mathematical Tools for Quantum Computing I

Exercise For which matrices A is A equal to AT ? We call such matrices
symmetric (for good reason). If a matrix is symmetric and all of its
entries are real numbers, we call it real symmetric. Real symmetric
matrices are very special matrices that deserve quite a bit of
attention, as we’ll see later.

11.138

We can transpose vectors just as well as matrices. To see this, we
recognize that we can think of any vector as a matrix. For example,
think of the vector   1 0 as a 2  1 matrix, so its transpose is the 1
 2 matrix 

1 0

T D

1 0



(11.139) 

11.140

Exercise

Find the transpose of the vector 

0 1

0 1

 , i.e., find

T



1 0



We’d like to mention now why it is that we consider the vector  T  1
and its transpose D 1 0 different objects. Of course, they are 0
visually different, but the difference is more than just in their
presentation.   1 For starters, we cannot multiply the vector by
itself, i.e., the ex0 pression    1 1 (11.141) 0 0 does not make
sense, as you should recall from our previous discussion about
appropriate dimensions for the product of two matrices. Explicitly, the
vector   1 has dimensions 2  1, and we see that the product of a 2 
1 matrix 0

SECTION 11.4 A First Look at Matrices

265

with a 2  1 matrix does not make sense since the “inner” dimensions, 1
and 2, do not agree. However, the expression    T   1 0 1 1 1 D
(11.142) 0 0 0 makes perfect sense, since the inner dimensions are both
2, as you should  T   1 1 verify. Thinking of each of and as
matrices and following 0 0 the description of matrix multiplication
described above, we have    T   1 0 1 1 1 D D11C00D1 (11.143) 0
0 0 This result makes sense since we multiplied a 1  2 matrix by a 2 
1 matrix and got a number, i.e., a 1  1 matrix! Another fun operation
we can perform on matrices is conjugation. Yes, the same conjugation
from earlier! Let’s see how this works. Consider the matrix   1Ci 0 C
WD (11.144) 0 1 i We denote by C the conjugate of the matrix C .    
1Ci 0 1 i 0 C WD D 0 1Ci 0 1 i

(11.145)

To conjugate a matrix, just conjugate each of its entries. Exercise
Figure out when a matrix is equal to its conjugate. Hint: When is a 1 
1 matrix, i.e., a number, equal to its conjugate? 11.146

Of course, viewing a vector as a matrix  allows us  to conjugate any
vector. 1Ci For example, the conjugate of the vector is the vector 1 i 

1Ci 1 i



 WD

1Ci 1 i



 D

1 i 1Ci

 (11.147)

Let’s tie a few concepts together now by expressing the inner product of
two vectors using the notation we’ve developed.

266

CHAPTER 11 Mathematical Tools for Quantum Computing I

0 B B Given two vectors u D B @

u1 u2 :: :

1

0

C B C B C and v D B A @

un

v1 v2 :: :

1 C C C, we would express A

vn

their inner product via hu; vi WD u1  v1 C u2  v2 C ::: C un  vn

(11.148)

using our earlier notation. Notice that 0 u1  v1 C u2  v2 C ::: C un 
vn D

u1 ; u2 ; : : : ; un

B B B @

v1 v2 :: :

1 C C C (11.149) A

vn which we may express using our recently developed notation for
transpose as follows: 0 1 0 1T 0 1 v1 u1 v1 C B C B C B B v2 C B u2 C B
v2 C u1 ; u2 ; : : : ; un B : C D B : C B : C (11.150) @ :: A @ :: A @
:: A un

vn

vn

and we may further adorn this expression with our new notation for the
conjugate of a matrix (and thus a vector) as follows: 0 B B B @

u1 u2 :: : un

1T 0 C C C A

B B B @

v1 v2 :: :

1 C C C D uT v A

(11.151)

vn

All in all, we may compactly express the inner product of vectors u and
v as simply uT v – fantastic! So, in summary, we have the following
equivalent expressions for the inner product of two vectors u and v: hu;
vi D hujvi D uT v

(11.152)

By convention, we can refer to uT as u , so we have hu; vi D hujvi D uT
v D u v

(11.153)

SECTION 11.4 A First Look at Matrices

267

We can go even further to relate this to Dirac notation! What the above
string of equalities reveals is that we may think of the “bra” 0 huj of
1 a vector u u1 B u2 C B C as the conjugate-transpose of the vector u,
i.e., for a vector B : C, : @ : A un 0

u1 u2 :: :

B B huj jvi D uT v D B @

1T 0 C C C A

B B B @

un

1 C C C A

(11.154)

vn 0

D

v1 v2 :: :

u1 ; u2 ; : : : ; un

B B B @

v1 v2 :: :

1 C C C A

(11.155)

vn Given that we now have the operations of transposition and
conjugation at our disposal, we may apply both to a matrix to yield what
is known as its conjugate transpose. Exercise First, conjugate the Pauli
Y operator Y , i.e., the matrix  0 i Y D . Then, transpose the result.
We call this the conjugate transi 0 pose of the matrix Y . Do you notice
something special about the relationship between Y and its conjugate
transpose?

11.156

We’ll show now that you could equivalently transpose the matrix Y and
then conjugate. First, we transpose Y , yielding Y

T

 D

0 i

i 0

T

 D

0 i

i 0

 (11.157)

Then, we conjugate Y T : .Y T /

 D

0 i

i 0



 D

0 i

i 0



 D

0 i

i 0

 (11.158)

268

CHAPTER 11 Mathematical Tools for Quantum Computing I

Check to see that you got the same thing in the exercise above! So, in
general, we may compute the conjugate transpose of a matrix, and we may
compute it in either order: conjugate first, then transpose, or
transpose first, then conjugate. We will see later that the idea of the
conjugate transpose is important for defining a class of operators
called unitary operators. A unitary operator is an operator whose
inverse is its conjugate transpose, as we will consider further in this
section. This is important because quantum states are represented as
vectors with norm 1 living in something called a Hilbert space (which we
will define rigorously later in this exposition). It turns out that
unitary operators have the special property that they preserve the norm
of the vectors on which they operate. So, the application of a unitary
operator to a vector whose norm is 1 is a vector whose norm is also 1.
There is another important operation that we can perform on a matrix,
known as taking the trace. Let us recall that the primary diagonal of
interest to us in analyzing matrices is the one that runs from the upper
left-hand corner to the lower right-hand corner; we refer to this as the
main diagonal. Given a matrix A, we can find the sum of entries of the
main diagonal of A like so:   1 3 AD 7! 1 C 4 D 5 (11.159) 8 4 We
notate this as Tr.A/ D 5, which can be read, “The trace of A is 5.” 

 5 6 11.160 Exercise Compute the trace of the matrix B D . Then, 7 8
check that the trace of B is the trace of B T . That the trace of a
matrix and its transpose are always the same is a theorem of advanced
linear algebra, so we content ourselves with this example for now.

The trace has a number of interesting properties including the
following: 11.161

Invariance of the Trace

The trace remains invariant among matrices that are similar. Similar
matrices can be thought of as matrices that represent the same linear
transformation viewed from different perspectives.13 Now we are 13
Unfortunately, we won’t be able to discuss the idea of similar matrices
in this exposition, but the name should give some indication of the
idea. Two matrices are similar if they are in

SECTION 11.4 A First Look at Matrices

269

equipped to verify the list of equalities of products of matrices stated
in chapter 3. Recall from earlier chapters that H is the Hadamard
operator defined as 1 H WD p 2



1 1

1 1



X is the Pauli X operator x , also known as the NOT (or “(qu)bit flip”)
operator defined as  X WD



0 1 1 0

Z is the Pauli Z operator z defined as  Z WD

1 0

0 1



Y is the Pauli Y operator y defined as  Y WD

0 i

i 0



and I is the identity operator, which we’ll take to be two-dimensional,
so  I WD

1 0 0 1



Recall also that for any matrix A, A denotes the conjugate transpose of
A. Exercise Verify the following list of equalities of matrices:  HXH D
Z  HZH D X  HYH D Y  H D H

11.162

some sense the same. We can make this idea more precise when we
understand the notion of a basis, and what it means to change a basis.
The idea is that two matrices are similar iff they differ only by a
change of basis. This invariance is useful for distinguishing classes of
quantum operators.

270

CHAPTER 11 Mathematical Tools for Quantum Computing I

So, we can say that the Hadamard operator H is unitary,14 since its
inverse is its conjugate transpose, H

1

D H

Matrix Exponentiation Let us now discuss the exponentiation of matrices.
To do this, first we discuss powers of matrices. We can apply the same
matrix successively to a vector, as in X.Xj i/ D X 2 j i The notation on
the right hand side of this equation suggests we are applying the square
of the X operator (matrix) to the vector. Indeed, powers of linear
operators (matrices) are defined in this way. In general, the notation
Ak for any operator A and any positive integer k means k successive
applications of A. This leads naturally to the notion of the exponential
of a matrix, denoted exp A or e A . The way this is defined is through
the Taylor series of e x , namely ex D

1 X 1 n x : nŠ

nD0

In the same way, we use this to define the exponential of a matrix exp A
 e A WD

1 X 1 n A nŠ

(11.163)

nD0

We define A0 D I , the identity matrix, for any matrix A. Although we
will not prove it here, it can be shown that the infinite sum in
(11.163) converges for any matrix A and thus is well-defined. 11.164

   

Exercise DI Y2 D I Z2 D I H2 D I

Please verify the following.

X2

14 We

will discuss unitary operators later on in this text.

SECTION 11.5 The Outer Product and the Tensor Product

271

Exercise Verify that for any operator A such that A2 D I , the following
identity holds:

11.165

e iA D cos./I C i sin. /A

(11.166)

For this exercise, it will be useful to recall the Taylor series for
cosine and sine. Use this expression for the Pauli matrices X, Y and Z.

11.5

The Outer Product and the Tensor Product

The Outer Product as a Way of Building Matrices Now we’ll demonstrate an
operation that builds a matrix from two vectors.  T    1 1 Consider
the vectors D 1 0 and : 0 0 As discussed earlier, it is perfectly
sensible to compute the product    1 0 1 (11.167) 0 since it is the
product of a 2  1 matrix with a 1  2 matrix, i.e., a 2  2 matrix.
Exercise Practice your matrix computation skills and compute the above
matrix product.

11.168

If you completed the above exercise, you now know that        1 0
1 11 10 1 0 D D 0 01 00 0 0

(11.169) 

 1 We call the resulting matrix the outer product of the vector with 0
itself. We’d like to emphasize that this is just fancy terminology! The
outer product is simply the matrix product of two vectors. We can think
of the first

 100e

CHAPTER 11 Mathematical Tools for Quantum Computing I

vector as a 2  1 matrix and the second vector as a 1  2 matrix,
remembering that the the product of an m  n matrix and an n  p matrix
is an m  p matrix. So, in this case, the product of a 2  1 matrix and
a 1  2 matrix yields a 2  2 matrix. In Dirac notation, we can express
the outer product above as j0ih0j. Likewise, we may construct the outer
products j0ih1j, j1ih0j, and j1ih1j. We leave it to you to compute these
in the following exercise: 11.170

Exercise

Find the outer products j0ih1j, j1ih0j, and j1ih1j.

To help you out, the first of these is:        1 10 11 0 1 0 1
D D j0ih1j WD 0 00 01 0 0

(11.171)

Hopefully, you’ve completed the rest! With the computation we completed
for you above and recalling how it is that we add two matrices, you can
now confirm a result written in chapter 3:   0 1 X WD j0ih1j C j1ih0j
D (11.172) 1 0 The outer product of two vectors is a specific case of
the more general concept of a tensor product, as we will see now. Before
we move on to the tensor product, we would like to discuss how the outer
product relates to Dirac notation. Recall that the inner product hujvi
of two vectors u and v is in fact expressible as u v, where u denotes
the conjugate transpose of u. It should not be too much of a surprise
then that the outer product juihvj is expressible as uv ! Exercise
Check that all of the above computations of outer products juihvj for
vectors u and v could have been thought of as computations of uv .

11.173

In summary:

SECTION 11.5 The Outer Product and the Tensor Product

273

Inner and Outer Product and Their Relationships with the Conjugate
Transpose

11.174

For any two vectors u and v, hujvi D u v and juihvj D uv

The Tensor Product Before introducing the operation of a tensor product,
let’s discuss some terminology for talking about tensor products. As we
have seen earlier, a scalar is simply a number. We can refer to scalars
as 0-tensors, meaning a tensor of order 0. Please note that we
discourage the use of the word “rank” when referring to the order of
tensors, as rank is a term reserved for another term in linear algebra.
We can refer to a vector as a 1-tensor. Similarly, we can refer to a
matrix as a 2-tensor. A 3-tensor would in fact be a rectangular prism of
numbers! Beyond the 3-tensor, we no longer have the ability to give a
geometric interpretation. However, many applications in the real world
call for tensors of higher order — sometimes in the thousands or
millions, as in the case of neural networks. We summarize this
terminology in Figure 11.15. 11.175 Exercise 11.15 is a 2-tensor?

Why is it appropriate to say that the table in Figure

Let us now return to our discussion of the tensor product as a
generalization of the outer product. The outer product is the product of
two 1-tensors, which produces a matrix (a 2-tensor). However, what
happens if we wish to take the tensor product of two tensors of any
arbitrary order? We can generalize the outer product of two 1-tensors to
the tensor product of any two tensors, A and B, of arbitrary order, like
so: A˝B   a To see what we mean by this, consider the two vectors u WD
and b  v WD c d e . Their tensor product is the matrix

274

CHAPTER 11 Mathematical Tools for Quantum Computing I

Tensors

Terminology

Example

0-tensor

scalar

3  1 0   1 1 1 p 2 1 1 

1-tensor

vector

2-tensor

matrix

Figure 11.15: Tensor terminology

 u˝vD

a b

 ˝

c d

e



 WD

ac ad bc bd

ae be

 (11.176)

This might remind you of the previously defined outer product of two
vectors, and it should, because the tensor product of the two vectors
here is the outer product. Let’s see the tensor product of two column
vectors: 0 1 r x B r y C 0 1 B C   r B sx C x C @ s A˝ WD B
(11.177) B sy C y C B t @ t x A t y You may have 0 read 1 earlier in
the book that we sometimes 0 1 write j00i to 1 0 B 0 C B 0 C C B C
denote the vector B @ 0 A, or j11i to denote the vector @ 0 A. We’d like
to 0 1 point out now that the notation j00i is shorthand for j0i ˝ j0i,
which is 0

 j00i WD j0i ˝ j0i D

1 0



 ˝

1 0



1 0 11 1 B 10 C B 0 C B DB @ 01 AD@ 0 00 0

1 C C (11.178) A

It should be noted that the tensor product cares about whether the
vectors are column vectors or row vectors, as we can see from
contrasting the previous two examples of tensor products. A quick
perusal of the previous examples should convince you that the tensor
product of a column vector with a row

275

SECTION 11.5 The Outer Product and the Tensor Product

vector yields a matrix, whereas the tensor product of two column vectors
yields another column vector. 11.179

Exercise

What do you think the tensor product of two row vectors

yields?

If you thought about the exercise above, you’re hopefully convinced that
the tensor product of two row vectors is another row vector. 11.180

Size of tensor product of matrices

The tensor product of an .a  b/ matrix with a .c  d / matrix is an .a
 c/  .b  d / matrix. Exercise Check that the aforementioned formula
for the dimension of the tensor product of an a  b matrix with a c  d
matrix specializes, as examples, to the following cases:  the tensor
product of two row vectors  the tensor product of two column vectors
Note that a row vector can be thought of as matrix whose dimensions are
1  m and a column vector can be thought of as a matrix whose dimensions
are n  1. 11.181

Now, we invite you to check that j11i is in fact j1i ˝ j1i, as claimed!
0

1 0 B 0 C C 11.182 Exercise Check that j11i WD j1i˝j1i is in fact the
vector B @ 0 A. 1 Then, check that the intermediate vectors are what
they’re supposed to be, i.e., 0 1 0 1 0 0 B 1 C B C C and j10i D B 0 C.
j01i D B @ 0 A @ 1 A 0 0

276

CHAPTER 11 Mathematical Tools for Quantum Computing I

We won’t dwell on the idea of the tensor product now. We’d just like to
introduce it and get you thinking about it. We’ll revisit this idea once
we’ve established the formal definition of vector spaces and linear
transformations between them. At that point, we’ll realize the tensor
product of two vectors is actually the tensor product of the two linear
transformations they represent. It will also become clear at that point
why it is that the dimension of the tensor product works the way it
does.

11.6

Set Theory

The Basics of Set Theory Now we’ll spend a bit of time developing some
of the prerequisite set theory necessary to continue with this chapter.
In particular, we’ll need to have an idea of what a function is (this
requires a bit of work!) and then we can ascertain what it means for a
function to be invertible. Invertible functions are of utmost importance
in quantum computing, since the quantum gates we use to construct
quantum circuits have to be reversible. The curious thing is that these
gates are represented by matrices, and we’ll learn that these matrices
are actually just representations of transformations of space, and so
are functions themselves. Once we believe that matrices are actually
just functions, we have a reasonable notion of what it means for a
matrix to be invertible, and thus for a quantum gate to be reversible!
So, don’t let the following passages discourage you. A firm mathematical
understanding of basic set theory and function theory will guide you
well on your way to grasping the underlying ideas of quantum computing.
First, we want to have a notation expressing the notion of the
containment of an element in a set. We say that x is an element of a set
S, and denote this by x 2 S. The symbol “2” resembles an “e” for
“element,” which might help us remember – some people like mnemonics. We
will often abbreviate the phrase “if and only if” with “iff.” So, any
time you see “iff,” think “if and only if.” We also often discuss the
notion of set containment, or set inclusion when doing mathematics, so
let’s make sure we have an idea of what this is. Given two sets A and B,
we say that A is a subset of B, denoted A  B, iff for all elements a 2
A, a 2 B. In other words, everything in A is also in B.

SECTION 11.6 Set Theory

277

Sometimes people indicate the inclusion of a set A into a set B by A ,!
B, and we say that “A includes into B.” Other ways to say this include
“A embeds into B” and “A injects into B.” The terminology “A injects
into B” is hinting at a property of functions called injectivity that
we’ll investigate soon. 11.183

Exercise

Check that f0g  f0; 1g.

We will find ourselves talking about a few important sets in this
chapter, so let us define them. The set of natural numbers,15 denoted N,
is N WD f0; 1; 2; 3; :::g

(11.184)

The set of integers,16 denoted Z, is Z WD f:::; 3; 2; 1; 0; 1; 2; 3;
:::g The set of rational numbers,17 denoted Q, is   p Q WD W p; q 2 Z;
q ¤ 0 q

(11.185)

(11.186)

The set of real numbers, denoted R, is a bit more complicated to define
formally, but it is acceptable to think of a real number as any number
that can be approximated to any level of precision by a sequence of
rational numbers. Examples of real numbers include 3 p 0; 1; 1; ; 2; e;
 4

(11.187)

Non-examples of real numbers include 15 Some

people prefer to define the natural numbers excluding 0, like so: N D
f1; 2; 3; :::g. It makes no difference, really, although computer
scientists are inclined to include 0. Some have suggested that the
symbol N be reserved for the set f1; 2; 3; :::g and that the symbol N0
be reserved for the set f0; 1; 2; 3; :::g. It is a good idea, but it has
not yet caught on as far as we know. 16 You are probably wondering why
the set of integers, beginning with the letter “i” is denoted with a
“z.” It turns out that the word “number” is “zahlen” in German, and the
Germans are responsible for much of the notation found in number theory
and algebra. 17 Can you figure out why the rational numbers are denoted
with a “q”? The root of the word “rational” is “ratio,” and another word
for ratio is “quotient”!

278

CHAPTER 11 Mathematical Tools for Quantum Computing I

i; 1 C i; 1

1 1 i; p C p i 2 2

(11.188)

By including the imaginary number i , we get the complex numbers,
denoted C. The set C is defined as C WD fa C bi W a; b 2 Rg

11.190

Exercise

(11.189)

Check the following set inclusions are actually true NZQRC

You might want to think of each integer x as the rational number x1 to
establish the second inclusion in the chain. Then, you might want to
think of each real number a as the complex number a C 0i to establish
the fourth inclusion.

We can also say things like “B contains A,” emphasizing B’s containment
of A rather than A’s containment in B. We will also begin to use
set-builder notation18 to express and describe sets. For example, we can
describe the set of all integers whose square is 1 with the notation S
WD fx 2 Z W x 2 D 1g (11.191) We read this as “The set of elements x in
the integers (recall, Z denotes the set of integers) such that the
square of x is 1.” So, the colon (:) indicates that we should say “such
that.” 11.192 Exercise How many elements are in the set S above? Can you
write in set-builder notation the set of all integers whose cube is 1?
How many elements are in that set?

Exercise Can you express the set of all complex numbers whose square is
1 in set-builder notation? What about the set of all complex numbers
whose fourth power is 1? The set of all complex numbers whose third
power is 1? How many are there of each? The answer to the third question
is not 1! Remember, you’re dealing with complex numbers. This

11.193

18 Note that this notation is also called a set comprehension, which is
the origin of the term of list comprehension in Python and other
high-level languages.

SECTION 11.6 Set Theory

279

is hinting at a classical theorem about the complex numbers known as De
Moivre’s theorem.19

The Cartesian Product In the development of the definition of vector
space, we’ll have a desire to understand the notion of a Cartesian
product of two sets. The idea is that if we have two sets, say S and T ,
we’d like to create one unified set from which each of S and T may be
identified unambiguously. We call this set the Cartesian product of the
sets S and T and denote it by S  T . The notation  was likely chosen
to remind us that the number of elements in the Cartesian product of S
and T is the number of elements of S times the number of elements of T .
Formally, the Cartesian product of the sets S and T is defined S  T WD
f.s; t / W s 2 S; t 2 T g

(11.194)

For example, if we take our two sets to be S D f1; 2; 3g and T D f4; 5g,
then, the Cartesian product of S and T is the new set S  T D f.s; t/ W
s 2 S; t 2 T g D f.1; 4/; .2; 4/; .3; 4/; .1; 5/; .2; 5/; .3; 5/g
(11.195) Notice that S  T has the promised 2  3 D 6 elements. 11.196
Exercise Think about what the Cartesian product of the set R with itself
is. We call this R2 , i.e., R2 WD R  R. Similarly, we say that C2 WD C
 C, and more generally, that Rn WD R :::  R „ ƒ‚ … n times

and Cn WD C :::  C „ ƒ‚ … n times

satisfying the equation z n D 1 for a natural number n form the vertices
of a regular n-gon in the complex plane. The n complex numbers
satisfying the equation z n D 1 are known as the nth roots of unity,
since 1 is also known as unity, and they are the nth roots of 1. For
example, the complex numbers satisfying the equation z 3 D 1 are the 3rd
roots of unity, and form an equilateral triangle in the complex p p 19
De Moivre’s theorem states that the complex numbers z

plane. Specifically, they are 1 D e 0 you can verify with Euler’s
formula!

2 3

;

1 2

C

3 2 i

D e 1

2 3

; and

1 2

3 2 i

D e 2

2 3

, as

280

CHAPTER 11 Mathematical Tools for Quantum Computing I

Relations and Functions Before we venture into the concept of a
function, we’ll want to discuss relations. The following discussion of
relations could accidentally convince you that relations are only
interesting in that they are a stepping stone on the path to the
definition of a function. This is far from the truth!20 Maybe you
remember writing and seeing things like f .x/ D x 2

(11.197)

while in school. People would say f .x/ is a function. What really is a
function though? Intuitively, a function is an unambiguous assignment of
each element of one set to an element of another set. Of course, we’ll
want to make this mathematically precise, since it is the backbone of
nearly all of the concepts that follow. Actually, we’ll learn soon that
matrices themselves are functions! Let’s look at some examples and
non-examples of functions to get an idea of what they are. Consider the
sets X WD f1; 2g and Y WD f3; 4g. We can assign each element of X to an
element of Y like so 1 7! 3 2 7! 4 Introducing notation, we denote the
assignment described above by the letter f (for “function”) and write f
WX !Y to indicate that f assigns elements of X to elements of Y . We
sometimes say “f maps X to Y ” as well. We refer to the set X as the
domain of the function f and to the set Y as the codomain (sometimes
called the “range”) of f . We can concisely describe the assignment
above with the notation 20 Curious readers should investigate category
theory, where the category of sets and relations,

denoted Rel, is an interesting mathematical object in its own right and
enjoys an intimate connection with the category of finite-dimensional
Hilbert spaces, denoted Hilb. For example, every relation R  X  Y of
finite sets is naturally associated to a matrix Rij , where Rij D 1 iff
.xi ; yj / 2 R and is 0 otherwise. Viewing these matrices as having
coefficients in the complex numbers C leads to an interpretation of a
relation as a linear transformation between finite-dimensional Hilbert
spaces. Category theory offers an enticing framework for computing and
other sciences. To learn more about category theory as a unifying
language for all of mathematics and science (and even understanding
language!), check out Tai-Danae Bradley’s blog Math3ma \[54\]. More
advanced readers might enjoy the n-Category CafKe.

SECTION 11.6 Set Theory

g.1/ D 3

and

g.2/ D 4

281

(11.198)

and say that “g assigns (i.e., maps) the element 1 to the element 3” and
that “g assigns (i.e., maps) the element 2 to the element 4.” Now, for a
non-example of a function. Let X and Y be the sets as before, but
consider instead the assignment, denoted by the letter h, described by 1
7! 3 1 7! 4 2 7! 3 Note that the symbol 7! denotes “is assigned to” or
“maps to.” What is strange is that 1 is now being assigned not only to
3, but also to 4. So, the rule of assignment given by h is ambiguous. It
is exactly this ambiguity that we seek to preclude in our formal
definition of a function. We won’t give the formal definition of a
function just yet though. We would like to emphasize that a function is
a special case of a more general phenomenon known as a relation. This
defers our discussion to that of relations. More precisely, we would
like to define the notion of a relation between two sets. The definition
of a relation is quite brief and might surprise you: 11.199

Definition Definition of a relation

A relation on two sets X and Y is a subset of their Cartesian product.
That’s all? Yes, that’s what a relation is. Let’s see a few examples of
relations to get an idea of what they are. Consider the subset R WD f.x;
x 2 / W x 2 Rg  R  R D R2

(11.200)

By definition, R is a relation, since it is a subset of the Cartesian
product R  R of the set of real numbers R with itself. But what is it?
The following are examples of points which are elements of R, as you
should check p .1; 1/; .2; 4/; .3; 9/; .4; 16/; .5; 25/; . 2; 2/; .; 
2 /; ::: (11.201)

282

CHAPTER 11 Mathematical Tools for Quantum Computing I

See what’s going on? These are not elements of R   p p 1 1 .0; 1/; .1;
2/; .e; /; .7; 89/; . 2; 3/; ; ::: 2 3

(11.202)

Notice that we say that a point is in the relation because we’re
indicating membership in the set defined by the relation. 11.203

Exercise

Plot the points of R2 in the relation R.

If you tried the above exercise, you see now that the set of points in
the relation R is a parabola! What is interesting about R is that it is
even better than a relation – it’s a function! In fact, you might
recognize it as being described compactly by the equation f .x/ D x 2 .
However, the equation f .x/ D x 2 hides so much of the character of the
function f that it’s virtually useless to say. To see what we mean by
this, first realize that to say f .x/ D x 2 gives no indication of the
domain or codomain of f . For all we know, f could be mapping from the
set C to f0; 1g or whichever pair of sets you like. In fact, if the
domain of f .x/ D x 2 is taken to be C and the codomain is taken to be
f0; 1g, f isn’t a function at all – we’ll see why when we give the
formal definition of a function! Exercise Check that the set f.0; 0/;
.1; 1/; .2; 2/; .3; 3/g  Z  Z is a relation. Can you describe this
relation using set-builder notation?

11.204

The point we’re trying to make is that we need to give the domain and
codomain when specifying a function, not just the rule of assignment.
For example: A function f from a set X to a set Y is a relation on X and
Y satisfying a special criterion... Before we give the special
criterion, a comment: Recall that to say that f is a relation on X and Y
is to say that f is a subset of the Cartesian product X  Y , so we can
reasonably talk about elements of the function (thus, relation) f . This
type of terminology may sound odd. You’ve likely not heard of someone
saying “.x; y/ is an element of the function f ” and

SECTION 11.6 Set Theory

283

are probably more accustomed to the phrase f .x/ D y. However, to say f
.x/ D y is literally to say that .x; y/ is in the function (and thus,
relation) f. After much deliberation, the special criterion that the
points .x; y/ in the relation f must satisfy is 11.205

Definition Definition of a function

A relation f on a Cartesian product X  Y of sets X and Y is a function
iff f satisfies for all .x1 ; y1 /; .x2 ; y2 / 2 f; x1 D x2 H) y1 D y2
The symbol H) denotes “implies.” In other words, if the first
coordinates are equal, then the second coordinates have to be equal! We
could also phrase this as for all x1 ; x2 2 X; x1 D x2 H) f .x1 / D f
.x2 / Let’s revisit the non-example we gave earlier and confirm that it
is not a function. Recall that we had defined a mapping h W f1; 2g ! f3;
4g earlier by the rule of assignment 1 7! 3 1 7! 4 2 7! 3 Let’s express
this as a relation. h is the relation h D f.1; 3/; .1; 4/; .2; 3/g  f1;
2g  f3; 4g

(11.206)

Exercise Use the definition of a function to check that h, as given, is
not a function. What rule of the definition of a function does it
violate? Next, recall that we claimed earlier that if we take the
mapping f .x/ D x 2 and assign its domain to be C and its codomain to be
the set f0; 1g, then f is not a function. Explain why this is true.
Hint: Think of f as a relation first – is it even a relation?

11.207

284

CHAPTER 11 Mathematical Tools for Quantum Computing I

Hopefully, you realized that h above is not a function because .1; 3/
and .1; 4/ are in h and yet despite the fact that their first
coordinates are equal (both equal 1), their second coordinates differ
(they’re each 3 and 4). This is exactly why h violates the definition of
a function. This example, when analyzed alongside the formal definition
of function we’ve given, hopefully illuminates exactly what type of
examples the definition is precluding. To request that if the first
coordinates of two points in a relation are equal that then their second
coordinates must be equal is essentially to ask that no element in the
domain is mapped by f to more than one element in the codomain. In other
words, the assignment that describes f should be unambiguous. Let’s turn
our attention to the second part of the exercise. If we insist that the
domain of the mapping f .x/ D x 2 is truly all of C and not any proper
subset, then we see that there exists an element in the domain of f
whose image under f is not an element of f0; 1g, e.g. x D 2, because if
x D 2, then f .x/ D f .2/ D 22 D 4 … f0; 1g. So, the codomain cannot be
just f0; 1g and would have to be expanded to accommodate all of the
potential images of elements of C under f . Then, the codomain would
have to be taken be all of C! A clever way of dealing with this issue is
to “restrict the domain” of f . By this we mean, instead of taking the
domain of the function f to be all of C, take it instead to be the
subset of C consisting only of complex numbers whose squares are in f0;
1g, i.e. f 1; 0; 1g. Making this restriction of the domain from C to f
1; 0; 1g ensures that each element in the domain maps to an element in
the codomain f0; 1g, solving the previously discussed issue. So, you
could take f to be the relation f WD f. 1; 1/; .0; 0/; .1; 1/g  C  f0;
1g

(11.208)

Then, f is in fact a relation on C  f0; 1g as per our definition, and
it is also a function on C  f0; 1g as per our definition. Some might
argue that this new f that we’ve constructed in an effort to remedy the
problem about the codomain f0; 1g not being large enough to accommodate
all possible images of elements of C under f is not really the f given
at the outset. If we were to take the set of inputs to just be f 1; 0;
1g all along and not actually consider all of C, then why wouldn’t we
just say so originally? People do this occasionally, i.e. state a domain
that is larger than what is actually intended. A relation of this sort
is known in the literature as a “partial

SECTION 11.6 Set Theory

285

function.” As we do not have necessity to develop this concept here, we
will encourage interested readers to check this out on their own. The
curious reader might wonder why we restrict our focus to functions and
seldom mention relations. A quick answer is that relations are such a
broad class of objects that it’s difficult to classify and study them at
all. This is not to say that they aren’t interesting, just to say that
the theory for functions is better understood. Exercise of assignment

11.209

Consider the function f W R ! R described by the rule f .x/ WD x 2

We are inclined to say that the inverse function of f is the function p
f 1 .x/ WD x Ah, but if f 1 is to be a function, it has to have a
specified domain and codomain! What are its domain and codomain?
Describe the relation that the rule of assignment describing f 1 defines
after finding the domain and codomain. Is it even a function?

This exercise likely confused you, and rightly so! What is confusing is
that trying to formulate an inverse for the function f W R ! R defined
by f .x/ D x 2 demands a bit more care. To see what goes wrong, observe
that f maps two different elements of the domain R to the same element
of the codomain R: f .1/ D 12 D 1 (11.210) f . 1/ D . 1/2 D 1

(11.211)

So, in the process of “inverting” f (which we may think of as “undoing”
the squaring operation), we’ll have to determine what to do with the
number 1 in the codomain. In other words, the question of “Who in the
domain did f map to the number 1 in the codomain?” is ambiguous, since
both 1 and 1 get mapped to 1 by f . You could answer with either 1 or 1
and you’d be correct! Do you recall now why taking square roots demands
that we include “plus or minus”? It’s not just dogma! This phenomenon
manifests itself geometrically as the failure of the parabola (the graph
of f ) to pass the “horizontal line test” as you’re invited to explore
in the next exercise...

286

CHAPTER 11 Mathematical Tools for Quantum Computing I

Exercise Draw the graph of the function f and check that it is in fact a
parabola. Having done so, see that any horizontal line drawn above the
x-axis hits the curve twice. In particular, find the geometric
manifestation of the fact that f .1/ D 1 and f . 1/ D 1 by drawing a
horizontal line at height 1 on your plot. 11.212

Exercise You might be wondering now “But wait – then, f isn’t even a
function because it sends two different things to the same place!”
Careful, f is a function. The definition of a function disallows the
possibility that one thing map to two different things, which is
different from what is going on here. Check this using the formal
definition of a function!

11.213

We’ll see that if we impose a condition on the functions that we
consider, we’ll never encounter this problem while trying to invert
them. You can probably already guess that we will require that our
functions do not map two different things to the same thing in what
follows. From now on, we’ll revert to our usual notation for functions
and will likely not need to mention relations. We simply wanted to
emphasize the idea that a function is just a specific kind of relation,
which instructs its precise mathematical definition.

Important Properties of Functions We now describe three desirable
attributes of functions:21 injectivity, surjectivity, bijectivity We
grappled with the idea of a non-injective function earlier while
discussing the parabola. Intuitively, an injective function is a
function that never maps two different things to the same thing. You
might know this by the name one-to-one. 21 The

terminology injective, surjective and bijective can be traced back to
Nicolas Bourbaki, the pseudonym of a secret society of mainly French
mathematicians, including André Weil, Jean-Pierre Serre and Alexander
Grothendieck, who sought out to reformulate mathematics on an abstract,
yet self-contained basis around 1935.

SECTION 11.6 Set Theory

11.214

287

Definition Injective function

A function f W X ! Y is injective iff for all x1 ; x2 2 X; f .x1 / D f
.x2 / H) x1 D x2 : In other words, we ask that f maps two elements to
the same element only if those elements are equal. You should check that
the function f W R ! R defined by f .x/ D x 2 earlier is not injective,
despite being a function. Exercise Prove that if a function f is
injective, then for all x1 ; x2 2 X, f .x1 / D f .x2 / iff x1 D x2 .
Recall the definition of a function!

11.215

Sure, f W R ! R defined by f .x/ D x 2 is not injective. However, if we
restrict the domain of f to the smaller set Œ0; 1/ WD fx 2 R W x  0g
and consider instead the function f jŒ0;1/ W Œ0; 1/ ! R

(11.216)

(read this “the restriction of f to the set Œ0; 1/”), we realize that f
jŒ0;1/ is suddenly injective! Geometrically, this corresponds to
chopping off the left side of the parabola and considering only the
right side. Graph this to see what we mean. We can express this by
saying that we’re only considering a single “branch.” Now, let’s try to
invert this new restricted version of f . Having attempted a previous
exercise, you might have struggled to determine the domain and codomain
for the inverse function, which we at least know should be somep thing
like x. Since the restriction f jŒ0;1/ W Œ0; 1/ ! R is a function from
the domain Œ0; 1/ to the codomain R, it seems reasonable to request that
the inverse function have opposite domain and codomain, i.e., that the
domain  1 of the inverse function f jŒ0;1/ should be R and the codomain
should be Œ0; 1/.  1 p No worries about the codomain: the inverse f
jŒ0;1/ D x certainly has codomain Œ0; 1/ since the square root of any
real number is either 0 or positive, i.e., is an element of the set Œ0;
1/, as you should check. However, we have an interesting dilemma arising
from the issue of what the domain should be. As you may have already
noticed, we cannot take the domain of

288

CHAPTER 11 Mathematical Tools for Quantum Computing I

f jŒ0;1/



1

D

p

x

(11.217)  1

to be all of R. If we did, we would have to declare how it is that f
jŒ0;1/ operates on numbers like 1... In other words, we would have to
take the square root of 1 (and all of the other negative numbers!),
which would take us into the imaginary domain. Since there is no real
number whose square is 1, we’ll have to restrict  1 p the domain of the
inverse function f jŒ0;1/ D x just as well, or else the inverse won’t be
a function as per our previous definition! Specifically, we   1 p
remedy our problem of inverting f jŒ0;1/ by restricting f jŒ0;1/ D x
only to the non-negative numbers, i.e., Œ0; 1/. In other words, we
needed for the function to map onto every element of the codomain. In
this particular example, we see that the function f .x/ D x 2 and even
its restriction f jŒ0;1/ to Œ0; 1/ does not “hit” everything on the
other side. For instance, it misses the number 1, since there is no real
number whose square is 1. You can see this geometrically by recognizing
that the parabola, and even its right-hand branch, do not ever encroach
into negative territory. We now state a definition clarifying all of
this discussion and giving a precise mathematical meaning to the word
onto. 11.218

Definition Surjective function

A function f W X ! Y is surjective iff for each element y 2 Y there
exists an element x 2 X such that f .x/ D y. Colloquially, we could say
that every element in Y is “hit” by some element of X . Now, the
punchline. We set out to make the idea of a function precise and then to
give attributes of a function, but we never stated explicitly why we
care about these attributes. This next definition is truly a theorem,
but we state it as a definition: 11.219

Definition Bijective function

A function f W X ! Y is bijective, equivalently, invertible by a
function f 1 W Y ! X, iff f is injective and surjective. So, now we know
that a function is invertible by another function precisely when f is
bijective. Invertible functions play an important role in defining what
it means for two mathematical objects to be the same. For example, for

SECTION 11.6 Set Theory

289

most purposes, it is often sufficient to consider two sets to be the
same iff they have the same number of elements. One way of expressing
that two sets have the same number of elements is by stating that there
exists an invertible function between them (think about why!). If the
sets that we’re interested in happen to have a bit more structure and
we’d like to assign a meaning to the statement that they’re the same, it
seems only natural to request that there be an invertible function
between them that preserves their structure, i.e., it is not sufficient
only to have a bijective map between the sets. We’ll see later that this
idea of a structure-preserving map manifests itself in linear algebra as
an invertible linear transformation. A few comments: If f is not
injective, it is fair to restrict the domain of the function to impose
injectivity on it, as we did above with the function f W R ! R defined
by f .x/ D x 2 . But then the function might not be surjective, so we
have to invert the function f only on its image, where by the image of f
we mean f .X / WD ff .x/ W x 2 X g; (11.220) i.e., the elements f .x/ 2
Y for some x 2 X. If we don’t invert the function only on its image, the
inverse we desire might not end up being a function, as was the case for
the squaring function and its presumed inverse, the square root!
Exercise You should check that the image of the squaring function f W R
! R defined by f .x/ D x 2 is in fact Œ0; 1/.

11.221

For a moment, let’s recall how it is that we compose two functions. If
you have two functions, say f W R ! R defined via f .x/ D x 2

(11.222)

g W R ! R defined via g.x/ D x C 1;

(11.223)

and it’s natural to ask what their composition is, i.e., the result of
applying them iteratively. 11.224

Definition The composition of two functions

In general, we define the composition of two functions f WX !Y

and

gWY !Z

to be the function .g ı f / W X ! Z defined via g.f .x//.

290

CHAPTER 11 Mathematical Tools for Quantum Computing I

So, you apply g first, then f . In the case we have above, the
composition of f .x/ D x 2 and g.x/ D x C 1 is the function .f ı g/.x/
WD f .g.x// D f .x C 1/ D .x C 1/2

11.226

Exercise

(11.225)

Check to see that g ı f is not the same function and is

in fact .g ı f /.x/ D x 2 C 1

In general, it’s quite rare that f ı g D g ı f for two functions f and
g. For any set X, there is a special function called the identity
function, denoted IX such that for all x 2 X, IX .x/ D x. Given a
function f W X ! Y , it’s natural to ask if there is another function f
1 W Y ! X such that the following two properties hold: (1) f 1 ı f W X !
Y ! X is equal to the identity function IX on X and (2) f ı f 1 W Y ! X
! Y is the identity function IY on Y . If we can find such a function f
1 , we say that we have found an inverse function for the function f .
Now, we have a more refined notion of an invertible function: 11.227

Characterization of invertible functions

A function f W X ! Y is invertible iff there exists a function f 1 W Y !
X such that f 1 ı f D IX (11.228) and f ıf

1

D IY

(11.229)

That is, f is invertible iff we can find a function f 1 whose
composition with f in either order yields the identity function! This
idea will manifest itself later in our discussion of matrices, when we
discuss what it means for a matrix to be invertible.

SECTION 11.7 The Definition of a Linear Transformation

11.7

291

The Definition of a Linear Transformation

You might have wondered since the beginning of this chapter why it is
that we call linear algebra “linear algebra.” So far, it’s likely not
clear at all, since we have not discussed lines or anything obviously
linear in any sense. Interestingly, the matrices that have occupied our
previous discussion are in fact what we refer to as linear
transformations. This demands some explanation. So, what is a linear
transformation then? The next (non)example might startle you... Consider
the function (transformation) T from R ! R described by x 7! x C 1

(11.230)

In words, T is the transformation of 1-dimensional space that maps a
vector (a number, in this case) to that vector plus one. For example, T
.0/ D 0C1 D 1 and T .1/ D 1 C 1 D 2. Those familiar with function
notation might describe the transformation T as T WR!R (11.231) T .x/ D
x C 1

(11.232)

and draw its graph as in Figure 11.16 Well, you might say, “Then T is
obviously linear – it’s a line!” Ah, but it’s not actually! In fact, the
relation above is affine, not linear.22 The reason why this example goes
against our intuition is because we have been trained to analyze the
graph of a function. Typically, the information encoded by the graph of
a function guides our intuition. However, in this case, the graph of T
is the set of points f.x; T .x// W x 2 Rg

(11.233)

which does indeed resemble a line when plotted. However, we are not
asking that the graph of the function be a line – we’re asking that the
function 22 An

affine transformation is a transformation of the form Ax WD T x C b,
where T is a linear transformation and b is a vector. In other words, an
affine transformation is the result of a linear transformation (i.e., a
composition of rotations and dilations) and then a translation. In fact,
the reason the transformation T .x/ WD x C 1 is not linear is because it
translates by 1! It’s a good exercise to determine exactly what A and b
are in the definition of T f and to realize that an affine
transformation is linear exactly when the translation vector b is zero.

292

CHAPTER 11 Mathematical Tools for Quantum Computing I

y T .x/ D x C 1

x

Figure 11.16: The graph of T .x/ D x C 1

itself be linear! You might want to revisit this example after learning
the definition of a vector space to see if you can find more reason for
why this should not be included in our set of linear functions. Try to
wrap your head around this for a moment (or three). Here is the
definition of linear that we will take, at least for the case of a
transformation that maps from R to R: 11.234

Definition The definition of a linear transformation

A transformation T W R ! R (interchangeably, function) is linear iff 1.
for all x; y 2 R, T .x C y/ D T .x/ C T .y/ 2. for all a 2 R and for all
x 2 R, T .a  x/ D a  T .x/ So, we’re requiring that applying T to a
sum is the same as applying T to each of the summands and then summing,
and that applying T to a scalar multiple is the same as applying T to
the multiplicand and then multiplying the result by the scalar. In other
words, we require that T preserve addition and scalar multiplication.
Often people will say things like structure-preserving map. By
structure, they mean algebraic structure, i.e., the way things are added
and multiplied.

SECTION 11.8 How to Build a Vector Space From Scratch

293

Let’s see why the previously defined map T .x/ D x C 1 is not linear. If
T were linear, it would be the case that for all x and y in R, T .x C y/
D T .x/ C T .y/. We see, however, that this is not true: T .x C y/ WD .x
C y/ C 1

(11.235)

and T .x/ C T .y/ WD .x C 1/ C .y C 1/ D .x C y/ C 2 ¤ .x C y/ C 1
(11.236) So, T .x C y/ ¤ T .x/ C T .y/ in general, and so T does not
satisfy our definition of linear! Exercise Check that T also violates
the second property specified in the definition of linear with a
specific choice of a and x in R. So, T is hopelessly not linear!

11.237

We still claim that the matrices shown earlier are in fact linear
transformations. However, to explain this correctly, we’ll need to
understand in what sense a matrix is a transformation from a more
careful and mathematical perspective. In particular, we’ll need to turn
our attention toward exactly which spaces the matrices are transforming.
These spaces are known as vector spaces.

11.8

How to Build a Vector Space From Scratch

The name vector space likely brings to mind a space of vectors. That is
pretty much what a vector space is – a space where a bunch of vectors
live. We want this space to facilitate all of the usual operations we
perform on vectors, such as addition of vectors and scalar
multiplication of vectors. We’ll state the precise definition of a
vector space and then unpack the terminology. 11.238

Definition Vector space

A vector space V over a field F is an abelian group V equipped with an
action of the field F on V .

294

CHAPTER 11 Mathematical Tools for Quantum Computing I

There are a lot of unfamiliar terms in this definition which we will
explain step by step. First of all, what is a field? It turns out that
it will be best to define an abelian group first, since we’ll see that
any field is an augmentation of an abelian group. Later on in this
section we will define the word action.

Groups Recall that the notation x2G

(11.239)

denotes “x is an element of G.” We also write things like x; y; z 2 G

(11.240)

meaning “x; y and z are elements of G.” We’ll state the definition of a
group precisely now. After its statement, we’ll delve into what all of
this really means. A group .G; ?/ is a set G satisfying the following
properties:  Closure: There exists a function ?WGG !G which we call
the binary operation of G. Instead of writing the application of the
operation ? to a pair of elements g1 ; g2 each in G as ?.g1 ; g2 /, as
we usually do when describing the application of a function to a pair of
elements, we write g1 ? g2 to be succinct. For now, it’s advisable to
think of ? as being a familiar operation like addition or
multiplication. For example, it would be weird, but correct, to say that
addition is a binary operation that accepts two numbers as the input and
outputs a new number. We could write such a thing like this, where we
replace the name ? for the binary operation with the symbol C C.x; y/ WD
x C y: This idea shouldn’t be too unfamiliar to computer scientists and
programmers – it’s like defining a function or method!

SECTION 11.8 How to Build a Vector Space From Scratch

295

 Associativity: For any triplet x; y; z of elements of G, .x ? y/ ? z D
x ? .y ? z/ This is a reasonable assumption that we often make in
mathematics. You should be aware of the fact that not every binary
operation is associative! Exercise Can you think of an example of a
binary operation that isn’t associative? Think of the usual subtraction
of two numbers, e.g., 3 2 D 1. Interestingly, this simple operation is
not associative! To see this, consider the ambiguous difference 1 2 3.
Is it .1 2/ 3 or is it 1 .2 3/? Check to see that it does matter!

11.241

 Identity: There exists an element e 2 G, called the identity element
such that for any element x 2 G, x?e De?x Dx Again, it’s advisable to
think of a familiar scenario: you’re likely already familiar with the
number 0 in the integers equipped with the operation of addition.
Exercise You should check that 0 has the identity property for any set
of numbers equipped with addition, i.e., adding any number x and zero in
either order yields the number x.

11.242

 Inverse: For each element x 2 G, there exists an inverse element x 1 2
G, with the property that x?x

1

Dx

1

?x De

Inverses in any set of numbers equipped with the operation of addition
are the “negatives.” To see what we mean, try to find a number such that
when you add it to 1 on either side, you get 0. A moment’s thought makes
us realize that the number we’re looking for is 1! So, we would say that
1 is the inverse of the number 1 with respect to addition.

296

CHAPTER 11 Mathematical Tools for Quantum Computing I

11.243

Definition The definition of a group

A group .G; ?/ is a set G satisfying the following properties: 
Closure: There exists a function ? W G  G ! G; which we call the binary
operation of G.  Associativity: For any triplet x; y; z of elements of
G, .x ? y/ ? z D x ? .y ? z/  Identity: There exists an element e 2 G,
called the identity element of G, such that for any element x 2 G, x?e
De?x Dx  Inverse: For each element x 2 G, there exists an inverse
element x 1 2 G, with the property that x?x

1

Dx

1

?x De

Now, let’s regroup (sorry, intended...) and think about what this
definition really says. The idea of a group is simple. We begin with a
set of things. Then, we define a single binary operation on that set of
things, i.e., an operation that accepts two inputs from your set of
things and produces another thing in your set. This property is also
known as closure of the set under the operation. Next, we require that
the operation be associative. So, if we have three things to operate on,
we may operate on any two first, and then the third (you can’t operate
on all three at once because you started with a binary operation!).
Afterward, we require that there be a special element in our set called
the identity element. If we apply the binary operation to this special
element and any other element, we get that element back. Finally, we ask
that each element in our set have an inverse element, also in the set,
so that when we apply the binary operation to that element and its
inverse element (in either way), we get the identity element. To make
the group abelian,23 we ask that the operation be commutative, in the
sense that the operation yields the same result regardless of the order.
23 The

name “abelian” honors the mathematician Niels Henrik Abel.

SECTION 11.8 How to Build a Vector Space From Scratch

11.244

297

Definition Abelian group

A group .G; ?/ is called abelian iff ? is a commutative operation, i.e.,
for all x; y 2 G; x ? y D y ? x This definition is fairly abstract, so
let’s pin it down with an example: the integers, denoted Z. This example
will hopefully solidify a few of the remarks made during the course of
the definition. The integers Z are the numbers Z WD f:::; 3; 2; 1; 0; 1;
2; 3; :::g

(11.245)

There is a natural choice of binary operation ? W Z  Z ! Z. It’s
addition! We define ?.x; y/ WD x C y (we saw this earlier when
explaining the meaning of a binary operation). In other words, ? is just
the binary operation of usual integer addition. Then the claim is that
this operation does in fact satisfy all of the other properties listed.
Well, associativity is certainly satisfied, since addition of integers
is associative (although some might take issue with this, since in some
sense associativity is satisfied by fiat). For example, if asked to find
the sum 1 C 2 C 3, we know that we may either compute 1 C 2 first, then
add 3, or compute 2 C 3 first, then add 1. In symbols, .1 C 2/ C 3 D 1 C
.2 C 3/, and in fact, this is true for all triplets of integers. The
next question is as to what the identity element is here. The answer is
0 because adding 0 and any other integer yields that integer. Finally,
we ask that every integer have an inverse, and this is true, since any
integer a has inverse a. Check that for any integer a 2 Z, a C . a/ D .
a/ C a D 0 11.247

Exercise

(11.246)

Try to figure out why the set of natural numbers N WD f0; 1; 2; 3; :::g

(11.248)

is not a group with the operation of usual addition of natural numbers,
e.g., 1 C 2 D 3.

In any case, it turns out that the rational numbers (Q), the real
numbers (R) and the complex numbers (C) each form abelian groups under
usual addition of numbers.

298

CHAPTER 11 Mathematical Tools for Quantum Computing I

Now, we have the following observation: Key idea

11.249

Vectors of numbers form an abelian group! To see what we mean, let’s
revisit our definition of the addition of two vectors. Let’s focus on
what happens in two dimensions. In fact, let’s check to see that the set
of all vectors with two complex components, denoted    x 2 V D C WD
W x; y 2 C (11.250) y does in fact form an abelian group under usual
vector addition. First, we need to verify that this set is closed with
respect to the operation of vector addition, i.e., if we take two
elements of this set and we add them, T that we do in fact get another
element of this set (closure). So, let x y T and z w be any two
elements in the set V . We need to check that their sum       x z
xCz C D (11.251) y w yCw is in fact another element of the set V . Since
each of x; y; z; w are complex numbers, the sums x C z and y C w are in
fact complex numbers too. So, the resulting vector is an element of V
after all. Then, V is closed with respect to vector addition. The next
question is as to whether this addition is associative. You’re invited
to check this and we’ll set it up for you. Let       a c e ; ;
(11.252) b d f be elements of V . 11.253



Exercise a b



 C

Check the associativity of vector addition, i.e., that c d



 C

e f



 D

a b



 C

c d



 C

e f



SECTION 11.8 How to Build a Vector Space From Scratch

299

So now we need an identity element. We can take the vector that has only
zero entries  eD

0 0

 (11.254)

Exercise Check that the vector e is in fact an identity element for the
set V , i.e., adding e to any vector on either side yields the same
vector.

11.255

We then ask whether any given vector in V has an inverse element in V
with respect to addition. This isn’t too bad. If we’re given a vector T
T x y v WD x y in V , the inverse element is v WD , as you might have
expected. 11.256

Exercise

Check to see that it is in fact the case that v C . v/ D . v/ C v D e

(Remember that “e” is the all-zero vector defined above!)

Now, what about the abelian part? Let us recall that abelian refers to
commutativity, so let’s see if the group of vectors has commutativity
for the operation of addition. Exercise You should check that adding
vectors in V in either order yields the same result, i.e., that they
commute.

11.257



a b

     c e ; ; d f

(11.258)

This is true due to the fact that adding complex numbers in either order
yields the same result, as you’ll see while completing this exercise.

We have now verified that C2 , the set of all two-dimensional vectors
with complex entries is an abelian group!

300

CHAPTER 11 Mathematical Tools for Quantum Computing I

Exercise Prove that R2 is an abelian group by similar means. Then, prove
that the n-dimensional analogue Rn is also a group. Last, prove the
n-dimensional analogue Cn of C2 is also an abelian group with respect to
usual vector addition. 11.259

A comment about notation: After assuming the group is abelian, it’s fair
to revert to calling the abstract operation ? by the name C. This is
because the binary operation for every abelian group can be realized as
some sort of addition of integers! We won’t have time to discuss this
idea here, however. The inverse of an element x in the abelian group
setting is thus fairly referred to by x. Exercise To see an example of a
non-abelian group, consider the Pauli matrices X; Y; Z from earlier, and
the identity matrix I WD I2 . Check that the set of sixteen matrices

11.260

P WD f˙I; ˙iI; ˙X; ˙iX; ˙Y; ˙iY; ˙Z; ˙iZg equipped with the operation of
matrix multiplication is a group by verifying the axioms listed above.
We call this group the Pauli group. It is non-abelian because the matrix
product is not commutative in general. For example, XY ¤ YX .

You should now be wondering what we mean by an action of a field F on V
, and in particular, what a field is. We can jump directly from abelian
groups to fields, but we might as well take a more leisurely route and
visit the notion of a ring along the way. We’ll save the idea of an
action for last.

Rings A ring is an abelian group with an additional operation, which is
often called “multiplication,” that satisfies some additional
conditions. Rings are not too abstract, actually. You’ve been working
with rings all of your life! Examples include the integers, Z, rational
numbers Q, the real numbers R, the complex numbers C, and more exotic
finite rings like Z=2Z D f0; 1g equipped with addition and
multiplication modulo 2 (also known as F2 ), as we will see. In fact,
most of these rings turn out to be fields.

SECTION 11.8 How to Build a Vector Space From Scratch

301

More formally, a ring R is an abelian group (so, it’s a set satisfying
all of the properties of an abelian group defined earlier – review
these!), where we denote the commutative binary operation playing the
role of addition by C, equipped with an additional binary operation,
denoted by by , playing the role of multiplication, and satisfying the
following properties:  Closure: There exists a binary operation WRR
!R additional to C, which we usually call multiplication. Similar to the
scenario with groups, we often write the application of  to a pair of
elements .x; y/ of R as x  y as opposed to .x; y/. As before, you’re
advised to think of usual multiplication of numbers as you read through
these axioms. For example, the rational numbers Q (all ratios of
integers, i.e., fractions) are closed under usual multiplication.
Exercise

Verify that the rational numbers na o Q WD W a; b 2 Z; b ¤ 0 b are in
fact closed under usual multiplication. So, let a c ; 2Q b d (so, a; b;
c; d 2 Z) and check that their product a c ac  WD b d bd is actually
another rational number. This amounts to confirming the numerator and
denominator of the result are each integers and that the product of two
integers is an integer (which might even be considered defining
properties of the integers!). 11.261

We also want for this multiplication to be associative so that
multiplying “three things at once” is well-defined. To see what we mean
by this, we dare you to multiply 3 numbers at once, e.g. 2  3  4.
Pause for a moment and try to genuinely multiply all 3 numbers at once,
i.e. no “cheating” by multiplying two of them, and then proceeding from
there. Give up? Given a product of 3 numbers, e.g. 2  3  4, we must
compute their product by either associating 2 and 3, computing their
product: 2  3 D 6, and then associating this with 4 afterward or by
associating 3 and 4 first, computing

302

CHAPTER 11 Mathematical Tools for Quantum Computing I

their product: 12, and then associating this with 2. The fact that we
can compute this product in either way and get the same result is the
miracle of associativity of multiplication of numbers. Here is the
formal axiom requesting associativity:  Associativity: For all x; y; z
in R, .x  y/  z D x  .y  z/ This is similar to the axiom for groups,
but we’d like it to be true for multiplication. Exercise Verify that
multiplication of rational numbers is associative. So, take three
arbitrary rational numbers, say a c e ; ; 2Q b d f

11.262

and show that

a

c e a   D  b d f b



c e  d f



This will amount to the fact that integer multiplication is associative!
In usual arithmetic, we are familiar with the idea that we may
distribute multiplication “over” addition. So, we also require an axiom
of distributivity:  Distributivity: For all x; y; z 2 R x  .y C z/ D x
 y C x  z Also, .y C z/  x D y  x C z  x This is a bit subtle. We
want the distributivity to “work” on both sides. We won’t dwell on it
though.24 Exercise Verify that multiplication of rational numbers does
in fact distribute over addition. So, take three rational numbers, say

11.263

a c e ; ; b d f 24 Technically,

we could request the axiom of distributivity before the axiom of
commutativity, or even request the axiom of distributivity and not the
axiom of commutativity. Do you see that if we request the axiom of
distributivity and not the axiom of commutativity that we really need
both equalities in the axiom of distributivity?

SECTION 11.8 How to Build a Vector Space From Scratch

303

and show that: a  b



c e C d f

 D

a c a e  C  b d b f

Fortunately, the multiplication of rational numbers is commutative, so
there’s no need to verify the distributive property “on the other side”.
You can if you want to practice, however! We’ll get you started: Realize
that because we are verifying the distributivity of multiplication,
we’re not yet allowed to use it. So, we have to first add the two
parenthesized rational numbers (by giving the common denominator of df
and get a single rational number, like so: c e c e c1 e1 c 1 e 1 c f e
d C D C D C D  C  D  C  d f d f d 1 f 1 d 1 f 1 d f f d
Continuing... D

cf ed cf ed cf Ced C D C D d f f d d f d f d f

So, we may now freely multiply this result (sum of dc and fe by ab . Go
ahead and do this and see what you get. Then, perform the addition on
the right-hand side and see what you get. Are these the same? It might
surprise you how much work goes into verifying something as seemingly
simple as this! So, a ring is an abelian group (and therefore comes
equipped with a binary operation which is fairly called “addition”)
equipped with another binary operation, called “multiplication,” which
is associative and satisfies a distributive law compatible with addition
(on both the right and the left). Most rings of interest also come with
a special element called the (multiplicative) identity element that
“preserves the identity” of the elements that it multiplies. For
example, you will be able to verify for yourself shortly that the
(multiplicative) identity element in each of the rings Z; Q; R; and C is
in fact simply the number 1, as we would hope. This (multiplicative)
identity element is almost always different from the (additive) identity
element that the underlying abelian group of the ring already came with.
To see this, notice that the underlying abelian groups of each of the
rings Z; Q; R; and C has (additive) identity element 0, which is
drastically different from 1. A ring

304

CHAPTER 11 Mathematical Tools for Quantum Computing I

equipped with a (multiplicative) identity element is known as a ring
with unity, where “unity” is meant to evoke the notion of the number 1,
which it often is. Here is the axiom requesting the existence of a
multiplicative identity element:  Identity: There exists an element,
denoted by 1, in R such that for any element x in R, 1x Dx1Dx
Equationally, this is strikingly similar to the group property. The
identity element of a field is often literally the number 1, as opposed
to e or 0, however. Notice that we haven’t yet required multiplication
to be commutative, so it is truly necessary to request that the
multiplicative identity “works” on both sides. Exercise Verify that the
set of 2  3 matrices with integer entries is in fact a ring, i.e. is an
abelian group (what should be the binary operation likened to “addition”
be?) equipped with the additional binary operation of matrix
multiplication satisfying: closure, associativity, and distributivity.
Is there an identity element (as per our stringent axiom above) in this
ring? If you think so, discover it, and prove that it really is an
identity element. If you think not, prove that there cannot be an
identity element in this ring. 11.264

Many rings of interest are even better: they are commutative, i.e. their
multiplication enjoys a commutative property, as in the case of abelian
groups. In fact, almost of the examples above, e.g. Z; Q; R; and C, are
commutative rings. The example in the exercise above consisting of
matrices is a noncommutative ring. Nearly all rings of matrices are not
commutative. Once we show that matrix multiplication corresponds to
composition of linear transformations (which are themselves functions),
that matrix multiplication is not commutative is quite believable. Here
is the axiom requesting that multiplication be commutative: 
Commutativity: For all x; y 2 R, xy Dyx So, multiplication in either
order should yield the same product. Exercise Verify for yourself that
the following set of matrices surprisingly constitutes a commutative
ring with unity:

11.265

SECTION 11.8 How to Build a Vector Space From Scratch



1 0 0 1

  0 ; 1

1 0

  ;

1 0

0 1

305

   0 1 ; 1 0

Figure out the relationship between this ring of matrices and the
following ring: Z=4Z equipped with addition modulo 4 and multiplication
modulo 4. Are they “the same”? Rings which enjoy a multiplicative
identity and whose multiplication is commutative are called commutative
rings with unity. It turns out a field can be obtained from a
commutative ring with unity by simply requiring one more axiom: that
each nonzero element admits a multiplicative inverse in the ring. We’ll
see this in what follows.

Fields A field F is a commutative ring with unity (so, an abelian group
with an additional binary operation satisfying all of the axioms above –
review these carefully!), where we denote the binary operation of the
underlying abelian group by C and the binary operation of multiplication
by , satisfying the following salient property that requires each
nonzero element to have a multiplicative inverse:  Inverse: For each
nonzero element x 2 F, there exists an element x 1 in F such that xx 1
Dx 1x D1 25

We are finally able to state the definition of a field once and for all:
11.266

Definition The definition of a field

A field is a commutative ring with unity satisfying the additional axiom
that for each nonzero element x 2 F, there exists an element x 1 in F
such that xx 1 Dx 1x D1 25 If

we demand all of the axioms of a field except for the commutativity
axiom, we have what is referred to as a division ring. The quaternions
are a famous example (especially in physics!) of a division ring, i.e. a
non-commutative ring with unity and where each nonzero element has a
multiplicative inverse.

306

CHAPTER 11 Mathematical Tools for Quantum Computing I

Here’s an interesting example of a field not quite like those explored
in the previous exercise.26 Consider the set F2 WD f0; 1g. We equip F2
with addition and multiplication modulo-2, as indicated by the addition
and multiplication tables + 0 1

0 0 1

1 1 0

-   0 1

0 0 0

1 0 1

So, a quick look reveals interesting things like 1 C 1 D 0 happen in F2
. The addition and multiplication tables clearly indicate that closure
of each is satisfied. Let’s take for granted that associativity is
satisfied – it’s not difficult to check, just tedious. We can see from
the addition and multiplication tables that the (additive) identity
element is 0 and that the (multiplicative) identity element is 1.
Exercise Check the inverse property of each of addition and
multiplication for F2 given the addition and multiplication tables.

11.267

The final piece in the “definition of a vector space” puzzle is the
definition of an action of a field on an abelian group, which we’ll
discuss now. An action of a field on an abelian group is an abstraction
of the “scalar multiplication” of vectors by numbers defined earlier in
the chapter. Here it is formally: An action of a field F on an abelian
group V is a function  W F  V ! V satisfying some properties. Before
listing the properties, we’d like to mention that we’ll not write .a;
v/ when expressing the application of the function (action)  to a pair
.a; v/, with a in F and v in V . Instead, we’ll write a  v to be
succinct. it’s advisable to think of an action as scalar multiplication
of a vector v by a number a. Here are the defining properties of an
action:  Distributivity I: For all a 2 F and all u; v in V , 26 This

is called the Galois field, abbreviated GF2 . Galois was a startlingly
brilliant mathematician who lived for only twenty one years, from 1811
to 1832. During his short life, he essentially founded all of Galois
theory and group theory in an effort to determine precisely when the
solutions of a polynomial equation could be written down explicitly. To
understand the issue he was interested in, try to find the exact
solutions to the equation x 5 x C 1 D 0.

SECTION 11.8 How to Build a Vector Space From Scratch

307

a  .u C v/ D a  u C a  v  Distributivity II: For all a; b 2 F and
all v in V , .a C b/  v D a  v C b  v These distributivity axioms are
subtle. The addition on the left is happening in the field F, while the
addition on the right is happening in the group V ! To see what we mean,
try this exercise:  11.268

Let a D 2 and u D

Exercise

1 0



1 0





0 1

 . Check that



0 1



;v D

a  .u C v/ D a  u C a  v, i.e.,  2

1 0



 C

0 1



 D2

C2

 Compatibility of the action with multiplication in the field F: For
all a; b 2 F and v in V .ab/  v D a  .b  v/ This is also subtle.
We’re asking that multiplying two elements of the field and then
applying the resulting element of the field to a vector be the same as
iteratively applying those elements of the field. Try this exercise to
get a feel for this idea:  11.269

Exercise

Let a D 2; b D 3 and v D

1 0

 . Check that .ab/v D

a  .b  v/, i.e.,  .2  3/ 

1 0



 D2 3



1 0



 Identity: For all v in V , 1vDv This is to say that the
(multiplicative) identity element of the field should act on the group V
in such a way as to not disturb V .

308

CHAPTER 11 Mathematical Tools for Quantum Computing I

Exercise Check  that the (multiplicative) identity 1 of the field C 1
acts on the vector in the way that is requested in the identity clause,
0 i.e., check that     1 1 1 D 0 0

11.270

11.271

Definition Action of a field on an abelian group

An action of a field F on an abelian group V is a function  W F  V ! V
satisfying:  Distributivity I: For all a 2 F and all u; v in V , a  .u
C v/ D a  u C a  v  Distributivity II: For all a; b 2 F and all v in
V , .a C b/  v D a  v C b  v  Compatibility of the action with
multiplication in the field F For all a; b 2 F and v in V : .ab/  v D a
 .b  v/  Identity: For all v in V , 1vDv

The Definition of a Vector Space Congratulations! If you’ve made it to
this point (and you’ve completed and understood the exercises), you
understand the mathematician’s definition of a vector space V over a
field F. You’ll likely have to review the definitions above and play
around with a few examples to get a solid understanding of them, so here
are some examples to play with: 11.272 Exercise To solidify your
understanding of the definition of a vector space, verify that each of
the following are examples of vector spaces:  Q over itself (yes, it’s
a vector space!)  R over R  C over C

SECTION 11.8 How to Build a Vector Space From Scratch

     

309

Q2 over Q R2 over R C2 over C Qn over Q Rn over R Cn over C

You’re now invited to contrast the succinct sentence “A vector space V
over a field F is an abelian group V equipped with an action of F on V ”
with the definition found in most standard texts on linear algebra: A
vector space V over a field F is a set satisfying the following
properties:  Associativity of addition: For all u; v; w 2 V , .u C v/ C
w D u C .v C w/  Commutativity of addition: For all u; v 2 V , uCvDvCu
 Identity element of addition: There exists an element 0 2 V such that
for all v 2 V , vC0Dv  Inverse element of addition: For every v 2 V ,
there exists an element v 2 V such that v C . v/ D 0  Compatibility of
scalar multiplication and field multiplication: For any a; b 2 F and any
v 2 V , .ab/v D a.bv/  Identity element of scalar multiplication: For
any v 2 V , 1v D v where 1 is the multiplicative identity of the field F
 Distributivity of scalar multiplication with respect to vector
addition: For all a 2 F and any u; v 2 V , a.u C v/ D au C av 
Distributivity of scalar multiplication with respect to field addition:
For all a; b in F and any v 2 V , .a C b/v D av C bv

310

CHAPTER 11 Mathematical Tools for Quantum Computing I

Even after requiring the properties above, we would still have to define
a field axiomatically as a set F together with two operations, called
addition (denoted C) and multiplication (denoted ), where by an
operation we mean an association of any pair of elements of F to some
other element of F. Thus, the definition of a vector space in this
approach still requires additional properties:  Associativity of
addition and multiplication: For all a; b; c 2 F, a C .b C c/ D .a C b/
C c

and

a  .b  c/ D .a  b/  c

 Commutativity of addition and multiplication: For all a; b 2 F, aCb
DbCa

and

ab Dba

 Additive and multiplicative identity: There exist two elements 0 and 1
in F such that for all a 2 F, aC0Da

and

a1Da

 Additive inverses: For every a 2 F, there exists an element such that
a C . a/ D 0

a in F

 Multiplicative inverses: For every nonzero element a in F, there
exists an element a 1 in F such that aa

1

D1

 Distributivity of multiplication over addition: For all a; b; c 2 F, a
 .b C c/ D a  b C a  c The choice is up to you! Since many linear
algebra textbooks do not wish to cover set theory, they are forced to
delineate an exhaustive list of properties to define a vector space.
With set theory in hand, we state the definition of a vector space once
more to remind you: 11.273

Definition Vector Space

A vector space V over a field F is an abelian group V equipped with an
action of the field F on V .

SECTION 11.8 How to Build a Vector Space From Scratch

311

Subspaces Now that we know what a vector space is (make sure you do!),
we can define the notion of a subspace of a vector space. It’s pretty
much what it sounds like. You have a space of vectors and then you
consider a subcollection of vectors that also satisfies the properties
of a vector space. 11.274

Definition Subspace of a Vector Space

A subset S  V of a vector space V over a field F is a subspace of V iff
S is a vector space over F. The remarkable thing is that instead of
having to verify all of the properties of a vector space for S after
having done so for V , the verification of the subspace property of a
subcollection of a vector space can be checked in three easy steps:
11.275

The subspace lemma

S  V is a subspace of a vector space V over a field F iff  Identity: 0
2 S , where this 0 is the additive identity that comes as part of the
data of the vector space V  Additive closure: For all u; v 2 S , u C v
2 S  Closure under scalar multiplication: For all a 2 F, v 2 S, a  v 2
S Let’s see an example. Consider the vector space R2 and the x-axis,
which we may think of as the set of points    x X WD W x 2 R  R2
(11.276) 0 We claim that X  R2 is a subspace. We’ll apply the subspace
lemma to prove this. First of all, the zero vector is in fact part of
the x-axis, so the identity property is satisfied. Second, it’s easy to
see geometrically that the sum of two vectors on the x-axis is another
vector on the x-axis. However, here is a rigorous proof. Let     x1
x2 ; (11.277) 0 0 each be elements of the x-axis (these are like our u
and v in the additive closure clause of the subspace lemma). Then

312

CHAPTER 11 Mathematical Tools for Quantum Computing I



x1 0



 C

x2 0



 D

x1 C x2 0C0



 D

x1 C x2 0

 (11.278)

This is another element of the x-axis. Lastly, we see that if we take a
scalar multiple of a vector on the x-axis that it will again be a vector
on the x-axis. We give a rigorous proof.   x Let a be in R and v WD in
X. Then, we need to check that a  v is 0 again in X (here, a and v are
like the a in the v in the closure under the scalar multiplication
clause in the subspace lemma). To see that this is the case, look at  
  x ax avDa D (11.279) 0 0 This is another element of the x-axis.
So, it is true that the x-axis is a subspace of R2 . Exercise You’re
invited to verify that the y-axis, and in fact, any line through the
origin in the vector space R2 over R is in fact a subspace of R2 . By a
line through the origin in R2 , we mean the set of points    x LD
Wx2R ax for a fixed a 2 R. Use the subspace lemma like we did above to
make your life easier, or else you’ll have to verify all of the
properties of a vector space again. Why do we emphasize that the line be
“through the origin”? What happens if it doesn’t pass through the
origin?

11.280

We close this section with the definition of a linear transformation
between arbitrary vector spaces: Definition vector spacesa

11.281

Definition of a linear transformation between

A linear transformation T between vector spaces V and W , each over a
field F, is a function T W V ! W satisfying the following properties: 
For all x; y 2 V , T .x C y/ D T .x/ C T .y/.  For all x 2 V and all a
2 F, T .a  x/ D a  T .x/. a It should be noted that the addition of x
and y in the definition above is occurring in the vector space V ,
whereas the addition of T .x/ and T .y/ is occurring in W , and V and W
may have different definitions of the operation C. A similar remark
holds for the scalar multiplication occurring in the second criterion.

SECTION 11.9 Span, Linear Independence, Bases and Dimension

11.9

313

Span, Linear Independence, Bases and Dimension

Span A quick comment about  some  of the notation that follows: We
will often write T 1 a column vector like as a transposed row vector
like so 1 0 for 0 simplicity of presentation. The definition of a vector
space provided above is helpful, but it would be nice to have a more
concrete description. Let’s think about the vector space R2 over R for a
moment so that we can motivate a new definition. Let’s say we want to
make a vector in R2 . In other words, we would like to construct any
vector in two-dimensional space. A moment’s thought brings forth the
realization that we can build any vector in two-dimensional space with
just two vectors. Let’s make this idea more precise. Visualize the
vector   1 1 in R2 . Suppose we’d like to get from the origin to the
point in space to which this vector points. We can travel along the
x-axis 1 step, and then travel upward 1 step. We could also travel
upward along the y-axis first, and then rightward 1 step. Here is the
algebraic manifestation of this concept:       1 1 0 D1 C1 1 0 1
In other words, the vector . 1 1 /T is 1 of the vector . 1 0 /T plus 1
of the vector . 0 1 /T . So, we can build the vector . 1 1 /T using the
“building blocks” . 1 0 /T and . 0 1 /T . Can we make every vector in R2
in this way? Exercise Try to build the vector . 2 3 /T using some
combination of the building blocks . 1 0 /T and . 0 1 /T . Can you make
the vector . 12 13 /T ? Nobody said we can’t use fractional parts of our
building p p blocks! What about the vector . 22 22 /T ? 11.282

 100

CHAPTER 11 Mathematical Tools for Quantum Computing I

What we’re getting at here is the notion of a spanning set of vectors.
We say that the vectors . 1 0 /T and . 0 1 /T span the vector space R2
over R. We do have to be a bit more precise here though. What if we were
asked to build the vector . 12 13 /T and we weren’t allowed to use
fractional amounts of our building blocks . 1 0 /T and . 0 1 /T ? So,
imagine we can only use integer multiples of the building blocks. Well,
then we can’t make the vector . 12 13 /T , at least not with integer
multiples of . 1 0 /T and . 0 1 /T . So, we really should say a bit more
about in what sense the building blocks span the space. Here is the
formal definition and some terminology that will be useful for the
discussion which follows: 11.283

Definition Spanning set of vectors

We say that a set of vectors v1 ; :::; vm spans a vector space V over a
field F iff for each vector v in V , there exist elements a1 ; :::; am
of the field F such that a1  v1 C a2  v2 C ::: C am  vm D v Then, we
define the span of a set of vectors: 11.284

Definition Span of a set of vectors

The span of a set of vectors v1 ; :::; vm over a field F is defined to
be: span.fv1 ; :::; vm g/ WD fa1 v1 C ::: C am vm W a1 ; :::; am 2 Fg :
We often abbreviate the phrase “span of a set of vectors v1 ; :::; vm
over a field F” to simply “span of v1 ; :::; vm ” when the field F is
understood. We say that a vector v is in the span of some vectors v1 ;
:::; vm iff v 2 span.fv1 ; :::; vm g/. We call a1 ; :::; am the
coefficients of the F-linear combination of the vectors v1 ; :::; vm .
Furthermore, we say that the set of vectors spanned by the vectors v1 ;
:::; vm (equivalently, the set of all F-linear combinations of the
vectors v1 ; :::; vm ) is the span of the vectors v1 ; :::; vm . So, we
can rephrase our definition above to say that a set of vectors fv1 ;
:::; vm g spans a vector space V over a field F iff span.fv1 ; :::; vm
g/ WD fa1 v1 C ::: C am vm W a1 ; :::; am 2 Fg D V In other words, every
vector in V can be constructed from a sum of Fmultiples of the “building
blocks” (spanning set) of vectors v1 ; :::; vm .

SECTION 11.9 Span, Linear Independence, Bases and Dimension

315

Exercise Can you find another spanning set of vectors for R2 ? How many
such sets do you think there are? Can you find a spanning set for R3 ?

11.285

Linear Independence Having thought about the previous exercise a bit,
you’re likely convinced that there are several – in fact, infinitely
many – spanning sets for R2 , R3 , any Rn as vector spaces over R, and
likewise, any vector space Cn over C. This is wonderful in that we know
that there are several sets of vectors that suffice to build the vector
spaces we care about. What is interesting to consider is whether there
is a minimum set of vectors we can use to build the space we are
considering. For example, we can build all of the vectors in R2 using
the set of three (!) vectors       1 3 5 ; ; (11.286) 2 4 6
We’ll try to convince you here by showing that we can at least build the
T vector 10 10 using these three vectors. Before you see what we do you
should think of how many of each of these vectors you need to construct
T 10 10 . It’s not that easy, actually...         10 1 3 5 D1
C . 7/  C6 (11.287) 10 2 4 6 11.288

Exercise

Check that the equality above is true!

This probably seems a bit magical if you tried to figure it out yourself
before you looked. It turns out that it’s nothing more than solving a
bunch of equations though! Of course, you’re probably thinking “...we
had a perfectly good set of two vectors that we could use to build
everything already. Why bother with this set of three more complicated
vectors?” Fair question. First, we’ll show you that we don’t need three
vectors at all – only two. In other words, these three vectors span R2
over R, but we can do with just two. Later on, we’ll try to

316

CHAPTER 11 Mathematical Tools for Quantum Computing I

argue that it is occasionally advantageous to use different sets of
building blocks at different times – sort of like a change in
perspective. To see that we only need two of these vectors, we’ll show
that one of them can be built from the others and then we’ll revisit the
previous example and drive the point home. Observe that       5 1
3 D . 1/  C2 (11.289) 6 2 4 You might have seen this without any
calculation. The point is that we can T replace any instance of the
vector 5 6 with this combination     1 3 . 1/  C2 (11.290) 2 4 So,
we revisit the previous example and apply this substitution:      
  10 1 3 5 D1 C . 7/  C6 10 2 4 6     1 3 D1 C . 7/  2 4  
   1 3 C 6  . 1/  C2 (11.291) 2 4 and then reorganize:    1
D1 C . 7/  2    1 D1 C . 6/  2    1 D . 5/  C5 2

3 4



1 2



3 4



 C . 6/   C . 7/ 

1 2



3 4





3 4





3 4



C 12  C 12 

(11.292)

T So, we can express our original vector 10 10 using only the building
T T blocks 1 2 and 3 4 . T In sum, we say that 5 6 is R-linearly
dependent (even Z-linearly T dependent, since the coefficients are all
integers!) on the vectors 1 2 T T T and 3 4 and that 10 10 is in the
span of the vectors 1 2 T and 3 4 . Using our previous definition of
span, we can state precisely what it means for a vector to be linearly
dependent on a set of vectors.

SECTION 11.9 Span, Linear Independence, Bases and Dimension

11.293

317

Definition Linear dependence

A vector v in a vector space V over a field F is F-linearly dependent on
the vectors v1 ; :::; vm iff v is in spanfv1 ; :::; vm g. We often just
use the term linear dependence rather than F-linear dependence where the
field is understood. Naturally then, we have a notion of linear
independence of vectors! 11.294

Definition Linear independence of a set of vectors

We say that a set of vectors fv1 ; :::; vm g is linearly independent if
none of the vectors in the set are linearly dependent on the others.
More precisely, we say that fv1 ; :::; vm g is a linearly independent
set of vectors iff for each i 2 f1; :::; mg, vi is not in spanfv1 ; :::;
vi 1 ; vi C1 ; :::vm g. Exercise Do we need two vectors to span all of
R2 ? Can we get away with just having one?

11.295

Bases and Dimension Finally, we can define a basis of a vector space.
This definition will unlock a matrix-centric view of linear algebra, as
we’re about to see. You might be wondering why we bothered defining all
of the previous terms. It turns out that the precise definition of a
matrix that we desire depends (linearly? We couldn’t resist...) on the
precise definition of a basis of a vector space. In fact, you might have
been frustrated by the idea of a matrix this whole time, wondering,
“Where are the numbers in the grid coming from?” If you answered a
previous exercise asking you to conjecture what the columns of a matrix
tell us, what follows will be quite satisfying! First, the definition of
a basis: 11.296

Definition The definition of a basis

A basis of a vector space V over a field F is a linearly independent
spanning set of vectors.

318

CHAPTER 11 Mathematical Tools for Quantum Computing I

That’s it? Well, quite a bit is packed into the definitions of linearly
independent and spanning, so you might want to review those!  11.297

Exercise

Check that the set

1 0

   0 ; is in fact a basis 1

for R2 .

We keep saying a basis, which implies there are more than one.
Hopefully, you convinced yourself earlier that there are infinitely many
spanning sets of vectors for R2 . It thus follows that there’s an
infinite number of linearly independent spanning sets for R2 as a
result. Here are a bunch more:             2 0 1 3 1 0
; ; ; ; ; (11.298) 0 1 2 4 0 1 All of these bases have the same number
of vectors! With enough playing around (don’t just believe us!), we
might eventually be convinced that all bases have the same number of
vectors, and in fact they do. This is what many call the fundamental
theorem of linear algebra: 11.299

Invariance of basis number

The number of basis vectors for a vector space is the same no matter
which basis we choose. This calls for a definition! 11.300

Definition Dimension

The dimension of a vector space V is the number of vectors for any basis
for V . Observe that we need the theorem to have a well-defined notion
of dimension. If we didn’t know that all bases have the same length, we
could potentially have two different answers for what the dimension of a
vector space is! Believing the theorem, we have a natural notion of
finite-dimensionality: a vector space is finite-dimensional iff it has a
finite basis. We won’t prove the theorem here, and instead will offer
some slight indication for why it should be true. It is likely
believable that any set of linearly independent vectors in a
finite-dimensional vector space should have size less than or equal to
the size of any spanning set of vectors. This fact

SECTION 11.9 Span, Linear Independence, Bases and Dimension

319

is known as the Exchange Lemma. It is of fundamental importance in
linear algebra. You can quickly ascertain the power of the Exchange
Lemma, since knowing it and that any two bases are spanning sets already
implies they must be of the same length. Exercise Convince yourself that
any two bases for a finite-dimensional vector space have the same size.

11.301

This idea has major implications. Suppose we already know the dimension
d of a vector space V and that we’d like to find a basis for this vector
space. Imagine we already have a set of d vectors that spans the vector
space V . Well, then the previous discussion guarantees that this list
of d spanning vectors is linearly independent and thus already a basis
for V ! Likewise, if we have a list of d linearly independent vectors in
V , they must span V and are a basis as well. So if we want to find a
basis for a vector space V of dimension d , it suffices to discover a
list of d vectors that are either all linearly independent or that spans
the space V . One or the other is enough, so long as we have d vectors.
Unless otherwise mentioned, we will restrict our attention to the
finite-dimensional case. We write the dimension of a vector space V over
a field F as dimF .V /, but often shorten this to dim.V / when the field
is understood. So, relating this idea to a question asked in the
self-test at the outset of the chapter, we would write dimC .C2 / to
indicate the dimension of the vector space C2 considered as a vector
space over the field C and dimR .C2 / to indicate the dimension of the
vector space C2 considered as a vector space over the field R. The first
of these, dimC .C2 /, is equal to 2, while the second, dimR .C2 /, is
equal to 4. They are therefore not the same thing, and we now appreciate
that the subscript is occasionally quite important.27 Exercise Try to
find a basis of length 2 for the vector space C2 over C and then a basis
of length 4 for the vector space C2 over R. This should convince you
that the subscript is occasionally necessary. Then, think about the
question from the self-test again, and figure out why it’s a trick
question.

11.302

27 This point relates to the question in the self test at the opening of
the chapter which asks the reader to compare R4 and C2 .

320

CHAPTER 11 Mathematical Tools for Quantum Computing I

Orthonormal Bases Once we have a basis, we can ask that it satisfy
certain conditions. Let’s take our cue from a basis we know and love at
this point     1 0 ; D fj0i ; j1ig (11.303) 0 1 What’s so nice
about this particular basis is that each of the vectors are of unit
length (i.e., have L2 norm 1) and they are what is referred to as
orthogonal to each other. “Orthogonal” is essentially a fancy word for
perpendicular.28 11.304

Definition Orthogonality of vectors

More precisely, we say that two vectors u; v in a vector space V
equipped with an inner product h; i are orthogonal (to each other) iff
their inner product is zero, i.e., hu; vi D 0. In Dirac notation, we say
that two vectors u and v are orthogonal iff hujvi D 0. A basis such that
each of the elements have unit length and such that they are pairwise
orthogonal, is known as an orthonormal basis. In the context of quantum
computing, we choose a set of orthonormal basis vectors to be our
preferred computational basis vectors. We can say this a bit more
mathematically: 11.305

Definition Orthonormal basis

A set of vectors B D fv1 ; :::; vn g in a vector space V is called an
orthonormal basis iff B is a basis, and for all i; j 2 f1; :::; ng, (
hvi ; vj i D 1 if i D j hvi ; vj i D 0 if i ¤ j We’ll learn later that
what is written above is an instance of what is known as the Kronecker
Delta function ı. An important theorem of linear algebra 28
Perpendicular

and orthogonal are interchangeable except in the case that either vector
is the zero vector, since it does not make sense to say that a vector is
perpendicular to the zero vector as there is no angle between them. When
comparing two vectors when at least one of the vectors is the zero
vector, we use the word orthogonal.

SECTION 11.9 Span, Linear Independence, Bases and Dimension

321

is that every spanning set of vectors in a finite-dimensional vector
space can be pruned to form an orthonormal basis. The process yielding
the desired orthonormal basis is known as the Gram-Schmidt process in
honor of Jørgen Pedersen Gram and Erhard Schmidt. 11.306

Gram-Schmidt Orthonormalization

Every spanning set of vectors for a finite-dimensional vector space can
be modified to form an orthonormal basis. Let’s relate these ideas to
some of the quantum computing you’ve read earlier. You’ve read by now
that any state is a superposition of the states j0i and j1i. The first
thing you should check is that the states j0i and j1i are orthogonal to
one another: Exercise Verify that the vectors j0i and j1i are in fact
orthogonal to one another, i.e., h0j1i D 0.

11.307

Then, you should check that they’re even orthonormal! Exercise Verify
that the vectors j0i and j1i are even orthonormal, i.e., h0j0i D 1 and
h1j1i D 1.

11.308

We already know that fj0i ; j1ig is a basis for R2 . It’s not too
difficult to believe that fj0i ; j1ig is also a basis for C2 .

CHAPTER

12 Mathematical Tools for Quantum Computing II 12.1

Linear Transformations as Matrices

We claimed earlier that every linear transformation has an associated
matrix, and vice versa. We aim to demonstrate for you that, in fact, a
linear transformation and a matrix are the same thing. This justifies
the study of linear algebra as the study of matrices and operations on
them. Equipped with the definition of a basis, we are prepared to define
the matrix associated to a linear transformation between two vector
spaces. Let V and W be vector spaces over some field F. Yes, they have
to be vector spaces over the same field – you’ll see why! Then, V and W
each have a basis, say BV D fv1 ; :::; vn g and BW D fw1 ; :::; wm g.
So, V has dimension n and W has dimension m. Let T be a linear
transformation between the vector spaces V and W . So, T W V ! W is a
linear transformation, and thus a function. Since T is a linear
transformation from V to W , each basis element vj for j 2 f1; :::; ng
is mapped into W , i.e., T vj 2 W . Since W is spanned by the vectors w1
; :::; wm and T vj 2 W , there exist coefficients a1;j ; :::; am;j such
that T vj D a1;j w1 C ::: C am;j wm , i.e., we can express each T vj as
a linear combination of the basis elements w1 ; :::; wm . So, to each
basis element vj of V , we have an associated list of elements a1;j ;
:::; am;j of the field F. Maybe you see where we’re going with this...
We define the matrix M .T W V ! W /BV ;BW associated to the linear
transformation T W V ! W with respect to the bases BV and BW entrywise:

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_12

323

324 12.1

CHAPTER 12 Mathematical Tools for Quantum Computing II

Definition

Matrix associated to a linear transformation M .T W V ! W /BV ;BW

 i;j

WD ai;j

where ai;j is the coefficient of the i th basis element of BW in the
linear combination T vj D a1;j w1 C ::: C am;j wm expressing the image T
vj of the j th basis element of BV . Exercise You should wonder why we
can’t play the same game with any transformation between vector spaces.
More specifically, why do we only define a matrix for a linear
transformation between vector spaces? Can you figure this out? 12.2

Let’s see this construction of a matrix in action. Consider the linear
transformation T from R2 ! R2 described by  T

x y



 WD

xCy x y



where we take the basis for R2 to be the standard basis     0 1 ;
0 1 in each case. So far, we each of V and W are R2 , and each  have
Tas defined,  1 0 of BV and BW are ; . 0 1 Exercise Check that the
transformation T given above is actually a linear transformation.

12.3

Now that you’ve verified that the transformation T is linear, we can
proceed to figure out the coefficients ai;j as in the construction
above. This amounts to figuring out where T sends the two basis
elements. Following the definition of T , we have       1 1C0 1 T
WD D (12.4) 0 1 0 1 Then, we decompose this into a linear combination of
the basis vectors like so

SECTION 12.1 Linear Transformations as Matrices



1 1



 D1

1 0



 C1

0 1

325

 (12.5)

At this point, we see that M .T W V ! W /BV ;BW



M .T W V ! W /BV ;BW



1;1

WD a1;1 D 1

(12.6)

2;1

WD a2;1 D 1;

(12.7)

and that We’ll abbreviate the fancy notation M .T W V ! W /BV ;BW



(12.8)

with M .T / when the vector spaces V and W and their bases BV and BW are
understood. Verify that  a1;2  D 1 and a2;2 D 1 by determining 0 where
the second basis vector is mapped to and decomposing the 1   1
resulting vector into a linear combination of the basis vectors and 0 
 0 . 1 12.9

Exercise

After all of this computation, we realize that the matrix associated to
the linear transformation T W V D R2 ! W D R2 with respect to the bases
    1 0 BV D BW D ; (12.10) 0 1 is M .T / D



1 1

1 1

 (12.11)

Exercise To practice building matrices from the description of a linear
transformation, construct the matrix associated to the linear
transformation T W V D R3 ! W D R3

12.12

defined by

326

CHAPTER 12 Mathematical Tools for Quantum Computing II

0

1 0 1 x 1x C 2y C 3z T @ y A WD @ 4x C 5y C 6z A z 7x C 8y C 9z with
respect to the standard basis 80 1 0 1 0 19 0 0 = &lt; 1 @ A @ A @ 0 ; 1
; 0 A BV D BW D : ; 0 0 1 for each. You should first check that this is
a linear transformation. Then, figure out where each of the basis
vectors is mapped. Once you know this, decompose those into a linear
combination of the basis vectors and use the coefficients of those
linear combinations to build the matrix.

Unless we mention otherwise, we will assume that the vector spaces Rn
and Cn have the standard bases. You may be frustrated by the definition
of matrix multiplication that we gave earlier on. We’d like to
demonstrate why it is defined the way it is. It has to do with the
intimate relationship between the composition of two transformations (as
functions) and the product of the matrices as we have defined it.
Consider the following two transformations R W R2 ! R2 and S W R2 ! 2 R
defined by     x y R WD (12.13) y x and

 S

x y



 WD

y x

 :

(12.14)

Exercise First, try to understand these transformations geometrically.
Then, figure out matrices M .R/ and M .S / representing each of these
transformations (using the standard bases). Afterward, recall how it is
that we multiply two matrices, and compute each of the matrix products

12.15

M .R/  M .S /

and

M .S /  M .R/

(12.16)

They should not be equal, which might be clear from your geometric
interpretation!

If you did the above exercise, you now know that R and S have matrices

SECTION 12.1 Linear Transformations as Matrices

M .R/ D



0 1 1 0



and M .S / D



0 1 1 0

327

 (12.17)

and that the products are     1 0 1 0 M .R/  M .S/ D and M .S /  M
.R/ D (12.18) 0 1 0 1 Ok, now we’re prepared to find the composition of
the transformations (functions) R and S . Remember that we work
“inside-out.” So, S is applied first and R is then applied after S .
Thus, we can compute R ı S as          x x y x .R ı S/ DR S DR
D (12.19) y y x y Next, let us compute S ı R:          x x y x
.S ı R/ DS R DS D y y x y

(12.20)

They’re not the same! We’re getting closer to the analogy. Now, we find
the matrix associated to the transformation R ı S . Note where the two
basis vectors end up and then express each result as a linear
combination of the basis vectors on the other side. Then, the
coefficients in these linear combinations help us build the matrix.  
      1 1 1 0 .R ı S/ D D1 C0 (12.21) 0 0 0 1 and  .R ı S/

0 1



1 0



 D

0 1



1 0



 D0

1 0



 C . 1/ 

0 1



0 1



(12.22)

and  .S ı R/

 D

 D . 1/ 

1 0



 C0

(12.23)

and  .S ı R/

0 1



 D

0 1



 D0

1 0



 C1

0 1

 (12.24)

Now, we have everything we need to build the matrices M .R ı S / and M
.S ı R/!

328

CHAPTER 12 Mathematical Tools for Quantum Computing II

Exercise Using the above computations, determine the matrices M .R ı S/
and M .S ı R/.

12.25

Having done the above exercise, you now see that the matrices associated
to the transformations R ı S and S ı R are     1 0 1 0 M .R ı S/ D
and M .S ı R/ D (12.26) 0 1 0 1 and these are the matrices M .R/  M .S
/ and M .S /  M .R/ we computed earlier! This isn’t just a happy
coincidence, by the way. This is the motivation for defining the matrix
product the way we did. 12.27

The Matrix of a Composition of Linear Transformations

The matrix of a composition of linear transformations is the product of
their matrices, for all linear transformations S and T , M .S ı T / D M
.S /  M .T /

12.2

Matrices as Operators

We refer to a linear transformation that maps from a vector space to
itself as a linear operator on that space. In fact, all of the linear
transformations we’ve considered (except for one non-square matrix that
we used to explain the transpose operation on matrices) are linear
operators! We pay special attention to operators in quantum mechanics.
More particularly, we care about invertible linear operators because we
can use them to create quantum gates and thus quantum circuits. Next, we
introduce the determinant, a numerical invariant of a matrix encoding
the invertibility of the transformation of space that it represents!

An Introduction to the Determinant Each square matrix has an associated
determinant, which speaks for the geometry of the linear transformation
of space represented by that matrix. It subsequently describes the
invertibility of the linear transformation, whether the transformation
can be undone.

SECTION 12.2 Matrices as Operators

329

What do we mean by this idea that a transformation can be undone? Let’s
see an example of a transformation that can be undone, and then an
example that can’t. First, an example of a transformation that can be
undone: Consider the linear transformation R from R2 to R2 described by
the matrix   1 0 R WD (12.28) 0 ei  which can be found in chapter 3.
Exercise Review Euler’s formula from earlier in this chapter and check
that e i D cos ./ C i sin ./ D 1 C 0  i D 1

12.29

The above exercise alerts us to the fact that the matrix R above can
actually be expressed as     1 0 1 0 R WD D (12.30) 0 1 0 ei 
Exercise You’re invited to investigate and figure out which
transformation of two-dimensional space is described by this matrix.
Figure out where the basis vectors are mapped and you should get an
idea! 12.31

If you tried the above exercise, you probably figured out that the
matrix R describes a reflection of two-dimensional space over the
x-axis. Believing this, it is fairly clear geometrically that this
transformation can be undone – just reflect back! Or you could just
reflect again, since two reflections over an axis does nothing. You
might wonder then why  appears in the name of this matrix. We’ll give
you a little idea of why. The  is there to signify that this matrix has
the effect of rotating the larger space C2 about the z-axis1 by 
radians, although we’d prefer not to get into this discussion right now.
We’d like for you to take away the fact that this is a linear
transformation of space that can be undone – that’s good for now! 1
Refer

to the Bloch sphere in chapter 3.

330

CHAPTER 12 Mathematical Tools for Quantum Computing II

You might have also noticed that the matrix R is a special case of the
matrix   1 0 R' WD (12.32) 0 e i' mentioned in chapter 3, where the
angle ' is . Now, let us consider a transformation that cannot be
undone. Consider the transformation Projx from R2 to R2 described by the
matrix   1 0 Projx WD (12.33) 0 0 Exercise As before, you should try
and figure out which transformation of space is described by the matrix
  1 0 Projx WD 0 0

12.34

above. The name might give it away...

So, if you tried the above exercise, you’re hopefully convinced that
this matrix describes the projection of a vector onto the x-axis. For
example, T T applying Projx to the vector 1 1 yields 1 0 . Since many
vectors T also get mapped to 1 0 by Projx we lose information as to
what the T input was if we just look at the output. For example, this
vector 1 2 T also gets mapped to 1 0 (and actually, any vector whose
first component is 1 will as well!). Since we cannot recover the input
from the output and this transformation cannot be undone, it is not
invertible. In essence, this transformation collapses the whole space to
the x-axis. This mental image should give the impression that we cannot
undo this transformation. In some sense, a higher dimensional space is
collapsed into a smaller dimensional one, and so information must be
lost. We don’t like such transformations in quantum computing! We’d like
for the matrices that represent the quantum logic gates we use to
preserve all of the information given to them, and we’d like for these
transformations to be reversible. We’ll see that we even ask for more of
these matrices in what follows. So, at this point, hopefully you’re
convinced that not all linear transformations can be undone. It would be
nice to have a numerical invariant that encodes the invertibility of a
linear transformation. Enter the determinant.

SECTION 12.2 Matrices as Operators

331

Let’s see how to compute the determinant of a 22 matrix with an
example. Consider the matrix   1 2 A WD (12.35) 3 4 We compute its
determinant like so det.A/ WD

1 3

2 D14 4

23D4

6D

2

(12.36)

Exercise You’re invited to investigate and describe the transformation
of two-dimensional space described by this transformation. Figure out
where the basis vectors end up and that should give you an idea! 12.37

The previous exercise hopefully convinced you that the transformation of
two-dimensional space represented by the matrix A is invertible. Let’s
follow this example and compute the determinants of the matrices
described above det.R 2 / WD

1 0

det.Projx / WD

0 D 1  . 1/ -1

00D

1 0

00D0

0 D10 0

1

(12.38) (12.39)

If you’re observant, you may notice that the matrices corresponding to
the invertible transformations have nonzero determinant, while the
matrix corresponding to the non-invertible transformation has zero
determinant. 12.40

Determinant of a 2  2 matrix

The determinant of a 2  2 matrix   a b c d is ad

bc

332

CHAPTER 12 Mathematical Tools for Quantum Computing II

You might wonder how to compute the determinant of a 3  3 matrix.
Again, we’ll demonstrate by example 0

1 1 2 3 1 @ A det 4 5 6 WD 4 7 8 9 7 D1

D 1  .5  9

5 8

8  6/

D 1  .45

48/

6 9

2

2  .4  9 2  .36

D 1  . 3/ D 12.47

3 C 12

4 7

2 5 8

3 6 9

(12.41)

4 6 C3 7 9

5 8

7  6/ C 3  .4  8 42/ C 3  .32

2  . 6/ C 3  . 3/ 9D9

9D0

(12.42)

7  5/

35/

(12.43) (12.44) (12.45) (12.46)

Equivalent formulations of invertibility

The following are equivalent for a linear transformation T :  det.T / D
0  T is not invertible  The rows of the matrix representing T are
linearly dependent  The columns of the matrix representing T are
linearly dependent Unfortunately, we will not prove this here. This set
of equivalences relating the determinant of a matrix, and thus a linear
transformation, to geometric attributes such as invertibility of the
transformation should be surprising given the seemingly combinatorial
description of the determinant. It might not seem geometric at all from
the definition we’ve given.

The Geometry of the Determinant There is a more geometric definition of
the determinant and we would like to give you a small taste of it.
Consider the matrix   1 4 2 2

SECTION 12.2 Matrices as Operators



0 1

333





1 0



Figure 12.1: Unit square in the plane



1 2

 

4 2



Figure 12.2: Parallelogram

  1 again and observe that it sends the first basis vector to the
vector 0       1 0 4 and it sends the second basis vector to the
vector . This 2 1 2 should convince us that the unit square formed by
the basis vectors in the first quadrant, as in Figure 12.1, is mapped to
the parallelogram whose coordinates are at the points         0
1 4 5 ; ; and 0 2 2 4 as depicted in Figure 12.2. 12.48

Exercise

You should draw the parallelogram!

334

CHAPTER 12 Mathematical Tools for Quantum Computing II

You’ll realize that in some sense that the orientation of the unit 
square  1 “flips” upon being transformed to the parallelogram, since
the vectors 0   0 and , which constitute the unit square in the first
quadrant, exchange 1 places to form the parallelogram. The unit square
has area 1, while the parallelogram has area 2. What does this have to
do with the determinant of this matrix, which is -2? Well, that the
orientation of the unit square “flips” is encoded in the fact that the
determinant is negative. Transformations that preserve orientation have
positive determinant, while transformations that flip orientation have
negative determinant. Then, the magnitude of the determinant (absolute
value) encodes the factor by which the unit parallelogram is magnified
by the transformation. In general, the determinant of the matrix
associated to a linear transformation encodes whether that
transformation is orientation preserving and then by which factor it
“stretches” the unit parallelepiped (higher-dimensional analog of a
parallelogram) – quite geometric, actually! Figure 12.2 depicts the
parallelogram.

Matrix Inversion We previously discussed how the determinant of a matrix
encodes its invertibility. But how do we actually find the inverse
transformation? First off, when we say an inverse transformation, what
do we mean? Well, transformation is just another word for function, so
presumably what we seek is an inverse function of the transformation
we’re given. It might not be so simple to figure out what an inverse
function is though. To see what we mean, try to find the inverse
transformation for the transformation T of space described by T W R3 !
R3 (12.49) 0 1 0 1 x 1xC2yC3z @ A @ y 4xC5yC6z A T WD (12.50) z 7
 x C 8  y C 10  z Is it even clear that we can invert this
transformation? We saw that not all transformations are invertible.
Exercise Find the matrix M .T / associated to the transformation T and
then compute its determinant. Make a claim about the invertibility of

12.51

SECTION 12.2 Matrices as Operators

335

the transformation T based on your computation of the determinant. Can
we invert T ?

Exercise Can we give a reasonable geometric description of this
transformation of three-dimensional space from this definition of T ?

12.52

Recall from our earlier discussion about functions and attributes of
functions that we say that a function f W X ! Y is invertible iff there
exists an inverse function f 1 W Y ! X such that the compositions f 1 ıf
W X ! X and f ı f 1 W Y ! Y are the respective identity functions IX and
IY . So, we seek a transformation (function) T 1 whose composition with
the transformation T is the identity on either side. If we have such a T
1 , we’ll know that T ıT

1

D IR3

(12.53)

ı T D IR3

(12.54)

and T

1

Now that we know that every linear transformation of space is a matrix
and that the composition of two transformations is analogous to the
multiplication of their corresponding matrices, we might hope to express
the given transformation T as a matrix M .T /. We can then use this
matrix description to come up with an inverse matrix to multiply M .T /
to get the identity matrix (which corresponds to the identity function).
In other words, we apply the “matrix operation” to the compositions
above yielding M .T ı T

1

/ D M .IR3 /

(12.55)

ı T / D M .IR3 /

(12.56)

and M .T

1

The question then is what these matrices are. However, like we said
earlier, the matrix of a composition of transformations is the product
of their matrices, so we have M .T /M .T 1 / D M .IR3 / (12.57)

336

CHAPTER 12 Mathematical Tools for Quantum Computing II

and M .T

1

/M .T / D M .IR3 /

(12.58)

We need to find a matrix whose product with the matrix M .T / on either
side is the identity matrix. This is an enormous observation! We now
focus our attention on what it means to find such a matrix. Consider the
matrix   1 2 AD (12.59) 3 4 Let

 BD

x y z w

 (12.60)

be any other matrix, and now suppose that B has the desired inverse
property, that AB D I2 D BA. Well, then to start, we would have    1
2 x y AB D D I2 (12.61) 3 4 z w Let’s extract the meaning of 

1 2 3 4



x y z w

 (12.62)

Recall the definition of matrix multiplication. Before we compute the
product, you should give it a try!      1 2 x y 1xC2z 1yC2w D
(12.63) 3 4 z w 3xC4z 3yC4w Now, we want this to be equal to the
identity matrix, so we need for the following equations and inequations
to be satisfied 1x C 2z ¤ 0 1y C 2w D 0 3x C 4z D 0 3y C 4w ¤ 0 1x C 2z
D 3y C 4w

SECTION 12.2 Matrices as Operators

337

The second and third equations are self-evident, but the first, fourth
and fifth desire some explanation. We want for the first, fourth and
fifth entries to be nonzero and equal so that we can divide by them and
force the diagonal entries to be equal to 1 each. 12.64

Exercise

Try to solve the system of equations and inequations

above.

With enough effort, you’ll find that the appropriate choice of x; y; z;
w is x D 4; y D

2; z D

3; w D 1

(12.65)

So, the matrix we seek is  BD

4 3

Let’s compute the product   1 2 4 AB D 3 4 3

2 1

2 1



 (12.66)

 D

2 0

0 2

 (12.67)

That’s not the identity matrix! It’s not so bad, actually. Remember that
we demanded that the diagonal entries would be nonzero and equal? Now,
you’ll see why.  Sure, the matrix B doesn’t work, but the matrix 12  B
does (remember how we multiply a matrix by a number)        
 1 1 1 2 4 2 A B D  3 4 3 1 2 2     1 1 2 4 2 D 3 4 3 1 2  
  1 1 2 4 2 D 3 4 3 1 2    1 2 0 D 0 2 2   1   1 . 2/ 0 2
2  D 1 1 2 0 2  . 2/   1 0 D (12.68) 0 1

338

CHAPTER 12 Mathematical Tools for Quantum Computing II

So, we have good reason to call the matrix

1 2



B by the name A

1!

Exercise We should check that multiplying  on either side yields 1 the
identity matrix – do this! That is, verify that 2 B A D I.

12.69

Then, we have found the matrix inverting the matrix A, so it’s just a
matter of determining what linear transformation this inverse matrix
represents. Recalling that the entries in a matrix are exactly
expressing the coefficients of the images of the basis elements, we can
recover the transformation without too much trouble: Exercise  Try to
describe the linear transformation corresponding to the matrix 12  B
using function notation. Fill in the details in the unfinished equation
    1 x B WD y 2

12.70

Hopefully, you figured out that what should be on the right side of the
equation is the vector     1 4xC 3y  (12.71) 2xC1y 2 We’ve got
it! The inverse transformation of the linear transformation     x
1xC3y A WD (12.72) y 2xC4y which you might recall has the geometric
effect of transforming the unit square in the first quadrant into the
parallelogram described in the section about determinants, is the
transformation         1 1 x 4xC 3y B WD  (12.73) y 2xC1y
2 2 That’s wonderful and all, but is there a pattern here? Can we
extrapolate a general technique from this example? Perhaps you noticed
this matrix from our earlier discussion about determinants. Maybe you
even got the impression that the 2 appearing in the fraction 12 in front
of B has something to do with the previous discussion, since 2 is the
determinant of the matrix B! You’d be correct!

SECTION 12.2 Matrices as Operators

339

In general, given a 2  2 matrix  AD

a b c d

 (12.74)

its inverse matrix is the matrix A

12.76

1

WD

1 det.A/



d c

b a

 (12.75)

Definition Adjugate matrix

The matrix



d c

b a

 (12.77)

is known as the adjugate of A. In general, given a matrix A, we denote
the adjugate of A by adj.A/. What we discovered above can then be
phrased as  A  det.A/ 1 adj.A/ D det.A/ 1 .Aadj.A// D det.A/ 1
.det.A/I /  D det.A/ 1 det.A/ I D 1I D I (12.78) So, the inverse
of a matrix A is the matrix described by det.A/ 1  adj.A/. This makes
us realize that we need to find a way to determine the adjugate matrix.
Remarkably, the adjugate matrix is equal to the transpose of what is
known as the cofactor matrix of A. So, what is the cofactor matrix of a
matrix? We’ll define it and then invite you to verify that the adjugate
we built above does in fact satisfy this definition. Let us first define
Ai;j to be the .n 1/  .n 1/ submatrix of A formed by removing the i th
row and j th column of A. The i; j th entry of the cofactor matrix of A
is then Ci;j WD . 1/i Cj det.Ai;j /. We call Ci;j the i; j th cofactor
of A. We’ll demonstrate with an example. Consider the matrix 0 1 1 2 3
AD@ 4 5 6 A (12.79) 7 8 9 Let’s compute the 1; 1 cofactor C1;1 .
Removing the 1st row and 1st column of A yields the smaller 2  2 matrix

340

CHAPTER 12 Mathematical Tools for Quantum Computing II



5 6 8 9

 (12.80)

The cofactor C1;1 is then determined as follows C1;1 WD . 1/1C1 

12.82

Exercise

5 8

6 D59 9

8  6 D 45

48 D

3

(12.81)

Compute the cofactors C1;2 and C1;3 .

If you tried the above the exercise, you found that C1;2 WD . 1/1C2 

4 7

6 D . 1/Œ4  9 9

7  6 D 42

36 D 6 (12.83)

and C1;3 WD . 1/1C3 

4 7

5 D48 8

5  7 D 32

35 D

3

(12.84)

Exercise The ambitious reader should go forth and compute the remaining
6 cofactors C2;1 ; C2;2 ; C2;3 ; C3;1 ; C3;2 ; C3;3 and then construct
the cofactor matrix C . Further, transpose this matrix. You’ll run into
a problem if you try to create the inverse though!

12.85

If you try to construct the inverse of this matrix, you’ll run into an
issue, as stated in the above exercise. Everything works swimmingly
until you compute the determinant – it’s 0! There are several ways to
discern that the determinant of A is 0 and seeing them will tie some
ideas together. First of all, the first column 0 1 1 @ 4 A (12.86) 7 of
the matrix A is linearly dependent on the other two. 12.87

Exercise

Can you find the dependence?

SECTION 12.3 Eigenvectors and Eigenvalues

341

With a bit of computation, you’ll find that 2 times the second column
minus 1 times the third column yields the first column 0 1 0 1 0 1 1 2 3
@ 4 A D 2  @ 5 A C . 1/  @ 6 A (12.88) 9 7 8 If we apply the theorem
stated earlier about all of the equivalent ways of expressing that the
determinant of a linear transformation is 0, we see that the linear
dependence of the first column on the other two is equivalent to the
fact that the determinant of A is 0. Now, we’ll perform a computation
that will lead to a interesting observation connecting the inverse of a
matrix, its determinant, and the cofactor matrix we described above. It
will start off rather unusual, but if you follow each equality, you’ll
see the connection! det.A/ D 0 D .1/  . 3/ C .2/  .6/ C .3/  . 3/ D
.1/  C1;1 C .2/  C1;2 C .3/  C1;3 D A1;1  C1;1 C A1;2  C1;2 C A1;3
 C1;3

(12.89)

As you can see, we can compute the determinant by multiplying the
cofactors by their respective entries of the matrix along that row and
then summing the products. Hopefully, this example convinces you this
might be true. You should try to compute the determinant of A along the
second row instead. In fact, you should try to compute the determinant
along any row or column you like and see that they all yield the same
answer!

12.3

Eigenvectors and Eigenvalues

To motivate this next topic, let’s play around with the matrix   2 0 A
WD 0 3 Exercise it represents?

12.91

(12.90)

First of all, can you describe the transformation of space

342

CHAPTER 12 Mathematical Tools for Quantum Computing II

You’ll realize that the first basis vector is stretched by a factor of
2, while the second basis vector is stretched by a factor of 3. So,
these vectors don’t move under this transformation; they are simply
scaled. You should contrast this example with the previous example   1
2 (12.92) 3 4 Can you find a similar set of vectors that are only
stretched by the transformation corresponding to B for the
transformation corresponding to this matrix? Good luck – we bet you
can’t find them! The vectors in the first example, the standard basis
vectors, are referred to as eigenvectors of the matrix A. In general, a
nonzero vector v is an eigenvector of a linear transformation T iff
there exists  2 F such that T v D v

(12.93)

In other words, the operation of T on v simply scales the vector v by
the scalar . Where did the name eigenvector come from? Well, the
Germans are responsible for quite a bit of the terminology and notation
of algebra, and “eigen” means “own,” as in “one’s own” or
“characteristic” in German. So, an eigenvector is a vector
characteristic to the matrix A. This implies that we could very well be
able to identify the matrix A given all of its characteristic vectors,
eigenvectors. This is true for the most part. We know from earlier that
a linear transformation is described entirely by how it acts on a basis
for the space. For the example A above, we’re fortunate to know
immediately from the description of A how it acts on the standard basis,
and so we pretty much know everything about A already. What if the basis
was different though? We saw earlier that there are several bases for a
vector space, so could it be that we understand the behavior of a matrix
on a different basis than the standard basis? Well, sure. Here’s an
example of such a scenario: Consider the matrix   2 1 BD (12.94) 0 3 
   1 1 Let’s apply this transformation to the vectors v1 WD and v2 WD
: 0 1

SECTION 12.3 Eigenvectors and Eigenvalues

 Bv1 D

2 1 0 3



2 1 0 3



1 0



1 1



 D

2 0



3 3



 D2

1 0



1 1



343

D 2  v1

(12.95)

D 3  v2

(12.96)

and  Bv2 D

 D

 D3

Interesting: so, Bv1 D 2  v1 and Bv2 D 3  v2 .   0 Now, let’s try
this out on the vector v WD . Then, we have 1  Bv WD B

0 1



 D

2 1 0 3



0 1



 D

1 3



and notice that if there were a number  such that         1 0
0 0 D D D 3 1 1 

(12.97)

(12.98)

then 1 D 0. So, there is no such number . This is equivalent to saying
the vector v is not like the vectors v1 and v2 , since the
transformation does not simply stretch v by some factor. The vectors v1
and v2 are the eigenvectors of the matrix B, while v is not. We refer to
the scale factors 2 and 3 as the eigenvalues of the eigenvectors v1 and
v2 , respectively. In general, the eigenvalue associated to an
eigenvector v is the scalar  appearing in the definition of an
eigenvector from earlier T v D v

(12.99)

Collectively, we refer to the eigenvectors and eigenvalues of a
transformation as its eigenstuff.2 There can only be two of these
eigenvectors for an operator on two-dimensional space, and in general,
there could be as many as n for an operator on n-dimensional space.
12.100

Exercise

Find the eigenstuff for the matrices   1 0 Projx WD 0 0

(12.101)

and 2 The eigenstuff is sometimes called the eigensystem of the
transformation. We acknowledge (and embrace) the informal choice of
terminology.

344

CHAPTER 12 Mathematical Tools for Quantum Computing II



 0 M WD (12.102) 1 2 3 Finding the eigenstuff for Projx shouldn’t be
too hard, while M might pose a bit more of a challenge. 2

Change of Basis Let’s keep running with the matrix B from our discussion
of eigenstuff. Although the standard basis is great, we’d like to
demonstrate that changing our basis to the eigenvectors of B might be
advantageous for several reasons. Well, we should probably check that
the eigenvectors of B do indeed form a basis for the vector space R2 .
Exercise

Verify that the eigenvectors     1 1 v1 D ; v2 D (12.104) 0 1
actually form a basis for R2 . Remember that this means we have to check
that v1 and v2 are linearly independent and that v1 and v2 span R2 . You
should do this by brute force first. Then, think about how you could
apply the theorem about the length of any basis for a vector space of a
certain dimension afterward. We know the standard basis consisting of
two vectors is indeed a basis for R2 , so that theorem ensures the
length of any list of basis elements for R2 is also two. Knowing this
and that the eigenvectors are either linearly independent or spanning
therefore guarantees they form a basis by the theorem.

12.103

We know from earlier that the matrix describing a linear transformation
depends on the bases we choose for the space. Let’s change the basis
we’re using from the standard basis to the basis of eigenvectors and see
how the matrix B changes as a result! To perform this operation, we need
to know how the transformation T corresponding to the matrix B acts on
the eigenvectors v1 and v2 in terms of v1 and v2 only, but we’ve already
figured this out! Recall that Bv1 D 2  v1 D 2  v1 C 0  v2 and that
Bv2 D 3v2 D 0  v1 C 3  v2 . So, we can make the matrix for the
transformation T with respect to the basis

SECTION 12.3 Eigenvectors and Eigenvalues

BR2 WD fv1 ; v2 g

345

(12.105)

of eigenvectors v1 and v2 following the procedure described in an
earlier section    2 0  M .T W R2 ! R2 /BR2 ;BR2 D (12.106) 0 3
Let’s abbreviate all of that with M .T / like we have before. We can see
that this matrix is diagonal; diagonal matrices are quite useful. To see
why, try the following exercise. 

 2 0 12.107 Exercise Find the square of the matrix M .T / D 0 3 formed
with respect to the basis of eigenvectors v1 and v2 (sometimes called an
eigenbasis), compute M .T /2 WD M .T /  M .T / Then, compute M .T /3 WD
M .T /  M .T /  M .T / Then, compute M .T /4 WD M .T /  M .T /  M .T
/  M .T / What’s going on? Can you compute M .T /100 ?



 2 1 12.108 Exercise Now, try this for the original matrix B WD 0 3
formed with respect to the standard basis vectors. That is, compute the
square of B. Then, compute B 3 . Then, compute B 4 . Can you compute B
100 ?

We’re willing to bet you figured out how to do the exercise regarding M
.T / and gave up while trying the exercise regarding B — anybody would.
The difference between M .T / and B is that M .T / is diagonal, while B
is not. The failure of B to be diagonal causes considerable difficulties
when multiplying, as you learned in the exercise. The question then
becomes: Can we always change our basis to one where the matrix we start
with ends up a diagonal matrix? Actually, no, not always.

346

CHAPTER 12 Mathematical Tools for Quantum Computing II

Exercise Think about why we can’t find a basis of eigenvectors for the
transformation described by the matrix   0 1 T WD 0 0

12.109

Matrices that have this special property are aptly named diagonalizable.
It is not so simple to give an explicit characterization of matrices
that are diagonalizable, so we won’t delve into this right now. Here we
make a connection between quantum mechanics and eigenstuff. Linear
operators with eigenvalues that are real numbers form a special class of
operators. In our review of quantum mechanics in a previous chapter, we
reviewed the measurement postulate of quantum mechanics; this postulate
states that any operator associated with a physically measurable
property will be Hermitian. We have not seen Hermitian operators just
yet, but we will find that they are a class of operators whose
eigenvalues are always real numbers, and so will be measurable. We’ll
see what Hermitian operators are and why they have such a remarkable
property in a little bit!

12.4

Further Investigation of Inner Products

Further investigation of the previously defined inner product reveals
some salient properties. The first of which is that of conjugate
symmetry, which states for all vectors u; v, hu; vi D hv; ui. So,
exchanging the vectors does not yield the same result, but the conjugate
instead. This might seem odd at first glance, but an example should help
convince us this should be the case.     i 2 Let u WD and v WD .
Then 1 i  hu; vi D

i 1

   2 ; D i  2 C 1  i D . i/  2 C 1  i D i

2i C i D

i

(12.110) and  hv; ui D

2 i

   i ; D 2  i C i  1 D 2  i C . i /  1 D 2i 1

i Di (12.111)

SECTION 12.4 Further Investigation of Inner Products

347

So, unless we conjugate, we don’t get the same number. We should
conjugate if we exchange the vectors in the inner product. 

   i 1 12.112 Exercise Let u WD and v WD . Find the inner 2 i product
hu; vi. Now, find the inner product hv; ui. Do you see why we have to
conjugate?

Conjugate symmetry also guarantees that the inner product of any vector
with itself is a real number. To see this, observe that for any vector
v, conjugate symmetry ensures that hv; vi D hv; vi (we exchanged v with
itself!), so the inner product of v with itself needs to be equal to its
conjugate. A complex number a C bi is equal to conjugate a bi iff a C bi
D a bi, which occurs iff b D b. But b D b only in the case when b D 0,
i.e., our complex number a C bi was a real number all along. The inner
product is also linear in the first argument. So, first of all, for any
two vectors u; v and w, the inner product satisfies the following
equation: hu C v; wi D hu; wi C hv; wi Let’s see an example of this
phenomenon. Let       1 0 1 uD ;v D ;w D 0 1 2

(12.113)

(12.114)

Let’s compute hu C v; wi:           1 0 1 1 1 hu C v; wi D
C ; D ; 0 1 2 1 2 WD 1  1 C 1  2 D 1  1 C 1  2 D 3

12.116

Exercise

Now, you compute         1 1 0 1 hu; wi C hv; wi D ; C ; 0 2
1 2

and check that it equals 1 C 2 D 3.

(12.115)

348

CHAPTER 12 Mathematical Tools for Quantum Computing II

We said that the inner product is linear in the first argument, so you
should be wondering how scalar multiplication manifests itself here. The
second part of this linearity in the first argument is that for any
scalar a and any vectors u and v, we have ha  u; vi D a  hu; vi
(12.117) To see this property in action, let  a D 2; u D

1 2



 ;v D

3 4

 (12.118)

Let’s compute the left-hand side          1 3 2 3 ha  u; vi
D 2  ; D ; 2 4 4 4 D 2  3 C 4  4 D 6 C 16 D 22

(12.119)

Exercise Compute the right-hand side, i.e., a  hu; vi and check that
it’s equal to 22.

12.120

You might wonder if hu; a  vi D a  hu; vi for all scalars a and
vectors u and v. Check that this is not true in the following exercise.
Exercise Check that it is not true that hu; a  vi D a  hu; vi for all
scalars a and vectors u and v by finding a scalar a and two vectors u
and v such that hu; a  vi ¤ a  hu; vi. In fact, you can prove using
the axioms listed later on that for all scalars a and vectors u and v,
it is true that hu; a  vi D ahu; vi. This property of the inner product
is sometimes called conjugate homogeneity in the second argument. 12.121

The final property of the inner product is known as
positive-definiteness: for all vectors v, hv; vi  0 and hv; vi D 0 iff
v D 0. Let’s see why this is true from a more abstract perspective. Let
v D T v1 v2 : : : vn be a vector. Then hv; vi WD v1  v1 C v2  v2 C
::: C vn  vn (12.122) Recall that the product of a complex number with
its conjugate is always a non-negative real number (i.e., greater than
or equal to 0), so vi  vi is a

SECTION 12.4 Further Investigation of Inner Products

349

real number for each i 2 f1; :::; ng. Well, then the sum of a (finite)
bunch of non-negative real numbers is a real number, so the sum v1  v1
C v2  v2 C ::: C vn  vn

(12.123)

is still a non-negative real number, i.e., is greater than or equal to
0. 12.124 Exercise Convince yourself that the expression above is 0 iff
the vector v is the zero vector, i.e., has all zero entries.

So, we’ve shown that for any vector v, hv; vi  0 and that hv; vi D 0
iff v D 0. Exercise Notice that we never said that the inner product
satisfies linearity in the second argument! It is true, however, and
your task is to prove it using the axioms that we’ve already listed and
verified. Linearity in the first argument will be crucial for your
proof.

12.125

The Kronecker Delta Function as an Inner Product While discussing the
idea of an orthonormal basis for a vector space earlier, we mentioned
the idea that the mathematical description of an orthonormal basis could
be described in terms of the Kronecker delta function ı. The Kronecker
delta function ı has such a simple description that you can’t imagine
why it could possibly be named after anyone – although Kronecker isn’t
complaining. 12.126

Definition The Kronecker delta function

For a set f1; 2; :::; ng ( ı.i; j / D 1 if i D j ı.i; j / D 0 if i ¤ j
This should look familiar! Recall our definition of orthonormal basis
vectors from earlier. So, we can refer to an orthonormal set S of
vectors as a set of vectors such that the restriction of the inner
product to S is the Kronecker delta function! 12.127

Exercise

Check that the entries of the identity matrix can be

350

CHAPTER 12 Mathematical Tools for Quantum Computing II

described by the Kronecker delta function. More precisely, check that we
can define the identity matrix I entry-wise as Iij WD ı.i; j /.

12.5

Hermitian Operators

A linear operator (interchangeably, matrix) is referred to as Hermitian
iff it is equal to its conjugate transpose (defined above). Hermitian
operators are crucial in quantum mechanics. We often want to measure a
quantity associated with some state. Often the quantity we’re after is
the eigenvalue of an operator, and so we’d like for that eigenvalue to
be a real number in order to effectively measure it.

Why We Can’t Measure with Complex Numbers A subtle point worth
mentioning is that we can’t perform a measurement with complex numbers.
Suppose you wanted to figure out which of the numbers 0 or i is bigger?
Then, you would either have to decide that i D 0, 0 &lt; i or that i
&lt; 0. Of course, we won’t choose i D 0 because, if we do, then we
could multiply each side of the equation i D 0 by i and find that 1 D 0!
Let’s try the choice 0 &lt; i. If we choose that 0 &lt; i , then
multiplication by i on each side yields the inequality i 0<i i
(12.128)
But then
0 < i  i D i2 D

1

(12.129)

In summary, we have deduced that 0 < 1 from our assumption that 0 < i.
Since 0 < 1 does not make sense, we are left to conclude that our original
assumption that 0 < i does not make sense.
So, what if we choose that i < 0? Subtract i from both sides, revealing
i

i <0

i

(12.130)

So,
0<
Multiplying both sides by i reveals

i

(12.131)

SECTION 12.5 Hermitian Operators

0  . i/ <

i  . i/

351

(12.132)

But
i  . i / D . 1/  i  . 1/  i
. 1/. 1/  i  i D 1  i 2 D

(12.133)

1

(12.134)

So, the inequality 0  . i / < i  . i / really means 0 < 1. This does not
make sense either, and so we must conclude that the original hypothesis that
i < 0 does not make sense. So, what we’re discovering is that neither choice
of order, i.e., neither 0 < i nor i < 0 makes sense. Assuming either such
order reveals that 0 < 1, which is simply not true. We are left to conclude
that there is no acceptable way of ordering the complex numbers.
To make this more precise, suppose you want to come up with an order for
the complex numbers that satisfies the following reasonable conditions that
we are familiar with from our experience with usual real numbers:
 Trichotomy: For all complex numbers x; y, we have a trichotomy:
either x < y, x > y or x D y.  Additivity property: For all complex
numbers x; y; z, if x &lt; y, then x C z &lt; y C z.  Multiplicative
property: For all complex numbers x; y; z, if 0 &lt; z, then x &lt; y
implies xz &lt; yz. Now, let’s very carefully prove that the choice 0
&lt; i contradicts at least one of the above axioms. Since 0 &lt; i,
using the third (multiplicative) property stated above, we see that 0
&lt; i H) 0  i &lt; i  i D i 2 D

1

(12.135)

Although the fact that we have deduced that 0 &lt; 1 from our assumption
that 0 &lt; i is disturbing, it technically does not violate any of the
axioms above. Using the second (additivity) property above, the
inequality 0 &lt; 1 allows us to deduce 0&lt;

1 H) 0 C 1 &lt;

1C1D0

(12.136)

So, 1 &lt; 0. This is also disturbing, but is not a direct violation of
any of the axioms above. Now, we invoke the third (multiplicative)
property a final time yielding 1 &lt; 0 H) 1  i &lt; 0  i D 0

(12.137)

352

CHAPTER 12 Mathematical Tools for Quantum Computing II

Then, we have i &lt; 0, but our original assumption was that 0 &lt; i .
This violates the first (trichotomy) property above! Exercise Try to
figure out what goes wrong with defining i &lt; 0 in a similar fashion.

12.138

So, we really want these measurements to be real numbers, or else we
have no way of making sense of them. The question then becomes: Why is
it that Hermitian matrices have real eigenvalues?

Hermitian Operators Have Real Eigenvalues Despite the ease with which we
may verify that a matrix is equal to its conjugate transpose, a
different but equivalent definition of Hermitian makes the proof that
Hermitian matrices have real eigenvalues quite simple. We could also
define a linear operator T W V ! V to be Hermitian iff it is
self-adjoint, where we say: 12.139

Definition Adjoint of a matrix

The adjoint of a matrix T is a matrix T  such that for all vectors u; v
2 V hT u; vi D hu; T  vi. Then, that T is self-adjoint means that T D T
 and so for all vectors u; v 2 V , hT u; vi D hu; T vi. Notice that the
adjoint of an operator is precisely its conjugate transpose! So, to say
that an operator is self-adjoint is to say that it equals its conjugate
transpose. 12.140

Adjoint is conjugate transpose

The adjoint of a linear operator is its conjugate transpose. Now, if v
is an eigenvector with eigenvalue  of a Hermitian matrix T , then we
may further conclude that hT v; vi D hv; T vi

(12.141)

That v is an eigenvector of T with eigenvalue  means that T v D v, so
we may substitute v for T v in the equation hT v; vi D hv; T vi,
yielding hv; vi D hv; vi

(12.142)

SECTION 12.6 Unitary operators

353

Our intuition now is to factor out , which causes something interesting
to happen. By homogeneity of the inner product in the first argument and
conjugate homogeneity in the second argument, “factoring out ” yields
the new equation hv; vi D hv; vi (12.143) Now, we’d like to “divide by
hv; vi” on both sides and call it a day, but how do we know that it
isn’t zero? Well, we started by assuming v was an eigenvector of T , and
the definition of an eigenvector requests that v not be zero. Then, we
apply the definiteness property of the inner product to ensure that,
since v is not zero, the inner product of v with itself, i.e., hv; vi,
is not zero either. Thus, D (12.144) Remember what it means for a
complex number to equal its complex conjugate? Exactly — then it’s a
real number after all! Exercise It’s worth noting that any real
symmetric matrix (symmetric matrix with real entries only) is Hermitian.
Can you see why?

12.145

Hopefully, this foray into the proof of this theorem makes you realize
that all of the axioms we request in these definitions are truly
necessary! Do you see where we used each and every one of the axioms?

12.6

Unitary operators

You’ve surely encountered the zoo of matrices describing quantum logic
gates within chapter 3 and listed in chapter 15. Those matrices are
special because they are unitary. Unitary matrices preserve the length
of vectors. They are so named because unit vectors remain unit vectors
after an application of a unitary matrix. More precisely, 12.146

Definition Unitary Operator

A linear operator U W V ! V is unitary iff for all vectors x; y 2 V ,
hx; yi D hUx; Uyi i.e., U preserves inner products.

354

CHAPTER 12 Mathematical Tools for Quantum Computing II

It is interesting to note that we could equivalently define a unitary
operator (matrix) U W V ! V to be a matrix whose conjugate transpose is
its inverse, i.e., U D U 1 (12.147) So, U U D U U  D I

(12.148)

Nothing we’ve said so far directly implies that a unitary operator
preserves the length of any vector it operates on, so let’s verify this
in an exercise. Exercise Verify that a unitary operator U preserves the
length of any vector v that it operates on by using the definition given
above. Use p the fact that the length ofpthe vector v is equal to hv;
vi, and compare the original length of v, i.e., hv; vi, to the length of
v after U has operated, i.e., p hU v; U vi.

12.149

12.7

The Direct Sum and the Tensor Product

We might want to build bigger vector spaces from collections of vector
spaces we already have. There are two popular ways of doing this. One
way is the direct sum, the other the tensor product. We’ve already seen
the tensor product in the context of taking the tensor product of two
vectors, or even two matrices. There is a relationship between that
previously defined operation and the operation we’re about to describe.

The Direct Sum The first point we’d like to emphasize is that the direct
sum operates on vector spaces, not numbers, vectors or matrices
(although the astute reader already considers all of these to be simply
linear transformations!). The same is true for the tensor product.
Specifically, the direct sum is a binary operation that accepts two
vector spaces as input and yields another, usually “bigger,” vector
space as output. Let’s see an example. Consider the one-dimensional
vector space R and a copy of itself – so, two copies of R. The direct
sum of R with itself is written R˚R

(12.150)

SECTION 12.7 The Direct Sum and the Tensor Product

 113

and is defined to be  R ˚ R WD

x y



 W x 2 R; y 2 R

(12.151)

Hold on – that’s just the Cartesian product R  R of R and R! Exercise
Recall the definition of the Cartesian product R  R and compare it to
the direct sum R ˚ R.

12.152

Why do we have two names for the same thing? Well, they’re not actually
the same thing because the direct sum R ˚ R has more structure. In
particular, the direct sum R ˚ R is a vector space (over R), where the
Cartesian product R  R is simply a set. To further elaborate on this
idea, consider the sets A WD fa; b; cg and B WD fd; eg. We may create
their Cartesian product A  B WD f.x; y/ W x 2 A; y 2 Bg D f.a; d /; .a;
e/; .b; d /; .b; e/; .c; d /; .c; e/g

(12.153)

Now, we ask the question: What is the direct sum A ˚ B? Well, at first,
we have    x A ˚ B WD W x 2 A; y 2 B (12.154) y simply following the
definition from above. A cursory glance might convince us that the issue
is that the Cartesian product has row vectors and the direct sum has
column vectors, but when discussing sets, it doesn’t matter if we’re
using row or column vectors. The question is illuminated by a further
question: How is A ˚ B a vector space? And over which field? You see, in
order to define A ˚ B as a vector space, you have to give it additional
algebraic structure so that it is an abelian group and has a field
action by some specified field. Currently, it has neither of these.
You’re invited to ponder this for a moment. How would you define the
addition of two elements of A ˚ B? Whatever way you decide has to allow
for the addition of the specific T T elements a d and b e . Sure, we
could say 

a d



 C

b e



 D

aCb d Ce

 (12.155)

356

CHAPTER 12 Mathematical Tools for Quantum Computing II

but what do a C b and d C e even mean? Remember, a; b; d and e are just
letters. They have no numerical meaning whatsoever. So, the big idea is
that it’s perfectly reasonable to form Cartesian products of any two
sets you like. For example, the Cartesian product of the set COLORS WD
fchartreuse; magenta; periwinkleg

(12.156)

and the set ANIMALS WD fcat; dog; aardvarkg

(12.157)

is the new set COLORS  ANIMALS WD f.x; y/ W x 2 COLORS; y 2 ANIMALSg
(12.158) which ends up being 8 9 &lt; (chartreuse, cat), (chartreuse,
dog), (chartreuse, elephant), = (magenta, cat), (magenta, dog),
(magenta, elephant), : ; (periwinkle, cat), (periwinkle, dog),
(periwinkle, elephant) (12.159) which is just a set, and not a vector
space. Whereas the direct sum R ˚ R is, a priori, the set    x R ˚ R
WD W x 2 R; y 2 R (12.160) y which has a natural interpretation as being
a vector space over the field R, since we can define the addition (to
get the abelian group structure) to be usual vector addition and the
field action to be usual scalar multiplication. We would also like to
mention that since the direct sum of two vector spaces is itself a
vector space, it has a dimension. It turns out that the dimension of the
direct sum of two vector spaces is the sum of their dimensions, hence
the name direct “sum.” More specifically, for any two vector spaces V
and W both over the same field F, dim.V ˚ W / D dim.V / C dim.W / 12.162

Definition The direct sum of two vector spaces

The direct sum of vector spaces V and W is the vector space   v V ˚
W WD w

(12.161)

SECTION 12.7 The Direct Sum and the Tensor Product

12.163

357

Dimension of direct sum dim.V ˚ W / D dim.V / C dim.W /

(12.164)

The Tensor Product Now, we’ll discuss the tensor product. What is
remarkable about the tensor product of two vector spaces is that it is
entirely described by the “tensor product” of the basis elements for
each. What we mean by this is that if we have two vectors spaces V and W
both over the same field F and with bases BV D fv1 ; :::; vm g and BW D
fw1 ; :::; wn g, respectively, then the tensor product of V and W ,
denoted V ˝ W is a vector space with basis given by B V ˝W WD fv1 ˝ w1 ;
v1 ˝ w2 ; :::; v1 ˝ wn ; : : : ; vm ˝ w1 ; vm ˝ w2 ; : : : ; ˝vm ˝ wn g
(12.165) You might recognize that all of the possible pairs of tensor
products of the basis vectors of V with the basis vectors of W appear in
the “tensor product” of the bases of V and of W . In fact, this is
always the case! That is, if we have two vector spaces V and W both over
the same field F and we’d like to find their tensor product V ˝ W , we
can at least determine the basis of V ˝ W by tensoring all of the
possible pairs of basis vectors of V and W . Although this is a
convenient fact, it does require a little bit of work to prove; it is
often referred to as The Tensor Product Basis Theorem, emphasizing that
it is a result to be proved. What we would have to show is that, in
fact, the proposed basis for V ˝ W consisting of all possible tensor
products of pairs of basis vectors from V and W is actually a basis,
i.e., all of those tensor products are linearly independent and span V ˝
W . This is believable, given that the basis vectors from each of V and
W are linearly independent amongst themselves and they span their
respective spaces. However, we would like you to think about why this
requires a proof! Anyway, we’ll avoid defining the tensor product of two
vectors from an axiomatic perspective here, and instead give a
basis-centric view of the idea. If you’ve never seen the tensor product
of two vector spaces before, it’s fair to think like this for the
moment: Given two vector spaces V and W with bases BV and BW ,
respectively, we define their tensor product V ˝ W to be the vector
space with basis equal

358

CHAPTER 12 Mathematical Tools for Quantum Computing II

to the “tensor product” of their bases, i.e., the basis BV ˝W consisting
of the tensor products of all possible pairs of basis elements of V and
W , as described above. Mathematicians reading this might be frustrated,
but we’re simply trying to give a working definition. Readers interested
in why there might be any fuss about this definition of a tensor product
are invited to investigate more mathematical treatments of the tensor
product from the perspective of bilinear maps, and even further,
category theory!3 Now, a word about notation. You might come across some
fancy ways of writing the direct sum or tensor product of several copies
of the same vector space. For example, L H n (12.166) is just a fancy
way of writing H ::: ˚ H… „ ˚ƒ‚

(12.167)

n times

Another way to state this is: the direct sum of n copies of the vector
space H . This can also be written as M H (12.168) n

A similar notation is in place for tensor products H

N

n

WD H ::: ˝ H… „ ˝ƒ‚

(12.169)

n times

and O

H

(12.170)

n

Both of these notations refer to the n-fold tensor product of H , i.e.,
the tensor product of n copies of the vector space H . These notations
for the tensor product of several H s arise when notating a quantum
register, i.e., a collection of qubits, as we’ll see at the culmination
of this chapter with the definition of a Hilbert space. 3 Category

theory defines the tensor product of two vector spaces via its universal
property. This definition offers an elegant and sophisticated view of
the tensor product which eases proofs and offers insight into the
behavior of the tensor product as it interacts with other vector spaces.
This construction also instructs the definition of the tensor product of
more general objects than vector spaces, like modules!

SECTION 12.7 The Direct Sum and the Tensor Product

359

We can also take the tensor product of two operators. Thinking of each
operator as a linear transformation, and thus a matrix, allows us to
take their tensor product as we did earlier in this chapter! For
example, given the operators on two-dimensional complex space C2 ,   1
0 I WD (12.171) 0 1 and

 X WD

0 1 1 0

 (12.172)

we may form their tensor product     1 0 1X 0X I ˝ X WD ˝X D 0 1
0X 1X     1 0 0 1 0 1 0 B 1 1 0 C    1 0  C DB @ A 0 1 0 1
0 1 1 0 1 0    0  10 11 00 01 B  11 10   01 00  DB @
00 01 10 11 01 00 11 10    1 0 0  0 1 0 0 0 B C B 1 1 0 0 0
    CDB DB @ A @ 0 0 0 0 1 0 0 1 0 0

1 C C A 1 0 0 0

0 0 0 1

1 0 0 C C 1 A 0

(12.173)

Summarizing the result of our computation, we’ve created an operator
that now operates on four-dimensional complex space C4 with the
following effect .I ˝ X/.j00i/ D .I ˝ X /.j0i ˝ j0i/ 0 10 0 1 0 0 B 1 0
0 0 CB CB DB @ 0 0 0 1 A@ 0 0 1 0 D j0i ˝ j1i D j01i 12.175

Exercise

1 0 1 0 C B 0 C B 1 D 0 A @ 0 0 0

1 C C A (12.174)

Find the tensor product X ˝ I . Is it the same as I ˝ X?

360

CHAPTER 12 Mathematical Tools for Quantum Computing II

Note that we constructed a 4  4 matrix as the tensor product of two 2 
2 matrices, which makes sense given our earlier discussion of how the
tensor product of an .a  b/ matrix and a .c  d / matrix is a .a  c/ 
.b  d / matrix. Curious readers might try to build the quantum
operators discussed in chapter 3 by taking tensor products of
two-dimensional operators. Beware: it’s not easy! In fact, you cannot
build CNOT by taking the tensor product of two two-dimensional
operators.

12.8

Hilbert Space

The modern definition of a quantum computer laid out in the text
postulates that a qubit is modeled by a two-dimensional complex Hilbert
space, so we include the formal definition here. However, before we can
do so, we need to have a brief discussion of the notions of a metric on
a vector space, Cauchy sequences, and finally, the idea of completeness
of a vector space.

Metrics, Cauchy Sequences and Completeness By a metric on a vector
space, we mean that we can measure (hence, “metric”) the distance
between two vectors u and v by computing the norm of their difference,
i.e., hu v; u vi (12.176) Exercise Check that the distance between two
vectors u and v as defined above is zero iff u D v, equivalently, u v D
0.

12.177

At first glance, a Cauchy4 sequence can be thought of as “a sequence of
numbers whose terms get as close as we like, given that we look far
enough.” Before we investigate Cauchy sequences, we should understand
the notion of convergence of a sequence of numbers. Here is an example
of a Cauchy sequence of real numbers f W N ! R:

4 This

sequence is named after Augustin-Louis Cauchy.

SECTION 12.8 Hilbert Space

f .1/ f .2/ f .3/ f .4/ :: :

1 2 1 4 1 8 1 16

f .n/

1 2n

361

:: :

We can see that these numbers are getting closer and closer to the
number 0, and in fact, we can make them as close to 0 as we like by
choosing terms sufficiently far along in the sequence. Exercise Verify
for yourself that we can make the numbers in the sequence above as close
to the number 0 as we like by finding the number n such that f .n/ D 21n
is close to 0 within an error of 0:000001. In other words, figure out
how far we need to go in the sequence before the terms differ from 0 by
only 0:000001 or less. It might help to think of 0:000001 as 1016 .

12.178

We say that this sequence of numbers converges to the number 0. We can
express that the above sequence f W N ! R of real numbers defined by f
.n/ D 21n converges to 0 more mathematically by saying, for all  &gt;
0, there exists N 2 N such that for all n 2 N, if n &gt; N , then jf .n/
0j &lt; . You actually found the “N ” in the previous mathematical
description of the convergence of a sequence to 0 in the above exercise!
Of course, there is nothing special about this particular sequence, nor
the number 0. We can play this game with any sequence and number. In
general, we say that a sequence f W N ! R converges to a number L (L
stands for “limit”) iff for all  &gt; 0 there exists N 2 N such that
for all n 2 N, if n &gt; N , then jf .n/ Lj &lt; . Again, intuitively,
we should think of this as saying “A sequence of numbers converges to a
number L iff we can make those numbers get as close to L as we like
simply by taking terms further along in the sequence.” Now, a Cauchy
sequence is a special type of sequence whose terms, as we said earlier,
“get as close as we like, given that we look far enough.” Let’s revisit
the previous sequence

362

CHAPTER 12 Mathematical Tools for Quantum Computing II

f .1/ f .2/ f .3/ f .4/ :: :

1 2 1 4 1 8 1 16

f .n/

1 2n

:: :

Observe the following phenomenon: How far apart are the terms f .1/ and
f .2/? Well, ˇ ˇ ˇ ˇ ˇ1 1ˇ ˇ1ˇ ˇ ˇDˇ ˇD 1 jf .1/ f .2/j D ˇ 2 4ˇ ˇ4ˇ 4
so they’re 14 apart. How far apart are the terms f .2/ and f .3/? You
should 1 check that they’re 18 apart. f .3/ and f .4/? Now, they’re 16
apart! Hmm... So, it seems that as we go further along in the sequence,
pairs of terms get closer and closer together. Let’s make this
mathematically precise. We say that a sequence f W N ! R is Cauchy iff
for all  &gt; 0, there exists N 2 N such that for all m; n 2 N, if m; n
&gt; N , then jf .m/ f .n/j &lt; . Exercise Convince yourself that this
precise mathematical formulation of a Cauchy sequence agrees with our
intuitive statement about terms getting closer further along in the
sequence. Then, check that the sequence f .n/ D 21n is in fact a Cauchy
sequence.

12.179

So, we’re convinced that the above sequence is Cauchy. Now, we can ask
the question as to whether a sequence of numbers converges to a number
already in our set. You might be wondering how a sequence of numbers
could ever possibly converge to something not already in our set...
Well, let’s look at the sequence f .n/ D 21n once more. Suppose we’re
only considering numbers greater than 0 for the moment. In other words,
we’re working with the numbers .0; 1/ WD fx 2 R W x &gt; 0g So, the
numbers in the set we’re considering cannot be equal to 0. Well, then
the previous sequence has the curious property that it is Cauchy and it
converges, but not to any number in the space we’re working in, because

SECTION 12.8 Hilbert Space

363

it converges to 0, which is not a number in our set! This is a failure
of the set .0; 1/ to be what we refer to as complete. Formally, we say
that a set is complete iff any Cauchy sequence of elements in the set
converges to an element in the set. We often relax this statement to
“Cauchy sequences converge” when the context is understood. Now, we can
generalize all of these ideas by allowing ourselves to measure the
distance between two objects using a more general notion of an absolute
value. The absolute value is actually a special case of a more general
phenomenon known as a metric: 12.180

Definition Definition of a metric

A metric is a binary function d W S  S ! R from the Cartesian product
of two copies of a set S to the real numbers satisfying the following
properties:  For all x; y 2 S, d.x; y/  0  Definiteness: For all x; y
2 S , d.x; y/ D 0 iff x D y  Triangle inequality: For all x; y; z 2 S ,
d.x; z/  d.x; y/ C d.y; z/ The absolute value j  j W R ! R is in fact
a metric, as we invite you to check: Exercise Check that the absolute
value j  j W R ! R is actually a metric by verifying that it satisfies
the above three properties. Also, convince yourself that the third
property really should be called the triangle inequality! 12.181

But we said that a metric is a more general notion! What’s a more
general metric? Well, consider the following way of measuring the
“distance” between two vectors: Given two vectors u and v in R2 , we
could measure the distance between them by taking the (L2 ) norm of
their difference (as vectors, that is), i.e., d.u; v/ WD jju vjj2 : But
a moment’s thought makes us realize that this is simply taking the
square root of the inner product of the vector difference with itself,
i.e., p jju vjj2 D hu v; u vi There we have it! A very general notion of
a metric. We can now define a metric on any vector space with an inner
product in the following way. For any vector space V with inner product
h; i, define the metric

364

CHAPTER 12 Mathematical Tools for Quantum Computing II

d WV V !R

(12.182)

via d.u; v/ WD

p

hu

v; u

vi

(12.183)

We invite you to check that this definition does in fact satisfy the
criteria for a metric from earlier. 12.184

Exercise

Check that the metric we defined above d WV V !R

via d.u; v/ WD

p

hu

v; u

vi

is actually a metric by checking that it satisfies the criteria laid out
earlier.

We say then that the inner product induces a metric on the vector space
V , or that the metric is the metric induced by the inner product.

An Axiomatic Definition of the Inner Product Let us touch briefly upon
the idea of an axiomatic definition of an inner product. The definition
given previously in this text serves us well, but it turns out that
there are more exotic ways of taking the inner product of two vectors.
In fact, we could possibly be working in a vector space where the
vectors are... matrices or something some other mathematical object.
There are vector spaces, for example, whose “vectors” consist of all
continuous functions f W R ! R, where the inner product of two “vectors”
(really, functions!) f and g is defined to be 1

Z hf; gi WD

f .x/g.x/dx

(12.185)

0

Yes, inner products, and vectors spaces for that matter, can be quite
otherworldly. So, we want an axiomatic framework for them that captures
the essence.

SECTION 12.8 Hilbert Space

12.186

365

Definition Axiomatic definition of an inner product

An inner product h; i on a vector space V over a field F (where F is
either R or C) is a binary function h; i W V  V ! F satisfying the
following properties:  Conjugate symmetry: For all u; v 2 V , hu; vi D
hv; ui  Linearity in the first argument: For all a 2 F; u; v; w 2 V ,
ha  u; vi D a  hu; vi and hu C v; wi D hu; wi C hv; wi 
Positive-definiteness: For all v 2 V , hv; vi  0 and hv; vi D 0 iff v D
0 Exercise With the axioms laid out above, you’re invited to verify that
the inner product which we have been using does in fact satisfy these
axioms.

12.187

Finally, we’re able to state the precise definition of a Hilbert space!

The Definition of Hilbert Space 12.188

Definition Definition of Hilbert space

A Hilbert space is a vector space H over either the field of real or
complex numbers equipped with an inner product h; i that is a complete
metric space with respect to the metric induced by the inner product.

366

CHAPTER 12 Mathematical Tools for Quantum Computing II

The definition of a Hilbert space is the culmination of this chapter,
and we’d like to mention briefly how Hilbert spaces arise in quantum
computing.5 We care about Hilbert spaces over the field C of complex
numbers, and the following discussion refers only to such spaces.

12.9

The Qubit as a Hilbert Space

One of the central concepts of quantum computing is that a qubit can be
represented as a two-dimensional complex Hilbert space.6 We denote a
Hilbert space with the letter H, or sometimes more fancily with H .
12.189

A qubit is a vector space

A qubit is represented by a vector space — more specifically, a Hilbert
space! We sometimes call the Hilbert space representing the qubit the
state space. A state in the state space is a vector in the state space
with L2 norm 1. So, a state is on the Bloch sphere – refer to chapter 3.
For example, the familiar vectors j0i and j1i are states in the
2-dimensional Hilbert space (state space) H , which represents one
qubit. In fact, j0i and j1i are an orthonormal basis for H , as you
verified earlier in our discussion of orthonormal bases, and so every
vector in the state space is a linear combination of these two vectors
with L2 norm 1. In the terminology of quantum mechanics, every state is
a superposition of these two states! We refer to a collection of n
qubits as a quantum register and often notate it as H ˝ : : : ˝ H…
(12.190) „ ˝ H ƒ‚ n times

It turns out that the tensor product of Hilbert spaces is another
Hilbert space, although it will have a greater dimension in general!
Exercise Think about why the dimension of the tensor product of two
two-dimensional Hilbert spaces is 4. Then, think about why the dimension
of the tensor product of three two-dimensional Hilbert spaces is 8 – not
6! Then, figure out why the dimension of the tensor product of n
two-dimensional 12.191

5 The 6 We

name Hilbert space honors the mathematician David Hilbert. take our
motivation from page 15 of Yuri Manin’s seminal paper \[182\].

SECTION 12.9 The Qubit as a Hilbert Space

367

Hilbert spaces is in fact 2n . It might help to think of what the basis
for the tensor product space is.

For example, if we have two qubits H and H , each with orthonormal basis
BH D fj0i ; j1ig (12.192) then the quantum register H ˝H

(12.193)

is a Hilbert space of dimension 4 (as you checked in the exercise above)
with basis BH ˝H D fj0i ˝ j0i ; j0i ˝ j1i ; j1i ˝ j0i ; j1i ˝ j1ig D
fj00i ; j01i ; j10i ; j11ig;

(12.194)

where we recall from earlier that j00i is just a convenient renaming of
the tensor product j0i ˝ j0i, i.e., 0 1 1     B 1 1 0 C C j00i WD
j0i ˝ j0i D ˝ DB (12.195) @ 0 0 0 A 0 and the vectors j01i ; j10i ; j11i
are defined similarly. Exercise Figure out the basis BH ˝3 for H ˝3
where H has basis BH D fj0i ; j1ig: It should consist of 23 D 8 vectors
by the previous exercise. Can you figure out the basis for H ˝n ?

12.196

12.197

A quantum register is a tensor product

A quantum register consisting of n qubits is a 2n -dimensional tensor
product of vector spaces!

368

CHAPTER 12 Mathematical Tools for Quantum Computing II

Summary of the relationship between quantum computing and linear algebra

12.198

 A qubit can be represented by a two-dimensional complex Hilbert space.
The state of the qubit is represented by a vector in the Hilbert space.
 More specifically, the vectors representing the states of a qubit have
an L2 norm of 1.  The quantum register consisting of n qubits is a 2n
-dimensional complex Hilbert space composed of the n-fold tensor product
of the two-dimensional Hilbert spaces representing the qubits.  A
computational basis vector of the space represents a definite
computational state of the qubit.  A superposition of states is a
linear combination of the computational basis vectors.  Quantum logic
gates are unitary operators, which act on the state space. Since unitary
operators preserve the norm of the vectors they act on, states are
transformed to new states and not to just any vector in the space. Thus,
we can build quantum circuits using unitary operators.  Measurement is
performed by projection operators And so our review of linear algebra
culminates with the table in Figure 12.3. Readers wanting a deeper
understanding of linear algebra are encouraged to read:  Sheldon
Axler’s Linear Algebra Done Right \[20\], where emphasis is placed on
the theory and proof technique common to linear algebra, a sophisticated
vantage point of matrices, the spectral theorem (which determines when
the eigenvectors of a linear operator form a basis), and the determinant
are presented.  Michael Artin’s Algebra \[18\] caters to a more
mathematical audience. It begins with a wonderful discussion of
elementary matrices and their role in Gaussian elimination and offers
great perspective for group theory.  Gilbert Strang’s textbook Linear
Algebra and its Applications \[264\] is helpful for applications of
linear algebra to the sciences and is supplemented by free MIT
OpenCourseWare material.  See Appendix A and B of Rieffel and Polak’s
textbook, Quantum Computing, A Gentle Introduction, for connections
between quantum me-

369

SECTION 12.9 The Qubit as a Hilbert Space Quantum Computing

Linear Algebra

Example

qubit

two-dimensional complex Hilbert space

H D spanC fj0i ; j1ig

n-qubit quantum register

n-fold tensor product of two-dimensional complex Hilbert spaces

H ˝n

state space

vectors with L2 norm 1 (Bloch sphere)

fv 2 H W hvjvi D 1g

definite state

orthonormal basis vector

j0i ; j1i

superposition of states

linear combination of orthonormal basis vectors with L2 norm 1 (on the
Bloch sphere)

quantum logic gates

unitary operators

measurement operators

projection operators

p1 2

p1 2

j1i

0 1 1 0



j0i C

 XD



1 0 0 0



Figure 12.3: Relationship of quantum computing to linear algebra





 



chanics and probability theory as well as a treatment of the Abelian
hidden subgroup problem \[236\]. For readers interested in learning more
about abstract algebra, here are additional texts: - John Fraleigh’s A
First Course in Abstract Algebra \[117\] - Dummit and Foote’s Abstract
Algebra \[97\] - Joseph Rotman’s Advanced Modern Algebra \[243\] A
whimsical introduction to category theory can be found in the text
Conceptual Mathematics: A First Introduction to Categories \[166\] by F.
William Lawvere and Stephen H. Schanuel. Readers interested in acquiring
a refined definition of the tensor product should look up Tai-Danae
Bradley’s blog Math3ma \[54\]. More adventurous readers are invited to
read Bradley’s book What is Applied Category Theory? \[55\] to see that
category theory is not simply a rephrasing of mathematics and is in fact
quite useful for things like chemistry and natural language processing!
Emily Riehl’s Category Theory in Context \[237\] is a helpful
introduction to category theory for advanced undergraduates and graduate
students.

CHAPTER

13 Mathematical Tools for Quantum Computing III 13.1 13.1

Boolean Functions

Definition

Boolean function

A Boolean function f is a function from a Cartesian product f0; 1gn !
f0; 1gm where f0; 1gn denotes the n-fold Cartesian product of the set
f0; 1g with itself, i.e., f0; 1gn WD f0; 1g  :::  f0; 1g „ ƒ‚ … n
times

Cartesian products and functions are discussed in chapter 11, if you
want to brush up on these terms. Boolean functions arise naturally in
computing. For example, the Deutsch-Jozsa Algorithm discussed in chapter
7 involves the four Boolean functions f0 ; f1 ; fx ; fx

(13.2)

each with domain and codomain f0; 1g. So, in the case of these four
functions, n D 1 and m D 1 when we compare them to the definition of a
Boolean function given above. Other examples of Boolean functions
include NOT , AND, OR and XOR.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_13

371

372

CHAPTER 13 Mathematical Tools for Quantum Computing III

Interest Rate

Number of Times Compounded Annually

Amount in One Year

percent

1 time per year

2 dollars

D 50 percent

2 times per year

2:25 dollars

100 1 100 2

100 3

percent

3 times per year

 2:37 dollars

100 4

percent

4 times per year

 2:44 dollars

100 5

percent

5 times per year

 2:49 dollars

100 100

percent

100 times per year

 2:70481 dollars

100 1

percent

1 times per year

e dollars

Figure 13.1: The Banker’s experiment

13.2

Logarithms and Exponentials

We recall some of the basic facts about logarithms here. We first
consider the natural logarithm with a base of the number e. The number e
is approximately 2:71 and appears in a menagerie of mathematical and
scientific contexts. One interesting way to acquire e is via the
following banker’s thought experiment: Invest 1 dollar in a bank account
at an interest rate of 100 1 percent annually (once per year) and in one
year, you’ll earn 1 dollar, and thus have a total of 2 dollars after one
year. Now, allow yourself to accrue interest twice a year, but at the
compromised rate of 100 2 D 50 percent. After the first six months,
you’ll earn 50 cents, since 50 cents is 50 percent of the invested 1
dollar. After another six months, you’ll earn 50 percent of the 1:50
dollars you have, and end up with 2:25 dollars. This is more than if you
compounded only once per year. If you compound three times per year, you
have the compromised rate of 100 3 percent. You earn a little bit more
at this rate, as you can check. If you allow yourself to compound
“infinitely many times” at the compromised rate of “ 100 1 ” percent,
you’ll end up with e dollars! This is summarized in the table in Figure
13.1. ln WD loge W .0; 1/ ! . 1; 1/ where “ln” is the natural logarithm.
The following equivalence guides all of the facts to come:

(13.3)

SECTION 13.2 Logarithms and Exponentials

10

373

y D ex

5

y D ln.x/

5

5

10

5

Figure 13.2: Graphs of the logarithm and exponential

13.4

Equivalence of logarithm and exponential ln.y/ D x () e x D y

Some first properties of the natural logarithm include ln.e x / D x

and

e ln.x/ D x

(13.5)

So, the functions ln.x/ and e x are inverse to one another. Further, for
any two positive real numbers a and b, ln.a  b/ D ln.a/ C ln.b/

(13.6)

e a e b D e aCb

(13.7)

effectively because So, logarithms turn products into sums! Using the
above property, we can deduce the following for all positive real
numbersa and  b and any real number c:  ln

b a

D ln.b/ b

ln.a/

because eea D e b a  ln.ac / D c  ln.a/ because .e a /c D e ac We also
have a logarithm log2 with a base of 2. Similar to the natural
logarithm,

374

CHAPTER 13 Mathematical Tools for Quantum Computing III

log2 .y/ D x () 2x D y

(13.8)

In fact, the natural logarithm could be written ln.x/ D loge .x/, i.e.,
with an explicitly mentioned base of e. There are logarithms for every
positive real number base, so it’s nice to be able to base change. To
change the base of a logarithm from one base b to another base c, we can
use the formula logb .a/ D

logc .a/ logc .b/

(13.9)

One trick to remember this is that the a is above the b on the left-hand
side, and that after changing the base to c, the a remains above the b
on the right-hand side.

13.3

Euler’s Formula

We will give an inkling of a proof via power series (avoiding issues of
convergence for brevity) of the mysterious and wonderful formula of
Euler, relating the polar coordinates of a complex number of unit norm
to the number e, as mentioned in the previous chapter and depicted in
Figure 13.3. 13.10

Euler’s formula e i D cos. / C i sin./

The power series of the (complex-valued) cosine and sine functions are
cos.z/ D 1 and

z2 z4 C 2Š 4Š

z6 C ::: 6Š

(13.11)

z3 z5 z7 C C ::: (13.12) 3Š 5Š 7Š The power series of the
(complex-valued) exponential function e z WD exp .z/ is z2 z3 z4 ez D 1
C z C C C C ::: (13.13) 2Š 3Š 4Š Then, evaluating the power series for
the exponential function at the complex number iz yields sin.z/ D z

SECTION 13.3 Euler’s Formula

375

=2

e i D cos. / C i sin. / 1  

0

3=2

Figure 13.3: Euler’s formula

.iz/2 .iz/3 .iz/4 C C C ::: 2Š 3Š 4Š i 2z2 i 3z3 i 4z4 D 1 C iz C C C C
::: 2Š 3Š 4Š

e iz D 1 C .iz/ C

and remembering that i 2 D 1 C iz C

1; i 3 D

(13.14)

i and i 4 D 1 further yields

i 2z2 i 3z3 i 4z4 C C C ::: 2Š 3Š 4Š 1  z2 iz 3 z4 D 1 C iz C C C C :::
2Š 3Š 4Š z 2 iz 3 z4 D 1 C iz C C ::: (13.15) 2Š 3Š 4Š

and after a little reorganization, we have    z2 z4 D 1 C ::: C iz 2Š
4Š

iz 3 iz 5 C 3Š 5Š

Now, multiplying the power series for sin.z/ by i yields

 :::

(13.16)

376

CHAPTER 13 Mathematical Tools for Quantum Computing III

 i sin.z/ D i z D iz

z3 z5 C 3Š 5Š 3 iz iz 5 C 3Š 5Š

 z7 C : : : D iz 7Š iz 7 C ::: 7Š

i

z3 z5 Ci 3Š 5Š

i

z7 C ::: 7Š (13.17)

Adding the power series of cos.z/ and the newly acquired expression for
i sin.z/ yields     z2 z4 iz 3 iz 5 cos.z/ C i sin.z/ D 1 C ::: C iz
C ::: 2Š 4Š 3Š 5Š (13.18) which is exactly the expression we found for e
iz earlier! Therefore, e iz D cos.z/ C i sin.z/

(13.19)

Using Euler’s formula, we have Euler’s identity: 13.20

Euler’s Identity ei  C 1 D 0

For further resources and additional mathematical tools, please refer to
the book’s GitHub site.

CHAPTER

14 Dirac Notation Paul Dirac developed a notation for vectors as well as
vector and matrix operations that we use extensively in quantum
mechanics and quantum computing \[92\]. Now that we have built up our
mathematical toolkit we can describe the correspondence between
traditional linear algebra notation and Dirac notation.

14.1

Vectors

A vector in linear algebra is typically represented as a column vector
or as the row vector which is the conjugate transpose of the column
vector. In Dirac notation we denote a column vector as a ket and the
conjugate transpose of the column vector as a bra – thus the bra-ket
framework developed by Dirac. So the column vectors we represent as j0i
and j1i are as follows: 

1 0





0 1



j0i WD j1i WD

The symbol used inside the ket or bra is called the label and it is
important to note that the choice of a particular label is arbitrary. We
could have named the above two vectors jbluei and jgoldi as easily as
j0i and j1i. It is also important to note the difference between j0i and
the zero vector of traditional linear algebra notation which is denoted
as 0. That zero vector represents the origin point in a vector space and
has no relationship with the Dirac notation of j0i. The reason for
labeling the first basis vector with the numeral 0 is likely due to the
way that computer scientists like to count: starting from 0 © The
Author(s), under exclusive license to Springer Nature Switzerland AG
2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_14

377

378

CHAPTER 14 Dirac Notation

(then 1; 2, etc.) Using Dirac notation, we can signify that a particular
vector is in a Hilbert space like so jui  H In chapters 11 and 12, we
covered the core operations in linear algebra including inner and outer
products as well as the tensor product. Here will outline how to denote
these operations using Dirac notation.

14.2

Vector operations

We can represent vector operations using Dirac notation. We denote a
vector multiplied by a scalar as follows ˛ j0i where ˛ is a scalar. We
can represent the linear combination or superposition of states with
their normalization coefficients as in this example 1 1 j i D p j0i C p
j1i 2 2

(14.1)

Inner and Outer Products If we wish to take the inner product of two
vectors in Dirac notation, u and v, we can represent this operation as
huj jvi

(14.2)

Or, we can contract this notation as follows hujvi

(14.3)

Note that since in the inner product we take the conjugate transpose of
the first vector, we denote this vector with a bra. The second vector
remains a column vector so it is a ket. We recall that the result of the
inner product is a scalar. So if we take the inner product of j0i and
j1i we obtain 0 since the two vectors are orthogonal to each other, as
shown here h0j1i D 0

(14.4)

SECTION 14.3 Tensor Products

379

We can also represent the outer product (or matrix multiplication) of
two vectors (where we treat them as matrices) as juihvj

(14.5)

Note that in the outer product we keep the first vector in column form
and take conjugate transpose of the second vector. Thus we represent the
first vector as a ket and the second as a bra. The outer product yields
a matrix. So, for example, if we take the outer product of j0i and j1i
we obtain the following matrix  j0ih1j D

0 1 0 0

 (14.6)

We can also string several operations together. For example, the
following notation represents an inner product operation followed by
taking the inner product of u and v and multiplying the result as a
scalar with w. hujvi jwi

(14.7)

Recall that in traditional linear algebra notation, we can represent the
inner product of two vectors u and v like so: hu; vi

(14.8)

Dirac was probably inspired by this traditional notation to develop his
bra-ket system.

14.3

Tensor Products

To represent the state of two or more uncorrelated qubits in a register,
we can use the tensor product. If we have two qubits represented by j0i
and j0i since they were both initialized to that state, we can represent
the register as follows j0i ˝ j0i

(14.9)

Note that we can also represent the tensor of two qubits like so j0ij0i

(14.10)

j00i

(14.11)

and this way as well

380

CHAPTER 14 Dirac Notation

So all these are equivalent representations j0i ˝ j0i D j0ij0i D j00i

(14.12)

The reader might benefit from recognizing that if j0i and j1i are 2
states from one qubit and j0i and j1i are 2 states from another
(uncorrelated) qubit, then the quantum register includes the 4 states
j0i ˝ j0i ; j0i ˝ j1i ; j1i ˝ j0i ; j1i ˝ j1i

(14.13)

which are written more concisely as j00i ; j01i ; j10i ; j11i

(14.14)

00; 01; 10 and 11

(14.15)

and are not coincidentally the numbers 0,1,2 and 3 written in binary
notation. Exercise Check that the 8 states included in the tensor
product of 3 qubits, when written in the concise Dirac notation
described above, correspond exactly to the numbers 0,1,2,3,4,5,6, and 7
when written in binary notation. At that stage, the reader will
hopefully see the utility of this concise notation. 14.16

We can further signify n number of qubits as part of a register in the
following way j0i˝n (14.17) which represents n qubits, each initialized
to state j0i and tensored together.

14.4

Notation for PDF and Expectation Value

Another use of Dirac notation is to represent the probability density
function and expectation value. Recall that the integrated probability
density function (PDF) of a particle can be described as Z h‰j‰i D

C1 1

‰  .x; t / ‰.x; t / dx

(14.18)

SECTION 14.4 Notation for PDF and Expectation Value

381

which, for a normalized wave function ‰, will equal 1. We normalize the
wave function so that the integrated PDF = 1 to meet the Born Rule that
the integrated square of the modulus of the wave function gives us 1
since the particle exists somewhere. Now if we wish to calculate the
expectation value of the position operator, xO , we can do so as follows
Z C1 hOxi D h‰j xO j‰i D ‰  .x; t / xO ‰.x; t / dx (14.19) 1

This gives us the average position of the particle at time t . We call
this mean the expectation value for the xO operator. Dirac notation is
used extensively throughout quantum mechanics and quantum computing and
it is worth spending some time to get familiar with the use cases in
this chapter. Check the companion online site for exercises with Dirac
notation.

CHAPTER

15 Table of Quantum Operators and Core Circuits   0 1 1 0  0 i

i 0

 1 0

 0 1

p1 2



cos 2 i sin 2

1 1

X



1 1

Y

Z

Z

H

H

Rx . /

Rx . /

Ry . /

Ry ./

R'

R'



i sin 2 cos 2

cos 2 sin 2

sin 2 cos 2





1 0 0 e i'

Y

!

!

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2\_15

383

384

CHAPTER 15 Table of Quantum Operators and Core Circuits

  1 0 0 i

S

S

  1 0 0 e i =4

T

T

N/A

Meas.

0 1 B0 B @0 0

0 1 B0 B @0 0

0 1 B0 B0 B B0 B0 B B0 @ 0 0

0 1 0 0 0 0 0 0

0 1 0 0

0 1 0 0

0 0 0 1

0 0 1 0

1 0 0C C 1A 0

CNOT



1 0 0C C 0A 1

CZ



SWAP

 

Toffoli

 

0 1 B0 B @0 0

0 0 1 0

0 1 0 0

1 0 0C C 0A 1

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 1 0 0 0

0 0 0 0 0 1 0 0

0 0 0 0 0 0 0 1

Z

1 0 0C 0C C 0C 0C C 0C A 1 0

CHAPTER 15 Table of Quantum Operators and Core Circuits

0 1 B0 B0 B B0 B0 B B0 @ 0 0

0 1 0 0 0 0 0 0

0 0 1 0 0 0 0 0

0 0 0 1 0 0 0 0

0 1 0 B p1 @ 2 0 1

0 1 1 0

0 0 0 0 1 0 0 0 1 0 0 1

0 0 0 0 0 0 1 0

0 0 0 0 0 1 0 0

1 0 0C 0C C 0C 0C C 0C A 0 1

1 0 1C 1A 0

HXH D Z HZH D X HYH D Y H D H D H 1 X 2 D Y 2 D Z2 p DI H D .X C Z/= 2
H2 D I SWAP12 D C12 C21 C12 C12 X1 C12 D X1 X2 C12 Y1 C12 D Y1 X2 C12 Z1
C12 D Z1 C12 X2 C12 D X2 C12 Y2 C12 D Z1 Y2 C12 Z2 C12 D Z1 Z2 Rz;1 .
/C12 D C12 Rz;1 ./ Rx;2 . /C12 D C12 Rx;2 ./



Fredkin

 

Bell

Gate Identities (C D CNOT)

H



385

Works Cited

\[1\] S. Aaronson. Certified randomness from quantum supremacy. Multiple
unpublished talks. \[2\] S. Aaronson. The Limits of Quantum Computers.
Scientific American, March 2008. \[3\] S. Aaronson. Quantum Complexity
Theory. Fall 2010. Massachusetts Institute of Technology: MIT
OpenCouseWare. https://ocw.mit.edu. License: Creative Commons BY-NC-SA,
2010. \[4\] S. Aaronson. Read the fine print. Nature Physics, 11(4):291,
2015. \[5\] S. Aaronson and A. Arkhipov. The computational complexity of
linear optics. In Proceedings of the forty-third annual ACM symposium on
Theory of computing, pages 333–342. ACM, 2011. \[6\] S. Aaronson, G.
Kuperberg, C. Granade, and V. Russo. The Complexity Zoo.
https://complexityzoo.net/, 2005. \[7\] A. Abbas, D. Sutter, C. Zoufal,
A. Lucchi, A. Figalli, and S. Woerner. The power of quantum neural
networks. Nature Computational Science, 1(6):403–409, Jun 2021. arXiv:
2011.00027. \[8\] C. Adami and N. J. Cerf. Quantum computation with
linear optics. In Quantum Computing and Quantum Communications, pages
391–401. Springer, 1999.

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2

387

388

Works Cited

\[9\] M. Agrawal, N. Kayal, and N. Saxena. PRIMES is in P. Annals of
Mathematics, 160:781–793, 2004. \[10\] D. Aharonov, A. Ambainis, J.
Kempe, and U. Vazirani. Quantum walks on graphs. In Proceedings of the
thirty-third annual ACM symposium on Theory of computing, pages 50–59.
ACM, 2001. \[11\] D. Aharonov and U. Vazirani. Is quantum mechanics
falsifiable? A computational perspective on the foundations of quantum
mechanics. Computability: Turing, Gödel, Church, and Beyond. MIT Press,
2013. \[12\] Y. Aharonov, L. Davidovich, and N. Zagury. Quantum random
walks. Physical Review A, 48(2):1687– 1690, Aug 1993. \[13\] Y. Alexeev,
D. Bacon, K. R. Brown, R. Calderbank, L. D. Carr, F. T. Chong, B.
DeMarco, D. Englund, E. Farhi, B. Fefferman, and et al. Quantum computer
systems for scientific discovery. PRX Quantum, 2(1):017001, Feb 2021.
\[14\] S. Allen, J. Kim, D. L. Moehring, and C. R. Monroe.
Reconfigurable and programmable ion trap quantum computer. In 2017 IEEE
International Conference on Rebooting Computing (ICRC), pages 1–3, Nov
2017. \[15\] A. Almheiri, X. Dong, and D. Harlow. Bulk locality and
quantum error correction in ads/cft. Journal of High Energy Physics,
2015(4):163, 2015. \[16\] C. Arnold, J. Demory, V. Loo, A. Lemaître, I.
Sagnes, M. Glazov, O. Krebs, P. Voisin, P. Senellart, and L. Lanco.
Macroscopic rotation of photon polarization induced by a single spin.
Nature Communications, 6:6236, 2015. \[17\] J. M. Arrazola, V. Bergholm,
K. Brádler, T. R. Bromley, M. J. Collins, I. Dhand, A. Fumagalli, T.
Gerrits, A. Goussev, L. G. Helt, and et al. Quantum circuits

Works Cited

with many photons on a programmable nanophotonic chip. Nature,
591(78487848):54–60, Mar 2021. \[18\] M. Artin. Algebra. Pearson, 2010.
\[19\] F. Arute, K. Arya, R. Babbush, D. Bacon, J. C. Bardin, R.
Barends, R. Biswas, S. Boixo, F. G. S. L. Brandao, D. A. Buell, and et
al. Quantum supremacy using a programmable superconducting processor.
Nature, 574(7779):505–510, Oct 2019. \[20\] S. Axler. Linear Algebra
Done Right. Springer, 2014. \[21\] R. Babbush, D. W. Berry, and H.
Neven. Quantum simulation of the Sachdev-Ye-Kitaev model by asymmetric
qubitization. Physical Review A, 99(4):040301, 2019. \[22\] D. M. Bacon.
Decoherence, Control, and Symmetry in Quantum Computers. PhD thesis,
University of California at Berkeley, 2001. \[23\] S. Bae. JavaScript
Data Structures and Algorithms: An Introduction to Understanding and
Implementing Core Data Structure and Algorithm Fundamentals. Apress,
2019. \[24\] P. Baireuther, T. E. O’Brien, B. Tarasinski, and C. W.
Beenakker. Machine-learning-assisted correction of correlated qubit
errors in a topological code. Quantum, 2:48, 2018. \[25\] P. Ball.
Ion-based commercial quantum computer is a first. Physics World,
December 17, 2018 (https://bit.ly/2RrpZDf), 2018. Original URL:
https://physicsworld.com/a/ion-basedcommercial-quantum-computer-is-a-first/.
\[26\] A. Barenco, C. H. Bennett, R. Cleve, D. P. DiVincenzo, N.
Margolus, P. Shor, T. Sleator, J. A. Smolin, and H. Weinfurter.
Elementary gates for quantum computation. Physical review A, 52(5):3457,
1995. arXiv: quant-ph/9503016.

389

390

Works Cited

\[27\] A. Barna and D. I. Porat. Integrated Circuits in Digital
Electronics. Wiley-Interscience, 1987. \[28\] D. Barredo, V. Lienhard,
S. de Léséleuc, T. Lahaye, and A. Browaeys. Synthetic three-dimensional
atomic structures assembled atom by atom. Nature, 561(7721):79–82, Sep
2018. arXiv: 1712.02727. \[29\] S. Bartolucci, P. Birchall, H. Bombin,
H. Cable, C. Dawson, M. Gimeno-Segovia, E. Johnston, K. Kieling, N.
Nickerson, M. Pant, and et al. Fusionbased quantum computation.
arXiv:2101.09310 \[quant-ph\], Jan 2021. arXiv: 2101.09310. \[30\] P.
Benioff. The computer as a physical system: A microscopic quantum
mechanical hamiltonian model of computers as represented by turing
machines. Journal of Statistical Physics, 22(5):563–591, May 1980.
\[31\] C. H. Bennett, E. Bernstein, G. Brassard, and U. Vazirani.
Strengths and weaknesses of quantum computing. SIAM journal on
Computing, 26(5):1510–1523, 1997. \[32\] C. H. Bennett and G. Brassard.
Quantum cryptography: Public key distribution and coin tossing. In Proc.
IEEE Int. Conf. Computers, Systems, and Signal Processing, volume 175,
1984. \[33\] C. H. Bennett, G. Brassard, C. Crépeau, R. Jozsa, A. Peres,
and W. K. Wootters. Teleporting an unknown quantum state via dual
classical and EinsteinPodolsky-Rosen channels. Phys. Rev. Lett.,
70:1895– 1899, Mar 1993. \[34\] C. H. Bennett and S. J. Wiesner.
Communication via one- and two-particle operators on
EinsteinPodolsky-Rosen states. Phys. Rev. Lett., 69:2881– 2884, Nov
1992. \[35\] H. Bernien, B. Hensen, W. Pfaff, G. Koolstra, M. Blok, L.
Robledo, T. Taminiau, M. Markham, D. Twitchen, L. Childress, et al.
Heralded entangle-

Works Cited

ment between solid-state qubits separated by three metres. Nature,
497(7447):86, 2013. \[36\] E. Bernstein and U. Vazirani. Proceedings of
the 25th annual ACM symposium on the theory of computing. ACM, New York,
11, 1993. \[37\] D. W. Berry, A. M. Childs, R. Cleve, R. Kothari, and R.
D. Somma. Simulating hamiltonian dynamics with a truncated taylor
series. Physical review letters, 114(9):090502, 2015. \[38\] M. K.
Bhaskar, D. D. Sukachev, A. Sipahigil, R. E. Evans, M. J. Burek, C. T.
Nguyen, L. J. Rogers, P. Siyushev, M. H. Metsch, H. Park, et al. Quantum
nonlinear optics with a germanium-vacancy color center in a nanoscale
diamond waveguide. Physical Review Letters, 118(22):223603, 2017. \[39\]
J. Biamonte, P. Wittek, N. Pancotti, P. Rebentrost, N. Wiebe, and S.
Lloyd. Quantum machine learning. Nature, 549(7671):195, 2017. \[40\] A.
Blanco-Redondo, I. Andonegui, M. J. Collins, G. Harari, Y. Lumer, M. C.
Rechtsman, B. J. Eggleton, and M. Segev. Topological optical waveguiding
in silicon and the transition between topological and trivial defect
states. Physical Review Letters, 116(16):163901, 2016. \[41\] A.
Blanco-Redondo, B. Bell, M. Segev, and B. Eggleton. Photonic quantum
walks with symmetry protected topological phases. In AIP Conference
Proceedings, volume 1874, page 020001. AIP Publishing, 2017. \[42\] M.
Blok, V. Ramasesh, J. Colless, K. O’Brien, T. Schuster, N. Yao, and I.
Siddiqi. Implementation and applications of two qutrit gates in
superconducting transmon qubits. Presented at APS March Meeting, 2018.
\[43\] M. S. Blok, V. V. Ramasesh, T. Schuster, K. O’Brien, J. M.
Kreikebaum, D. Dahlen, A. Morvan,

391

392

Works Cited

B. Yoshida, N. Y. Yao, and I. Siddiqi. Quantum information scrambling in
a superconducting qutrit processor. Physical Review X, 11(2):021010, Apr
2021. arXiv: 2003.03307. \[44\] J. G. Bohnet, B. C. Sawyer, J. W.
Britton, M. L. Wall, A. M. Rey, M. Foss-Feig, and J. J. Bollinger.
Quantum spin dynamics and entanglement generation with hundreds of
trapped ions. Science, 352(6291):1297–1301, 2016. \[45\] S. Boixo, S. V.
Isakov, V. N. Smelyanskiy, R. Babbush, N. Ding, Z. Jiang, M. J. Bremner,
J. M. Martinis, and H. Neven. Characterizing quantum supremacy in
near-term devices. Nature Physics, 14(6):595–600, Jun 2018. arXiv:
1608.00263. \[46\] A. D. Bookatz. QMA-complete problems. Quantum
Information & Computation, 14(5&6):361–383, 2014. \[47\] M. Born. Zur
Quantenmechanik der Stoßvorgänge. Z. Phys., 37(12):863–867, 1926. \[48\]
M. Born. Das adiabatenprinzip in der quantenmechanik. Zeitschrift für
Physik A Hadrons and Nuclei, 40(3):167–192, 1927. \[49\] M. Born and V.
Fock. Beweis des adiabatensatzes (1928, English Translation). In L.
Faddeev, L. Khalfin, and I. Komarov, editors, V.A. Fock – Selected
Works: Quantum Mechanics and Quantum Field Theory. Chapman & Hall/CRC,
2004. \[50\] D. Boschi, S. Branca, F. De Martini, L. Hardy, and S.
Popescu. Experimental realization of teleporting an unknown pure quantum
state via dual classical and Einstein-Podolsky-Rosen channels. Phys.
Rev. Lett., 80:1121–1125, Feb 1998. \[51\] V. Bouchiat, D. Vion, P.
Joyez, D. Esteve, and M. Devoret. Quantum coherence with a single cooper
pair. Physica Scripta, 1998(T76):165, 1998.

Works Cited

\[52\] A. Bouland, B. Fefferman, C. Nirkhe, and U. Vazirani. Quantum
supremacy and the complexity of random circuit sampling. arXiv preprint
arXiv:1803.04402, 2018. \[53\] P. O. Boykin, T. Mor, M. Pulver, V.
Roychowdhury, and F. Vatan. On universal and fault-tolerant quantum
computing. arXiv preprint quant-ph/9906054, 1999. \[54\] T.-D. Bradley.
https://www.math3ma.com, 2015.

Math3ma.

\[55\] T.-D. Bradley. What is Applied Category Theory? arXiv preprint
arXiv:1809.05923, 2018. \[56\] G. Brassard and P. Hoyer. An exact
quantum polynomial-time algorithm for Simon’s problem. In Proceedings of
the Fifth Israeli Symposium on Theory of Computing and Systems, pages
12–23. IEEE, 1997. \[57\] G. Brassard, P. Hoyer, M. Mosca, and A. Tapp.
Quantum amplitude amplification and estimation. Contemporary
Mathematics, 305:53–74, 2002. \[58\] S. Bravyi, D. Gosset, and R.
Koenig. Quantum advantage with shallow circuits. Science,
362(6412):308–311, 2018. \[59\] S. Bravyi, D. Gosset, R. Koenig, and M.
Tomamichel. Quantum advantage with noisy shallow circuits in 3d. arXiv
preprint arXiv:1904.01502, 2019. \[60\] S. B. Bravyi and A. Y. Kitaev.
Quantum codes on a lattice with boundary. arXiv preprint
quantph/9811052, 1998. \[61\] K. R. Brown, A. W. Harrow, and I. L.
Chuang. Arbitrarily accurate composite pulse sequences. Physical Review
A, 70(5):052318, 2004. \[62\] D. Browne. Universal fault tolerant
quantum computing with 3D surface codes.

393

394

Works Cited

https://www.youtube.com/watch?v=jHbcdhSH89c, 2020. \[63\] C. D.
Bruzewicz, J. Chiaverini, R. McConnell, and J. M. Sage. Trapped-ion
quantum computing: Progress and challenges. arXiv preprint
arXiv:1904.04178, 2019. \[64\] Y. Cao, G. G. Guerreschi, and A.
Aspuru-Guzik. Quantum neuron: an elementary building block for machine
learning on quantum computers. arXiv preprint arXiv:1711.11240, 2017.
\[65\] J. Carolan, C. Harrold, C. Sparrow, E. Martín-López, N. J.
Russell, J. W. Silverstone, P. J. Shadbolt, N. Matsuda, M. Oguma, M.
Itoh, et al. Universal linear optics. Science, 349(6249):711–716, 2015.
\[66\] S. Castelletto, B. Johnson, V. Ivády, N. Stavrias, T. Umeda, A.
Gali, and T. Ohshima. A silicon carbide room-temperature single-photon
source. Nature Materials, 13(2):151, 2014. \[67\] M. Cerezo, A.
Arrasmith, R. Babbush, S. C. Benjamin, S. Endo, K. Fujii, J. R. McClean,
K. Mitarai, X. Yuan, L. Cincio, et al. Variational quantum algorithms.
arXiv preprint arXiv:2012.09265, 2020. \[68\] K. C. Chen, W. Dai, C.
Errando-Herranz, S. Lloyd, and D. Englund. Scalable and high-fidelity
quantum random access memory in spin-photon networks. arXiv:2103.07623
\[quant-ph\], Mar 2021. arXiv: 2103.07623. \[69\] W.-J. Chen, M. Xiao,
and C. T. Chan. Photonic crystals possessing multiple Weyl points and
the experimental observation of robust surface states. Nature
Communications, 7:13038, 2016. \[70\] X.-Y. Chen and Z.-q. Yin.
Universal quantum gates between nitrogen-vacancy centers in a levitated
nanodiamond. Physical Review A, 99(2):022319, Feb 2019. arXiv:
1810.00285.

Works Cited

\[71\] N.-H. Chia, A. Gilyén, T. Li, H.-H. Lin, E. Tang, and C. Wang.
Quantum-inspired sublinear algorithm for solving low-rank semidefinite
programming. arXiv:1910.06151 \[cs\], Aug 2020. arXiv: 1910.06151.
\[72\] N.-H. Chia, T. Li, H.-H. Lin, and C. Wang. Quantuminspired
sublinear algorithm for solving low-rank semidefinite programming.
arXiv:1901.03254 \[quant-ph\], Aug 2020. arXiv: 1901.03254. \[73\] L.
Childress and R. Hanson. Diamond nv centers for quantum computing and
quantum networks. MRS Bulletin, 38(2):134–138, 2013. \[74\] A. M.
Childs. Universal computation by quantum walk. Physical review letters,
102(18):180501, 2009. \[75\] A. M. Childs, R. Cleve, E. Deotto, E.
Farhi, S. Gutmann, and D. A. Spielman. Exponential algorithmic speedup
by a quantum walk. In Proceedings of the thirty-fifth annual ACM
symposium on Theory of computing, pages 59–68. ACM, 2003. \[76\] A. M.
Childs, E. Farhi, and S. Gutmann. An example of the difference between
quantum and classical random walks. arXiv preprint arXiv:
quantph/0103020v1, Mar 2001. \[77\] K. S. Chou, J. Z. Blumoff, C. S.
Wang, P. C. Reinhold, C. J. Axline, Y. Y. Gao, L. Frunzio, M. Devoret,
L. Jiang, and R. Schoelkopf. Deterministic teleportation of a quantum
gate between two logical qubits. Nature, 561(7723):368, 2018. \[78\] I.
Chuang. Recorded talk: Grand unification of quantum algorithms.
https://www.youtube.com/watch?v=GFRojXdrVXI. \[79\] J. I. Cirac and P.
Zoller. Quantum computations with cold trapped ions. Phys. Rev. Lett.,
74:4091–4094, May 1995.

395

396

Works Cited

Cirq \[80\] Cirq Developers. https://quantumai.google/cirq.

documentation.

\[81\] Cirq Developers. Cirq tutorials website.
https://quantumai.google/cirq/tutorials. \[82\] B. D. Clader, B. C.
Jacobs, and C. R. Sprouse. Preconditioned quantum linear system
algorithm. Physical Review Letters, 110(25):250504, Jun 2013. arXiv:
1301.2340. \[83\] R. Cleve, A. Ekert, C. Macchiavello, and M. Mosca.
Quantum algorithms revisited. Proceedings of the Royal Society of
London. Series A: Mathematical, Physical and Engineering Sciences,
454(1969):339– 354, 1998. \[84\] P. J. Coles, S. Eidenbenz, S. Pakin, A.
Adedoyin, J. Ambrosiano, P. Anisimov, W. Casper, G. Chennupati, C.
Coffrin, H. Djidjev, et al. Quantum algorithm implementations for
beginners. arXiv preprint arXiv:1804.03719, 2020. \[85\] C. M. Dawson
and M. A. Nielsen. The SolovayKitaev algorithm. arXiv preprint
quant-ph/0505030, 2005. \[86\] E. Dennis, A. Kitaev, A. Landahl, and J.
Preskill. Topological quantum memory. Journal of Mathematical Physics,
43(9):4452–4505, 2002. \[87\] D. Dervovic, M. Herbster, P. Mountney, S.
Severini, N. Usher, and L. Wossnig. Quantum linear systems algorithms: a
primer. arXiv preprint arXiv:1802.08227, 2018. \[88\] D. Deutsch.
Quantum theory, the Church–Turing principle and the universal quantum
computer. Proceedings of the Royal Society of London A: Mathematical,
Physical and Engineering Sciences, 400(1818):97–117, 1985.

Works Cited

\[89\] D. Deutsch. Lectures on Quantum Computation.
http://www.quiprocone.org/Protected/ DD\_lectures.htm, 2003. \[90\] D.
Deutsch and R. Jozsa. Rapid solution of problems by quantum computation.
Proceedings of the Royal Society of London A: Mathematical, Physical and
Engineering Sciences, 439(1907):553–558, 1992. \[91\] C. Ding, T.-Y.
Bao, and H.-L. Huang. Quantuminspired support vector machine.
arXiv:1906.08902 \[quant-ph, stat\], Mar 2021. arXiv: 1906.08902. \[92\]
P. A. M. Dirac. A new notation for quantum mechanics. Mathematical
Proceedings of the Cambridge Philosophical Society, 35(3):416–418, 1939.
\[93\] D. P. DiVincenzo. Topics in quantum computers. arXiv preprint
cond-mat/9612126, 1996. \[94\] D. P. DiVincenzo. The physical
implementation of quantum computation. Fortschritte der Physik: Progress
of Physics, 48(9-11):771–783, 2000. arXiv: quant-ph/0002077. \[95\] M.
W. Doherty, N. B. Manson, P. Delaney, F. Jelezko, J. Wrachtrup, and L.
C. Hollenberg. The nitrogenvacancy colour centre in diamond. Physics
Reports, 528(1):1–45, 2013. \[96\] L.-M. Duan and H. Kimble. Scalable
photonic quantum computation through cavity-assisted interactions.
Physical Review Letters, 92(12):127902, 2004. \[97\] D. S. Dummit and R.
M. Foote. Abstract Algebra, volume 3. Wiley Hoboken, 2004. \[98\] S.
Ebadi, T. T. Wang, H. Levine, A. Keesling, G. Semeghini, A. Omran, D.
Bluvstein, R. Samajdar, H. Pichler, W. W. Ho, and et al. Quantum phases
of matter on a 256-atom programmable quantum simulator. Nature,
595(7866):227–232, Jul 2021. arXiv: 2012.12281.

397

398

Works Cited

\[99\] A. Einstein. Letter from Einstein to D. M. Lipkin.
https://bit.ly/2CogEUC, July 1952. Accessed: 201805-19, Original URL:
http://sethlipkin.com/
collectibles/letters/letter1/letter%201%20%20page%201.jpg. \[100\] A.
Einstein, B. Podolsky, and N. Rosen. Can quantum-mechanical description
of physical reality be considered complete? Phys. Rev., 47:777–780, May
1935. \[101\] R. E. Evans, M. K. Bhaskar, D. D. Sukachev, C. T. Nguyen,
A. Sipahigil, M. J. Burek, B. Machielse, G. H. Zhang, A. S. Zibrov, E.
Bielejec, et al. Photonmediated interactions between quantum emitters in
a diamond nanocavity. Science, 362(6415):662–665, 2018. \[102\] K. Fang
and Z.-W. Liu. No-go theorems for quantum resource purification.
Physical Review Letters, 125(6):060405, Aug 2020. \[103\] E. Farhi, J.
Goldstone, and S. Gutmann. A quantum algorithm for the hamiltonian NAND
tree. arXiv preprint quant-ph/0702144, 2007. \[104\] E. Farhi, J.
Goldstone, and S. Gutmann. A quantum approximate optimization algorithm.
arXiv preprint arXiv:1411.4028, 2014. \[105\] E. Farhi, J. Goldstone,
and S. Gutmann. A quantum approximate optimization algorithm applied to
a bounded occurrence constraint problem. arXiv preprint arXiv:1412.6062,
2014. \[106\] E. Farhi, J. Goldstone, S. Gutmann, and M. Sipser. Quantum
computation by adiabatic evolution. arXiv preprint quant-ph/0001106,
2000. \[107\] E. Farhi and S. Gutmann. Analog analogue of a digital
quantum computation. Physical Review A, 57(4):2403, 1998.

Works Cited

\[108\] E. Farhi and S. Gutmann. Quantum computation and decision trees.
Physical Review A, 58(2):915–928, Aug 1998. arXiv: quant-ph/9706062.
\[109\] E. Farhi and H. Neven. Classification with quantum neural
networks on near term processors. arXiv preprint arXiv:1802.06002, 2018.
\[110\] R. Ferguson, L. Dellantonio, A. Al Balushi, K. Jansen, W. Dür,
and C. Muschik. Measurementbased variational quantum eigensolver.
Physical Review Letters, 126(22):220501, 2021. \[111\] R. P. Feynman.
Simulating physics with computers. International Journal of Theoretical
Physics, 21(6):467–488, Jun 1982. \[112\] R. P. Feynman. Feynman
Lectures on Computation. CRC Press, 2000. \[113\] C. Figgatt, D. Maslov,
K. A. Landsman, N. M. Linke, S. Debnath, and C. Monroe. Complete 3-qubit
grover search on a programmable quantum computer. Nature Communications,
8(11):1918, Dec 2017. \[114\] M. Fingerhuth, T. Babej, and P. Wittek.
Open source software in quantum computing. PLOS One, 13(12):e0208561,
2018. \[115\] C. Flühmann, T. L. Nguyen, M. Marinelli, V. Negnevitsky,
K. Mehta, and J. Home. Encoding a qubit in a trapped-ion mechanical
oscillator. Nature, 566(7745):513, 2019. \[116\] A. G. Fowler, M.
Mariantoni, J. M. Martinis, and A. N. Cleland. Surface codes: Towards
practical large-scale quantum computation. Phys. Rev. A, 86:032324, Sep
2012. \[117\] J. B. Fraleigh. A First Course in Abstract Algebra.
Pearson, 2002. \[118\] E. Fredkin and T. Toffoli. Conservative logic.
International Journal of Theoretical Physics, 21(3):219– 253, Apr 1982.

399

400

Works Cited

\[119\] M. Freedman, A. Kitaev, M. Larsen, and Z. Wang. Topological
quantum computation. Bulletin of the American Mathematical Society,
40(1):31–38, 2003. arXiv: quant-ph/0101025. \[120\] E. S. Fried, N. P.
Sawaya, Y. Cao, I. D. Kivlichan, J. Romero, and A. Aspuru-Guzik. qTorch:
The quantum tensor contraction handler. PloS one, 13(12):e0208510, 2018.
\[121\] N. Friis, O. Marty, C. Maier, C. Hempel, M. Holzäpfel, P.
Jurcevic, M. B. Plenio, M. Huber, C. Roos, R. Blatt, et al. Observation
of entangled states of a fully controlled 20-qubit system. Physical
Review X, 8(2):021012, 2018. \[122\] A. Frisk Kockum. Quantum optics
with artificial atoms. Chalmers University of Technology, 2014. arXiv:
1912.13012. \[123\] J. M. Gambetta, J. M. Chow, and M. Steffen. Building
logical qubits in a superconducting quantum computing system. NPJ
Quantum Information, 3(1):2, 2017. arXiv: 1510.04375. \[124\] M. Ganahl,
A. Milsted, S. Leichenauer, J. Hidary, and G. Vidal. TensorNetwork on
TensorFlow: Entanglement renormalization for quantum critical lattice
models. arXiv preprint arXiv:1906.12030, 2019. \[125\] A. Gilyén, Y. Su,
G. H. Low, and N. Wiebe. Quantum singular value transformation and
beyond: exponential improvements for quantum matrix arithmetics. In
Proceedings of the 51st Annual ACM SIGACT Symposium on Theory of
Computing, pages 193–204, 2019. \[126\] V. Giovannetti, S. Lloyd, and L.
Maccone. Quantum random access memory. arXiv preprint arXiv:0708.1879v2,
Aug 2007. \[127\] Google AI Quantum and others. Hartree-Fock on a
superconducting qubit quantum computer. Science, 369(6507):1084–1089,
2020.

Works Cited

\[128\] D. Gottesman. The Heisenberg representation of quantum
computers. arXiv preprint quantph/9807006, 1998. \[129\] Grove
Developers. Grove documentation, 2018.
https://grovedocs.readthedocs.io/en/latest/vqe.html. \[130\] L. K.
Grover. Quantum mechanics helps in searching for a needle in a haystack.
Phys. Rev. Lett., 79:325– 328, Jul 1997. arXiv: quant-ph/9706033.
\[131\] M. Hafezi, E. A. Demler, M. D. Lukin, and J. M. Taylor. Robust
optical delay lines with topological protection. Nature Physics,
7(11):907, 2011. \[132\] M. Hafezi, S. Mittal, J. Fan, A. Migdall, and
J. Taylor. Imaging topological edge states in silicon photonics. Nature
Photonics, 7(12):1001, 2013. \[133\] D. Hanneke, J. P. Home, J. D. Jost,
J. M. Amini, D. Leibfried, and D. J. Wineland. Realization of a
programmable two-qubit quantum processor. Nature Physics, 6(1):13, 2010.
\[134\] G. H. Hardy and J. E. Littlewood. Some problems of diophantine
approximation: Part II. The trigonometrical series associated with the
elliptic theta-functions. Acta Mathematica, 37:193–239, 1914. \[135\] A.
W. Harrow, A. Hassidim, and S. Lloyd. Quantum algorithm for linear
systems of equations. Physical Review Letters, 103(15):150502, 2009.
arXiv: 0811.3171. \[136\] A. W. Harrow and A. Montanaro. Quantum
computational supremacy. Nature, 549(7671):203, 2017. \[137\] M. Z.
Hasan and C. L. Kane. Colloquium: topological insulators. Reviews of
Modern Physics, 82(4):3045, 2010. \[138\] V. Havlíček, A. D. Córcoles,
K. Temme, A. W. Harrow, A. Kandala, J. M. Chow, and J. M. Gambetta.

401

402

Works Cited

Supervised learning with quantum-enhanced feature spaces. Nature,
567(7747):209, 2019. \[139\] M. Hayashi and H. Zhu. Secure uniform
randomnumber extraction via incoherent strategies. Physical Review A,
97(1):012302, 2018. arXiv: 1706.04009. \[140\] P. Hayden, S. Nezami,
X.-L. Qi, N. Thomas, M. Walter, and Z. Yang. Holographic duality from
random tensor networks. Journal of High Energy Physics, 2016(11):9,
2016. \[141\] L. Henriet, L. Beguin, A. Signoles, T. Lahaye, A.
Browaeys, G.-O. Reymond, and C. Jurczak. Quantum computing with neutral
atoms. Quantum, 4:327, Sep 2020. arXiv: 2006.12326. \[142\] B. Hensen,
H. Bernien, A. E. Dréau, A. Reiserer, N. Kalb, M. S. Blok, J.
Ruitenberg, R. F. Vermeulen, R. N. Schouten, C. Abellán, et al.
Loophole-free Bell inequality violation using electron spins separated
by 1.3 kilometres. Nature, 526(7575):682, 2015. \[143\] C. Hepp, T.
Müller, V. Waselowski, J. N. Becker, B. Pingault, H. Sternschulte, D.
Steinmüller-Nethl, A. Gali, J. R. Maze, M. Atatüre, et al. Electronic
structure of the silicon vacancy color center in diamond. Physical
Review Letters, 112(3):036405, 2014. \[144\] O. Higgott, D. Wang, and S.
Brierley. Variational quantum computation of excited states. arXiv
preprint arXiv:1805.08138, 2018. \[145\] C.-K. Hong, Z.-Y. Ou, and L.
Mandel. Measurement of subpicosecond time intervals between two photons
by interference. Physical Review Letters, 59(18):2044, 1987. \[146\] W.
J. Huggins, J. R. McClean, N. C. Rubin, Z. Jiang, N. Wiebe, K. B.
Whaley, and R. Babbush. Efficient and noise resilient measurements for
quantum chemistry on near-term quantum computers. npj Quantum
Information, 7(1):1–9, 2021. arXiv: 1907.13117.

Works Cited

Quantum Algorithm \[147\] S. Jordan. http://quantumalgorithmzoo.org/,
2011.

Zoo.

\[148\] M. Katanaev. Adiabatic theorem for finite dimensional quantum
mechanical systems. Russian Physics Journal, 54(3):342–353, 2011.
\[149\] J. Kempe. Quantum random walks hit exponentially faster. arXiv
preprint quant-ph/0205083, 2002. \[150\] J. Kempe. Quantum random walks:
an introductory overview. Contemporary Physics, 44(4):307–327, 2003.
arXiv: quant-ph/0303081. \[151\] I. Kerenidis and A. Prakash. Quantum
recommendation systems. arXiv preprint arXiv:1603.08675, 2016. \[152\]
A. Y. Kitaev. Quantum measurements and the abelian stabilizer problem.
Nov 1995. \[153\] A. Y. Kitaev. Fault-tolerant quantum computation by
anyons. Annals of Physics, 303(1):2–30, 2003. arXiv: quant-ph/9707021.
\[154\] M. Kjaergaard, M. E. Schwartz, J. Braumüller, P. Krantz, J.
I.-J. Wang, S. Gustavsson, and W. D. Oliver. Superconducting qubits:
Current state of play. Annual Review of Condensed Matter Physics,
11:369–395, 2020. \[155\] E. Knill, R. Laflamme, and G. J. Milburn. A
scheme for efficient quantum computation with linear optics. Nature,
409(6816):46, 2001. \[156\] D. E. Knuth. Big omicron and big omega and
big theta. ACM Sigact News, 8(2):18–24, 1976. \[157\] W. F. Koehl, B. B.
Buckley, F. J. Heremans, G. Calusine, and D. D. Awschalom. Room
temperature coherent control of defect spin qubits in silicon carbide.
Nature, 479(7371):84, 2011. \[158\] P. Kok, W. J. Munro, K. Nemoto, T.
C. Ralph, J. P. Dowling, and G. J. Milburn. Linear optical quantum

403

404

Works Cited

computing with photonic qubits. Reviews of Modern Physics, 79(1):135,
2007. \[159\] P. Krantz, M. Kjaergaard, F. Yan, T. P. Orlando, S.
Gustavsson, and W. D. Oliver. A quantum engineer’s guide to
superconducting qubits. arXiv preprint arXiv:1904.06560, 2019. \[160\]
Y. E. Kraus, Y. Lahini, Z. Ringel, M. Verbin, and O. Zilberberg.
Topological states and adiabatic pumping in quasicrystals. Physical
Review Letters, 109(10):106402, 2012. \[161\] T. D. Ladd, F. Jelezko, R.
Laflamme, Y. Nakamura, C. Monroe, and J. L. O’Brien. Quantum computers.
Nature, 464(7285):45, 2010. \[162\] V. Lahtinen and J. K. Pachos. A
short introduction to topological quantum computation. SciPost Physics,
3(3):021, Sep 2017. arXiv: 1705.04103. \[163\] R. Landauer.
Irreversibility and heat generation in the computing process. IBM
Journal of Research and Development, 5(3):183–191, July 1961. \[164\] F.
Lardinois. IBM publishes its quantum roadmap, says it will have a
1,000-qubit machine in 2023. TechCrunch, 2020. \[165\] R. LaRose.
Overview and comparison of gate level quantum software platforms.
Quantum, 3:130, 2019. \[166\] F. W. Lawvere and S. H. Schanuel.
Conceptual Mathematics: A First Introduction to Categories. Cambridge
University Press, 2009. \[167\] J. Ledin. Modern Computer Architecture
and Organization. Packt Publishing, 2020. \[168\] D. R. Leibrandt, J.
Labaziewicz, V. Vuletić, and I. L. Chuang. Cavity sideband cooling of a
single trapped ion. Physical Review Letters, 103(10):103001, 2009.
\[169\] H. Levine, A. Keesling, A. Omran, H. Bernien, S. Schwartz, A. S.
Zibrov, M. Endres, M. Greiner,

Works Cited

V. Vuletić, and M. D. Lukin. High-fidelity control and entanglement of
rydberg-atom qubits. Physical Review Letters, 121(12):123603, 2018.
\[170\] M. H. Levitt and R. Ernst. Improvement of pulse performance in
nmr coherence transfer experiments: A compensated inadequate experiment.
Molecular Physics, 50(5):1109–1124, 1983. \[171\] F. Li, X. Huang, J.
Lu, J. Ma, and Z. Liu. Weyl points and Fermi arcs in a chiral phononic
crystal. Nature Physics, 14(1):30, 2018. \[172\] C. Liu, M. G. Dutt, and
D. Pekker. Single-photon heralded two-qubit unitary gates for pairs of
nitrogenvacancy centers in diamond. Physical Review A, 98(5):052342,
2018. \[173\] S. Lloyd. A potentially realizable quantum computer.
Science, 261(5128):1569–1571, 1993. \[174\] S. Lloyd. Universal quantum
simulators. Science, pages 1073–1078, 1996. \[175\] S. Lloyd, S.
Garnerone, and P. Zanardi. Quantum algorithms for topological and
geometric analysis of data. Nature Communications, 7(1):10138, Jan 2016.
\[176\] M. Loceff. A Course in Quantum Computing. 2015. \[177\] G. H.
Low and I. L. Chuang. Optimal hamiltonian simulation by quantum signal
processing. Physical review letters, 118(1):010501, 2017. \[178\] G. H.
Low and I. L. Chuang. Hamiltonian simulation by qubitization. Quantum,
3:163, Jul 2019. arXiv: 1610.06546. \[179\] L. Lu, J. D. Joannopoulos,
and M. Soljačić. Topological photonics. Nat. Photonics, 8:821–829, 2014.
\[180\] D. Lucas, C. Donald, J. P. Home, M. McDonnell, A. Ramos, D.
Stacey, J.-P. Stacey, A. Steane, and S. Webster. Oxford ion-trap quantum
computing

405

406

Works Cited

project. Philosophical Transactions of the Royal Society of London.
Series A: Mathematical, Physical and Engineering Sciences,
361(1808):1401–1408, 2003. \[181\] Y. Manin. Computable and
Non-Computable (in Russian). Sovetskoye Radio, Moscow, 1980. \[182\] Y.
I. Manin. Classical computing, quantum computing, and Shor’s factoring
algorithm. In Séminaire Bourbaki : volume 1998/99, exposés 850-864,
number 266 in Astérisque, pages 375–404. Société mathématique de France,
2000. \[183\] A. Marchenkova. Recorded video: Five quantum algorithms
that could change the world.
https://www.youtube.com/watch?v=\_54i80UFHSs. \[184\] I. L. Markov, A.
Fatima, S. V. Isakov, and S. Boixo. Quantum supremacy is both closer and
farther than it appears. arXiv:1807.10749 \[quant-ph\], Jul 2018. arXiv:
1807.10749. \[185\] E. Martin-Lopez, A. Laing, T. Lawson, R. Alvarez,
X.-Q. Zhou, and J. L. O’brien. Experimental realization of Shor’s
quantum factoring algorithm using qubit recycling. Nature Photonics,
6(11):773, 2012. \[186\] J. M. Martyn, Z. M. Rossi, A. K. Tan, and I. L.
Chuang. A grand unification of quantum algorithms. arXiv preprint
arXiv:2105.02859, 2021. \[187\] K. Mattle, H. Weinfurter, P. G. Kwiat,
and A. Zeilinger. Dense coding in experimental quantum communication.
Phys. Rev. Lett., 76:4656–4659, Jun 1996. \[188\] R. Maurand, X. Jehl,
D. Kotekar-Patil, A. Corna, H. Bohuslavskyi, R. Laviéville, L. Hutin, S.
Barraud, M. Vinet, M. Sanquer, et al. A CMOS silicon spin qubit. Nature
Communications, 7:13575, 2016. arXiv: 1605.07599.

Works Cited

\[189\] J. R. McClean, S. Boixo, V. N. Smelyanskiy, R. Babbush, and H.
Neven. Barren plateaus in quantum neural network training landscapes.
Nature Communications, 9(1):4812, 2018. \[190\] J. R. McClean, Z. Jiang,
N. C. Rubin, R. Babbush, and H. Neven. Decoding quantum errors with
subspace expansions. arXiv preprint arXiv:1903.05786, 2019. \[191\] J.
R. McClean, M. E. Kimchi-Schwartz, J. Carter, and W. A. de Jong. Hybrid
quantum-classical hierarchy for mitigation of decoherence and
determination of excited states. Physical Review A, 95(4):042308, 2017.
\[192\] J. R. McClean, I. D. Kivlichan, K. J. Sung, D. S. Steiger, Y.
Cao, C. Dai, E. S. Fried, C. Gidney, B. Gimby, P. Gokhale, et al.
Openfermion: the electronic structure package for quantum computers.
arXiv preprint arXiv:1710.07629, 2017. \[193\] J. R. McClean, J. Romero,
R. Babbush, and A. Aspuru-Guzik. The theory of variational hybrid
quantum-classical algorithms. New Journal of Physics, 18(2):023023,
2016. \[194\] N. D. Mermin. Quantum Computer Science: An Introduction.
Cambridge University Press, 2007. \[195\] A. Milsted, M. Ganahl, S.
Leichenauer, J. Hidary, and G. Vidal. TensorNetwork on TensorFlow: A
spin chain application using tree tensor networks. arXiv preprint
arXiv:1905.01331, 2019. \[196\] A. Milsted and G. Vidal. Tensor networks
as conformal transformations. arXiv preprint arXiv:1805.12524, 2018.
\[197\] S. Mittal, S. Ganeshan, J. Fan, A. Vaezi, and M. Hafezi.
Measurement of topological invariants in a 2d photonic system. Nature
Photonics, 10(3):180, 2016.

407

408

Works Cited

\[198\] S. Mittal and M. Hafezi. Topologically robust generation of
correlated photon pairs. arXiv preprint arXiv:1709.09984, 2017. \[199\]
M. Mohseni, P. Read, H. Neven, S. Boixo, V. Denchev, R. Babbush, A.
Fowler, V. Smelyanskiy, and J. Martinis. Commercialize quantum
technologies in five years. Nature News, 543(7644):171, 2017. \[200\] R.
Movassagh. Efficient unitary paths and quantum computational supremacy:
A proof of average-case hardness of random circuit sampling. arXiv
preprint arXiv: 1810.04681, Oct 2018. \[201\] S. Mullane. Sampling
random quantum circuits: a pedestrian’s guide. arXiv preprint
arXiv:2007.07872, 2020. \[202\] Y. Nakamura, Y. A. Pashkin, and J. Tsai.
Coherent control of macroscopic quantum states in a singleCooper-pair
box. Nature, 398(6730):786, 1999. arXiv: cond-mat/9904003. \[203\] Y.
Nakamura, Y. A. Pashkin, and J. S. Tsai. Rabi oscillations in a
Josephson-junction charge two-level system. Phys. Rev. Lett., 87:246601,
Nov 2001. \[204\] NAS. Quantum Computing: Progress and Prospects. The
National Academies Press, Washington, DC, 2018. \[205\] C. Neill, P.
Roushan, K. Kechedzhi, S. Boixo, S. V. Isakov, V. Smelyanskiy, A.
Megrant, B. Chiaro, A. Dunsworth, K. Arya, R. Barends, B. Burkett, Y.
Chen, Z. Chen, A. Fowler, B. Foxen, M. Giustina, R. Graff, E. Jeffrey,
T. Huang, J. Kelly, P. Klimov, E. Lucero, J. Mutus, M. Neeley, C.
Quintana, D. Sank, A. Vainsencher, J. Wenner, T. C. White, H. Neven, and
J. M. Martinis. A blueprint for demonstrating quantum supremacy with
superconducting qubits. Science, 360(6385):195–199, 2018.

Works Cited

\[206\] M. A. Nielsen and I. L. Chuang. Quantum Computation and Quantum
Information: 10th Anniversary Edition. Cambridge University Press, New
York, NY, USA, 10th edition, 2011. \[207\] nLab authors. Topological
quantum computation. http://ncatlab.org/nlab/show/topological
%20quantum%20computation, June 2021. Revision 18. \[208\] J. Noh, S.
Huang, D. Leykam, Y. D. Chong, K. P. Chen, and M. C. Rechtsman.
Experimental observation of optical Weyl points and Fermi arc-like
surface states. Nature Physics, 13(6):611, 2017. \[209\] N. Ofek, A.
Petrenko, R. Heeres, P. Reinhold, Z. Leghtas, B. Vlastakis, Y. Liu, L.
Frunzio, S. Girvin, L. Jiang, et al. Extending the lifetime of a quantum
bit with error correction in superconducting circuits. Nature,
536(7617):441, 2016. \[210\] J. Olson, Y. Cao, J. Romero, P. Johnson,
P.-L. Dallaire-Demers, N. Sawaya, P. Narang, I. Kivlichan, M.
Wasielewski, and A. Aspuru-Guzik. Quantum information and computation
for chemistry. arXiv preprint arXiv:1706.05413, 2017. \[211\] P. J.
O’Malley, R. Babbush, I. D. Kivlichan, J. Romero, J. R. McClean, R.
Barends, J. Kelly, P. Roushan, A. Tranter, N. Ding, et al. Scalable
quantum simulation of molecular energies. Physical Review X,
6(3):031007, 2016. \[212\] J. Otterbach, R. Manenti, N. Alidoust, A.
Bestwick, M. Block, B. Bloom, S. Caldwell, N. Didier, E. S. Fried, S.
Hong, et al. Unsupervised machine learning on a hybrid quantum computer.
arXiv preprint arXiv:1712.05771, 2017. \[213\] T. Ozawa, H. M. Price, A.
Amo, N. Goldman, M. Hafezi, L. Lu, M. Rechtsman, D. Schuster, J. Simon,
O. Zilberberg, et al. Topological photonics. arXiv preprint
arXiv:1802.04173, 2018.

409

410

Works Cited

\[214\] M. Ozols. Clifford group. Essays at University of Waterloo,
Spring, 2008. https://bit.ly/2JZe2jO. \[215\] D. P. Pappas, J. S. Kline,
F. da Silva, and D. Wisbey. Coherence in superconducting materials for
quantum computing. https://slideplayer.com/slide/7770332/. \[216\]
Pasqal. https://pasqal.io/2020/10/26/1329/. \[217\] Pennylane.
https://pennylane.ai/qml/demos/tutorial \_pasqal.html. \[218\] A.
Peruzzo et al. A variational eigenvalue solver on a quantum processor.
eprint. arXiv preprint arXiv:1304.3061, 2013. \[219\] W. Pfaff, B.
Hensen, H. Bernien, S. B. van Dam, M. S. Blok, T. H. Taminiau, M. J.
Tiggelman, R. N. Schouten, M. Markham, D. J. Twitchen, et al.
Unconditional quantum teleportation between distant solid-state quantum
bits. Science, 345(6196):532– 535, 2014. \[220\] H. Pichler, S.-T. Wang,
L. Zhou, S. Choi, and M. D. Lukin. Quantum optimization for maximum
independent set using rydberg atom arrays. arXiv preprint
arXiv:1808.10816, 2018. \[221\] J. M. Pino, J. M. Dreiling, C. Figgatt,
J. P. Gaebler, S. A. Moses, M. S. Allman, C. H. Baldwin, M. FossFeig, D.
Hayes, K. Mayer, and et al. Demonstration of the trapped-ion quantum-ccd
computer architecture. Nature, 592(7853):209–213, Apr 2021. arXiv:
2003.01293. \[222\] J. Preskill. Lecture notes for Physics 219/Computer
Science 219 at Caltech: Quantum Computation.
http://theory.caltech.edu/\~preskill/ph229/, 1997 \[223\] J. Preskill.
Quantum computing and the entanglement frontier. arXiv preprint
arXiv:1203.5813, 2012. \[224\] J. Preskill. Quantum computing in the
NISQ era and beyond. Quantum, 2:79, 2018. arXiv: 1801.00862.

Works Cited

\[225\] J. Preskill. Quantum computing 40 years later. 2021. arXiv:
2106.10522. \[226\] X.-L. Qi and S.-C. Zhang. Topological insulators and
superconductors. Reviews of Modern Physics, 83(4):1057, 2011. \[227\] X.
Qiang, X. Zhou, J. Wang, C. M. Wilkes, T. Loke, S. O’Gara, L. Kling, G.
D. Marshall, R. Santagati, T. C. Ralph, et al. Large-scale silicon
quantum photonics implementing arbitrary two-qubit processing. Nature
Photonics, 12(9):534, 2018. arXiv: 1809.09791. \[228\] Qiskit.
https://qiskit.org/textbook/ch-algorithms/
grover.html\#5.-Solving-Sudoku-using-Grover’sAlgorithm-. \[229\] R.
Raussendorf and H. J. Briegel. A one-way quantum computer. Physical
Review Letters, 86(22):5188, 2001. \[230\] R. Raussendorf and H. J.
Briegel. Computational model underlying the one-way quantum computer.
Quantum Information & Computation, 2(6):443– 486, 2002. \[231\] R.
Raussendorf, D. Browne, and H. Briegel. The one-way quantum computer–a
non-network model of quantum computation. Journal of Modern Optics,
49(8):1299–1306, 2002. \[232\] R. Raussendorf, D. E. Browne, and H. J.
Briegel. Measurement-based quantum computation on cluster states.
Physical review A, 68(2):022312, 2003. \[233\] M. C. Rechtsman, J. M.
Zeuner, Y. Plotnik, Y. Lumer, D. Podolsky, F. Dreisow, S. Nolte, M.
Segev, and A. Szameit. Photonic floquet topological insulators. Nature,
496(7444):196, 2013. \[234\] M. Reiher, N. Wiebe, K. M. Svore, D.
Wecker, and M. Troyer. Elucidating reaction mechanisms on

411

412

Works Cited

quantum computers. Proceedings of the National Academy of Sciences,
114(29):7555–7560, 2017. \[235\] D. Reitzner, D. Nagaj, and V. Buzek.
Quantum walks. Acta Physica Slovaca. Reviews and Tutorials, 61(6), Dec
2011. arXiv: 1207.7283. \[236\] E. G. Rieffel and W. H. Polak. Quantum
Computing: A Gentle Introduction. The MIT Press, 1 edition edition, Mar
2011. \[237\] E. Riehl. Category Theory in Context. Courier Dover
Publications, 2017. \[238\] A. Rivas and S. F. Huelga. Open Quantum
Systems: An Introduction. SpringerBriefs in Physics. SpringerVerlag,
2012. \[239\] R. L. Rivest, A. Shamir, and L. Adleman. A method for
obtaining digital signatures and public-key cryptosystems.
Communications of the ACM, 21(2):120– 126, 1978. \[240\] C. Roberts, A.
Milsted, M. Ganahl, A. Zalcman, B. Fontaine, Y. Zou, J. Hidary, G.
Vidal, and S. Leichenauer. TensorNetwork: A library for physics and
machine learning. arXiv preprint arXiv:1905.01330, 2019. \[241\] J.
Romero and A. Aspuru-Guzik. Variational quantum generators: Generative
adversarial quantum machine learning for continuous distributions. arXiv
preprint arXiv:1901.00848, 2019. \[242\] S. Rosenblum, Y. Y. Gao, P.
Reinhold, C. Wang, C. J. Axline, L. Frunzio, S. M. Girvin, L. Jiang, M.
Mirrahimi, M. H. Devoret, et al. A cnot gate between multiphoton qubits
encoded in two cavities. Nature Communications, 9(1):652, 2018. \[243\]
J. J. Rotman. Advanced Modern Algebra, volume 114. American Mathematical
Soc., 2010.

Works Cited

\[244\] E. Rowell and Z. Wang. Mathematics of topological quantum
computing. Bulletin of the American Mathematical Society, 55(2):183–238,
2018. \[245\] A. Roy and D. P. DiVincenzo. Topological quantum
computing. arXiv preprint arXiv:1701.05052, 2017. \[246\] M. Saffman, T.
G. Walker, and K. Mølmer. Quantum information with rydberg atoms.
Reviews of Modern Physics, 82(3):2313, 2010. \[247\] U. Schollwöck. The
density-matrix renormalization group. Reviews of Modern Physics,
77(1):259, 2005. \[248\] C. Schreyvogel, V. Polyakov, R. Wunderlich, J.
Meijer, and C. Nebel. Active charge state control of single NV centres
in diamond by in-plane Al-Schottky junctions. Scientific Reports,
5:12160, 2015. \[249\] E. Schrödinger. Discussion of probability
relations between separated systems. In Mathematical Proceedings of the
Cambridge Philosophical Society, volume 31, pages 555–563. Cambridge
University Press, 1935. \[250\] M. Schuld and N. Killoran. Quantum
machine learning in feature Hilbert spaces. Physical Review Letters,
122(4):040504, 2019. \[251\] M. Schuld and F. Petruccione. Supervised
learning with quantum computers. Springer, 2018. \[252\] H. M. Sheffer.
A set of five independent postulates for Boolean algebras, with
application to logical constants. Trans. Amer. Math. Soc., 14:481–488,
1913. \[253\] Y. Shi. Both Toffoli and controlled-NOT need little help
to do universal quantum computing. Quantum Information & Computation,
3(1):84–92, 2003. \[254\] P. Shor. Algorithms for quantum computation:
discrete logarithms and factoring. In Proceedings of the 35th Annual
Symposium on Foundations of Com-

413

414

Works Cited

puter Science, pages 124–134. IEEE Computer Society, 1994. \[255\] J. W.
Silverstone, D. Bonneau, J. L. O’Brien, and M. G. Thompson. Silicon
quantum photonics. IEEE Journal of Selected Topics in Quantum
Electronics, 22(6):390–402, 2016. \[256\] S. Sim, Y. Cao, J. Romero, P.
D. Johnson, and A. Aspuru-Guzik. A framework for algorithm deployment on
cloud-based quantum computers. arXiv preprint arXiv:1810.10576, 2018.
\[257\] D. R. Simon. On the power of quantum computation. In Proceedings
of the 35th Annual Symposium on Foundations of Computer Science, SFCS
’94, pages 116–123, Washington, DC, USA, 1994. IEEE Computer Society.
\[258\] A. Sipahigil, R. E. Evans, D. D. Sukachev, M. J. Burek, J.
Borregaard, M. K. Bhaskar, C. T. Nguyen, J. L. Pacheco, H. A. Atikian,
C. Meuwly, et al. An integrated diamond nanophotonics platform for
quantum optical networks. Science, page 6875, 2016. \[259\] S.
Slussarenko and G. J. Pryde. Photonic quantum information processing: a
concise review. Applied Physics Reviews, 6(4):041303, Dec 2019. arXiv:
1907.06331. \[260\] M. Smelyanskiy, N. P. Sawaya, and A. AspuruGuzik.
qHiPSTER: The quantum high performance software testing environment.
arXiv preprint arXiv:1601.07195, 2016. \[261\] R. S. Smith, M. J.
Curtis, and W. J. Zeng. A practical quantum instruction set
architecture. arXiv preprint arXiv:1608.03355, 2016. \[262\] R. Solovay
and V. Strassen. A fast monte-carlo test for primality. SIAM Journal on
Computing, 6(1):84– 85, Mar 1977.

Works Cited

\[263\] N. Spagnolo, C. Vitelli, M. Bentivegna, D. J. Brod, A. Crespi,
F. Flamini, S. Giacomini, G. Milani, R. Ramponi, P. Mataloni, and et al.
Efficient experimental validation of photonic boson sampling against the
uniform distribution. Nature Photonics, 8(8):615–620, Aug 2014. arXiv:
1311.1622. \[264\] G. Strang. Linear Algebra and Its Applications.
Cengage Learning, 2018. \[265\] Y. Su, D. W. Berry, N. Wiebe, N. Rubin,
and R. Babbush. Fault-tolerant quantum simulations of chemistry in first
quantization. arXiv preprint arXiv:2105.12767, 2021. \[266\] S. Sun, H.
Kim, Z. Luo, G. S. Solomon, and E. Waks. A single-photon switch and
transistor enabled by a solid-state quantum memory. arXiv preprint
arXiv:1805.01964, 2018. \[267\] S. Sun, H. Kim, G. S. Solomon, and E.
Waks. A quantum phase switch between a single solidstate spin and a
photon. Nature Nanotechnology, 11(6):539–544, 2016. \[268\] L. Susskind.
Dear qubitzers, GR = QM. arXiv preprint arXiv:1708.03040, 2017. \[269\]
M. Taha Rouabah. Compiling single-qubit braiding gate for fibonacci
anyons topological quantum computation. arXiv e-prints, 2020.
2008.03542. \[270\] J.-L. Tambasco, G. Corrielli, R. J. Chapman, A.
Crespi, O. Zilberberg, R. Osellame, and A. Peruzzo. Quantum interference
of topological states of light. Science Advances, 4(9):eaat3187, 2018.
\[271\] M. S. Tame, B. A. Bell, C. Di Franco, W. J. Wadsworth, and J. G.
Rarity. Experimental realization of a one-way quantum computer algorithm
solving Simon’s problem. Physical Review Letters, 113(20):200501, 2014.
arXiv: 1410.3859.

415

416

Works Cited

Recorded talk: On quan\[272\] E. Tang. tum linear algebra for machine
learning. https://www.youtube.com/watch?v=pd24cDR87Lw. \[273\] E. Tang.
A quantum-inspired classical algorithm for recommendation systems.
Electronic Colloquium on Computational Complexity (ECCC), 25:128, 2019.
\[274\] J. Timmer. Quantum-computing startup rigetti to offer modular
processors, Jun 2021. \[275\] T. Toffoli. Reversible computing. In
Proceedings of the 7th Colloquium on Automata, Languages and
Programming, pages 632–644, Berlin, Heidelberg, 1980. Springer-Verlag.
\[276\] I. Tzitrin, T. Matsuura, R. N. Alexander, G. Dauphinais, J. E.
Bourassa, K. K. Sabapathy, N. C. Menicucci, and I. Dhand. Fault-tolerant
quantum computation with static linear optics. arXiv:2104.03241
\[quant-ph\], Apr 2021. arXiv: 2104.03241. \[277\] S. B. van Dam, M.
Walsh, M. J. Degen, E. Bersin, S. L. Mouradian, A. Galiullin, M. Ruf, M.
IJspeert, T. H. Taminiau, R. Hanson, et al. Optical coherence of diamond
nitrogen-vacancy centers formed by ion implantation and annealing. arXiv
preprint arXiv:1812.11523, 2018. \[278\] L. M. Vandersypen, M. Steffen,
G. Breyta, C. S. Yannoni, M. H. Sherwood, and I. L. Chuang. Experimental
realization of Shor’s quantum factoring algorithm using nuclear magnetic
resonance. Nature, 414(6866):883, 2001. arXiv: quant-ph/0112176. \[279\]
M. Verbin, O. Zilberberg, Y. E. Kraus, Y. Lahini, and Y. Silberberg.
Observation of topological phase transitions in photonic quasicrystals.
Physical Review Letters, 110(7):076403, 2013. \[280\] M. Verbin, O.
Zilberberg, Y. Lahini, Y. E. Kraus, and Y. Silberberg. Topological
pumping over a pho-

Works Cited

tonic Fibonacci quasicrystal. Physical Review B, 91(6):064201, 2015.
\[281\] G. Verdon, J. Marks, S. Nanda, S. Leichenauer, and J. Hidary.
Quantum hamiltonian-based models and the variational quantum thermalizer
algorithm. arXiv preprint arXiv:1910.02071, 2019. \[282\] G. Verdon, T.
McCourt, E. Luzhnica, V. Singh, S. Leichenauer, and J. Hidary. Quantum
graph neural networks. arXiv preprint arXiv:1909.12264, 2019. \[283\] G.
Verdon, J. Pye, and M. Broughton. A universal training algorithm for
quantum deep learning. arXiv preprint arXiv:1806.09729, 2018. \[284\] F.
Verstraete and J. I. Cirac. Renormalization algorithms for quantum-many
body systems in two and higher dimensions. arXiv preprint
condmat/0407066, 2004. \[285\] G. Vidal. Entanglement renormalization.
Physical Review Letters, 99(22):220405, 2007. \[286\] J. von Neumann.
Mathematical Foundations of Quantum Mechanics. Springer, Berlin, 1932.
\[287\] C. Wang, F.-G. Deng, Y.-S. Li, X.-S. Liu, and G. L. Long.
Quantum secure direct communication with high-dimension quantum
superdense coding. Phys. Rev. A, 71:044305, Apr 2005. \[288\] D. Wang,
O. Higgott, and S. Brierley. A generalised variational quantum
eigensolver. arXiv preprint arXiv:1802.00171, 2018. \[289\] J. Wang, C.
Roberts, G. Vidal, and S. Leichenauer. Anomaly detection with tensor
networks. arXiv preprint arXiv:2006.02516, 2020. \[290\] Y. Wang, X.
Zhang, T. A. Corcovilos, A. Kumar, and D. S. Weiss. Coherent addressing
of individual neutral atoms in a 3d optical lattice. Physical Review
Letters, 115(4):043003, 2015. arXiv: arXiv:1504.02117.

417

418

Works Cited

\[291\] Z. Wang, Y. Chong, J. D. Joannopoulos, and M. Soljačić.
Observation of unidirectional backscatteringimmune topological
electromagnetic states. Nature, 461(7265):772, 2009. \[292\] T. Watson,
S. Philips, E. Kawakami, D. Ward, P. Scarlino, M. Veldhorst, D. Savage,
M. Lagally, M. Friesen, S. Coppersmith, et al. A programmable two-qubit
quantum processor in silicon. Nature, 555(7698):633, 2018. \[293\] D.
Wecker, M. B. Hastings, and M. Troyer. Progress towards practical
quantum variational algorithms. Physical Review A, 92(4):042303, 2015.
\[294\] D. S. Weiss and M. Saffman. Quantum computing with neutral
atoms. Phys. Today, 70(7):44, 2017. \[295\] S. R. White. Density matrix
formulation for quantum renormalization groups. Physical Review Letters,
69(19):2863, 1992. \[296\] N. Wiebe, D. Braun, and S. Lloyd. Quantum
data fitting. Physical Review Letters, 109(5):050505, Aug 2012. arXiv:
1204.5242. \[297\] K. Wiggers. Alphabet is repurposing Google TPUs for
quantum computing simulations.
https://venturebeat.com/2021/03/10/alphabet-isrepurposing-google-tpus-for-quantum-computingsimulations/,
Mar 2021. \[298\] P. Wittek. Quantum machine learning edX MOOC.
https://www.edx.org/course/quantummachine-learning-2, 2019. \[299\] P.
Wittek and C. Gogolin. Quantum enhanced inference in Markov logic
networks. Scientific Reports, 7:45672, 2017. \[300\] K. Wright, K. Beck,
S. Debnath, J. Amini, Y. Nam, N. Grzesiak, J.-S. Chen, N. Pisenti, M.
Chmielewski, C. Collins, et al. Benchmarking an 11-qubit quantum
computer. arXiv preprint arXiv:1903.08181, 2019.

Works Cited

\[301\] T.-Y. Wu, A. Kumar, F. Giraldo, and D. S. Weiss. Stern–Gerlach
detection of neutral-atom qubits in a state-dependent optical lattice.
Nature Physics, page 1, 2019. \[302\] Y. Wu, W.-S. Bao, S. Cao, F. Chen,
M.-C. Chen, X. Chen, T.-H. Chung, H. Deng, Y. Du, D. Fan, M. Gong, C.
Guo, C. Guo, S. Guo, L. Han, L. Hong, H.-L. Huang, Y.-H. Huo, L. Li, N.
Li, S. Li, Y. Li, F. Liang, C. Lin, J. Lin, H. Qian, D. Qiao, H. Rong,
H. Su, L. Sun, L. Wang, S. Wang, D. Wu, Y. Xu, K. Yan, W. Yang, Y. Yang,
Y. Ye, J. Yin, C. Ying, J. Yu, C. Zha, C. Zhang, H. Zhang, K. Zhang, Y.
Zhang, H. Zhao, Y. Zhao, L. Zhou, Q. Zhu, C.-Y. Lu, C.-Z. Peng, X. Zhu,
and J.-W. Pan. Strong quantum computational advantage using a
superconducting quantum processor. 2021. arXiv: 2106.14734. \[303\] L.
Xiao, X. Zhan, Z. Bian, K. Wang, X. Zhang, X. Wang, J. Li, K. Mochizuki,
D. Kim, N. Kawakami, et al. Observation of topological edge states in
parity–time-symmetric quantum walks. Nature Physics, 13(11):1117, 2017.
\[304\] J.-S. Xu, K. Sun, Y.-J. Han, C.-F. Li, J. K. Pachos, and G.-C.
Guo. Simulating the exchange of majorana zero modes with a photonic
system. Nature Communications, 7:13194, 2016. \[305\] Z. Xu, Z.-q. Yin,
Q. Han, and T. Li. Quantum information processing with closely-spaced
diamond color centers in strain and magnetic fields. Optical Materials
Express, 9(12):4654, Dec 2019. arXiv: 1909.11775. \[306\] T. J. Yoder,
G. H. Low, and I. L. Chuang. Fixed-point quantum search with an optimal
number of queries. Physical review letters, 113(21):210501, 2014.
\[307\] W. J. Zeng. Clarifying quantum supremacy: better terms for
milestones in quantum computation. Medium, Jan 31, 2019.
https://medium.com/@wjzeng/clarifying-quantum-

419

420

Works Cited

supremacy-better-terms-for-milestones-inquantum-computation-d15ccb53954f.
\[308\] Z. Zhao, J. K. Fitzsimons, and J. F. Fitzsimons. Quantum
assisted gaussian process regression. Physical Review A, 99(5):052331,
May 2019. arXiv: 1512.03929. \[309\] L. Zhou, S.-T. Wang, S. Choi, H.
Pichler, and M. D. Lukin. Quantum approximate optimization algorithm:
Performance, mechanism, and implementation on near-term devices. arXiv
preprint arXiv:1812.01041, 2018. \[310\] O. Zilberberg, S. Huang, J.
Guglielmon, M. Wang, K. P. Chen, Y. E. Kraus, and M. C. Rechtsman.
Photonic topological boundary pumping as a probe of 4D quantum Hall
physics. Nature, 553(7686):59, 2018.

Index

algorithms adiabatic, 156 amplitude amplification, 138
Bernstein-Vazirani, 16, 110 Deutsch’s, 16, 106 Deutsch-Jozsa, 16, 109
Grover’s, 18, 135 Shor’s, 18 Simon’s, 17 amplitude, 4, 26 ancilla, 87
ansatz, 143 Bell inequality test, 94 Bell state, 82, 87 Benioff, Paul,
15 bijective, 286 binary operator, 28 Bloch sphere, 38 Boolean function,
103 Born rule, 6, 31 Bourbaki, 286 BQP, 48 bra-ket notation, 377
Cartesian Product, 279 Church-Turing Thesis, 49 circuit depth, 38
circuit diagram, 27 Cirq, 70 CNOT, 33

complexity classes, 43 computation-in-place, 41 cryptography, 117 CSWAP,
35 dequantization, 174, 203 determinant, 328 Dirac notation, 377
distillation, 224 DiVincenzo Criteria, 19 dot product, 237 eigenvalues,
341 eigenvectors, 341 entanglement, 6 EPR, 6 EPR pair, 87 EQP, 48 error
correction, 215 Feynman, Richard, 15 Forest (Rigetti), 75 Fredkin
operator, 35 Gottesman-Knill, 37 groups, 294 Hadamard, 31 Hamiltonian,
9, 143, 151 Hermitian, 40, 350 Hilbert Space, 360 injective, 286

© The Author(s), under exclusive license to Springer Nature Switzerland
AG 2021 J. D. Hidary, Quantum Computing: An Applied Approach,
https://doi.org/10.1007/978-3-030-83274-2

421

422

Index

inner product, 240, 242, 364 irreversible computation, 12 Landauer’s
limit, 11 Manin, Yuri, 15 matrix, 254 matrix exponentiation, 270
measurement, 40 neutral atoms, 55 nitrogen-vacancy, 57 NMR, 56 NOT
operator, 36 NV center-in-diamond, 57 OpenFermion, 152 outer product,
25, 271 Pauli operators, 28 phase kickback, 107 phase shift operator, 30
photonic quantum computer, 58 polarization, 4 purification, 150 QAOA,
156 QDK, 77 QisKit, 72 QMA, 48 QML, 167 QPE, 174 QPU, 53 QRAM, 204 QSVT,
202 quantum advantage, 214 quantum chemistry, 151 quantum circuit, 27
quantum circuit simulation, 67, 81 quantum computer definition, 3
hardware, 53

quantum error correction, 215 quantum Fourier transform, 114 quantum
machine learning, 167 quantum phase estimation, 174 quantum simulation,
207 quantum singular value transform, 202 quantum supremacy, 208 quantum
teleportation, 87 quantum walks, 194 qubitization, 152 random circuit
sampling, 209 reversible computation, 37 RSA, 117 set theory, 276
Solovay-Kitaev, 37 spin qubits, 60 superconducting qubits, 61 superdense
coding, 90 superposition, 4 surjective, 286 tensor product, 273 ternary
operators, 34 Toffoli operator, 34 topological quantum computing, 63
trapped ion, 64 Trotterization, 151 unary operator, 28 uncomputing, 13,
182 unitary operators, 24, 353 universal computation, 37 vector space,
293 VQE, 143


