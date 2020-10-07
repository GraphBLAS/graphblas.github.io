# Goals and premises

The GraphBLAS Forum is an open effort to define standard building
blocks for graph algorithms in the language of linear algebra.

We believe that the state of the art in constructing a large
collection of graph algorithms in terms of linear algebraic operations
is mature enough to support the emergence of a standard set of
primitive building blocks.  We believe that it is critical to move
quickly and define such a standard, thereby freeing up researchers to
innovate and diversify at the level of higher level algorithms and
graph analytics applications.  This effort was inspired by the Basic
Linear Algebra Subprograms (BLAS) of dense Linear Algebra, and hence
our working name for this standard is “the GraphBLAS”.

A key insight behind this work is that when a graph is represented by
a sparse incidence or adjacency matrix, sparse matrix-vector
multiplication is a step of breadth first search.  By generalizing the
pair of scalar operations involved in the linear algebra computations
to define a semiring, we can extend the range of these primitives to
support a wide range of parallel graph algorithms.

# More information

A C reference implementation, SuiteSparse:GraphBLAS, can be downloaded
from [http://faculty.cse.tamu.edu/davis/suitesparse.html here].

Our 2013 manifesto for this project can be found
[http://www.netlib.org/utk/people/JackDongarra/PAPERS/GraphPrimitives-HPEC.pdf
here].

The mathematical definition of the GraphBLAS can be found
[http://www.mit.edu/~kepner/GraphBLAS/GraphBLAS-Math-release.pdf
here].

Background information about graphs in the language of linear algebra
can be found in the book: [http://bookstore.siam.org/se22/ Graph
Algorithms in the Language of Linear Algebra], edited by J. Kepner and
J. Gilbert, SIAM, 2011.

A straw man proposal for the GraphBLAS can be found
[http://gauss.cs.ucsb.edu/~aydin/combblas-r2.pdf here].

Gabor Szarnyas maintains a list of
[https://github.com/szarnyasg/graphblas-pointers GraphBLAS pointers]
with lots of tutorial material.


# Application Program Interface (API)

A [http://gauss.cs.ucsb.edu/~aydin/GABB17.pdf short paper from
IPDPSW'17] describes the rationale behind the C API design.

Version 1.0 (provisional) of the [[C language API]] is released on May
29, 2017 at the GABB workshop
[http://graphanalysis.org/workshop2017.html].

Version 1.1.0 (provisional) is released on November 14, 2017.  

Version 1.2.0 (final) is released on May 18, 2018. It can be
downloaded from
[http://people.eecs.berkeley.edu/~aydin/GraphBLAS_API_C_v12.pdf
here]. This is only available for archival purposes, you should use
the latest version 1.3.0 below.

Version 1.3.0 (final) is released on September 25, 2019. It can be
downloaded from
[http://people.eecs.berkeley.edu/~aydin/GraphBLAS_API_C_v13.pdf here].


# Reference Implementations

* SuiteSparse:GraphBLAS (latest version) can be downloaded from [http://faculty.cse.tamu.edu/davis/suitesparse.html here].

* [https://github.com/IBM/ibmgraphblas IBM GraphBLAS]


# Projects developing implementations of the GraphBLAS

* [https://people.eecs.berkeley.edu/~aydin/CombBLAS/html/index.html MPI/C++ Combinatorial BLAS (CombBLAS)]

* [http://graphulo.mit.edu Java Graphulo]

* [http://d4m.mit.edu Matlab/Octave D4M]

* [http://domino.research.ibm.com/library/cyberdig.nsf/papers/607AD69B638C3BEF85257DA10061EC97/$File/rc25508.pdf GPI (IBM)] and [https://github.com/IBM/ibmgraphblas IBM GraphBLAS]

* [https://github.com/narayanan2004/GraphMat/tree/distributed_primitives_integration GraphPad (Intel)]

* [https://github.com/cmu-sei/gbtl GraphBLAS Template Library (SEI/Indiana)]

* [http://faculty.cse.tamu.edu/davis/suitesparse.html SuiteSparse Graph BLAS (Texas A&M)]

* [https://github.com/gunrock/graphblast GraphBLAST (UC Davis and LBNL)]


# Graph analysis systems that integrate GraphBLAS

* [https://redislabs.com/redis-enterprise/redis-modules/redis-enterprise-modules/redisgraph/ RedisGraph: A Graph Database Module for Redis]

* [https://github.com/michelp/pggraphblas pggraphblas: High Performance Graph Processing with PostgreSQL]


# Workshops and conferences featuring the GraphBLAS (reverse chronological)

* [http://hpc.pnl.gov/grapl/ GrAPL 2020 @IPDPS]: Submission deadline February 1, 2020

*[https://sc19.supercomputing.org/session/?sess=sess319 SC2019 BOF on HPC Graph Toolkits and the GraphBLAS Forum]: Session is Wed 20 Nov, 5:15pm - 6:45pm

* [http://www.ieee-hpec.org/ HPEC 2019]: 

* [http://hpc.pnl.gov/grapl/ GrAPL 2019 @IPDPS]:

* [http://GraphChallenge.org/ GraphChallenge 2018]

* [http://ieee-hpec.org/2018/techprog2018.html HPEC 2018]

* [http://graphanalysis.org/workshop2018.html GABB 2018 @IPDPS]

* [http://graphchallenge.mit.edu/champions GraphChallenge 2017]

* [http://ieee-hpec.org/2017/techprog2017/sept13.htm HPEC 2017]

* [http://graphanalysis.org/workshop2017.html GABB 2017 @IPDPS]

* [http://ieee-hpec.org/2016/techprog2016/sept14.htm HPEC 2016]

* [http://meetings.siam.org/sess/dsp_programsess.cfm?SESSIONCODE=23074 Minisymposium 2016 @SIAM Annual Meeting]: [[SIAM Presentations]]

* [http://graphanalysis.org/workshop2016.html GABB 2016 @IPDPS]

* [http://www.ieee-hpec.org/2015/ HPEC 2015]

* [http://www.graphanalysis.org/workshop2015.html GABB 2015 @IPDPS]

* [http://www.ieee-hpec.org/2014/copy/agendatext.html HPEC 2014]

* [http://www.graphanalysis.org/workshop2014.html GABB 2014 @IPDPS]

* [http://ieee-hpec.org/2013/agenda.htm HPEC 2013]


# Blogs (and other interesting discussions) on GraphBLAS

* [http://aldenmath.com/blog Tim Davis's GraphBLAS blog]

* [https://github.com/GraphBLAS/LAGraph/issues/28#issuecomment-542952115 A good discussion thread on dropping explicit zeros (fall 2019)]

# GraphBLAS mailing list

If you wish to join our effort (or just watch it), please send an
email message to our [mailto:abuluc@lbl.gov mailing list coordinator].


# Steering Committee (alphabetical)

* [https://davidbader.net/ David Bader (NJIT)]

* [https://people.eecs.berkeley.edu/~aydin/ Aydin Buluc (Berkeley Lab)]

* [http://www.cs.ucsb.edu/~gilbert/ John Gilbert (UC Santa Barbara)]

* [http://www.mit.edu/~kepner/ Jeremy Kepner (MIT Lincoln Laboratory Supercomputing Center)]

* Tim Mattson (Intel)

* Henning Meyerhenke (KIT)
