mist
====

Safety checker for Petri Nets (and some extensions)

% last updated: Sat Feb  9 20:53:10 CET 2013

COMPILATION
-----------

To compile:
   './configure'
   'make'

You can optionally install the package (in /usr/local/bin) with
root privileges:
   'make install'

To uninstall:
   'make uninstall'


EXECUTION
---------

The runnable file are in 'src/':
   'src/mist'
   or 'mist' if you installed the package.

Running:
   'mist --<algorithm> <input_file>'


CONTEXT
-------

mist provides a set of functions together with a data structure (IST that
stands for Interval Sharing Tree) to manipulate interval constraints in a
multi-dimensional space.  Additionnaly to the traditional operations on sets,
some operations are specialized to verification of MTNs (an extension of the
Petri Net formalism). MTN is a infinite state model for finite abstraction of
Java multi-threaded programs. In fact, each thread can be viewed as a finite
automata for which an abitrary number of instances can be considered.

REFERENCES
----------

For the original sharing tree data structure

- [Zam97]	Denis Zampuniéris' Ph.D. Thesis The Sharing Tree Data Structure
Theory and Applications in Formal Verification University of Namur (Belgium)
May 1997 

Denis Zampuniéris is the original author of a data structure called "Sharing
Tree".  Our "Interval Sharing Tree" as well as the "Covering Sharing Tree" of
G. Delzanno, J.F. Raskin, L. Van Begin are extension of the "Sharing Tree" data
structure. Further reading on CST:

- [DRV04] Giorgio Delzanno, Jean-François Raskin and Laurent Van Begin. CSTs (Covering Sharing Trees):  compact Data Structures for Parameterized Verification. Will appear in Software Tools for Technology Transfer manuscript, 2004.

- [Van03] Laurent Van Begin, Ph.D Thesis Efficient Verificaition of
Counting Abstraction.  Université Libre de Bruxelles. 2003.

Further reading on IST:

- [GMD+07] Pierre Ganty, Cédric Meuter, Giorgio Delzanno, Gabriel Kalyon, Jean-François Raskin, Laurent Van Begin. Symbolic Data Structure for sets of k-uples. Technical Report 570, Université Libre de Bruxelles, 2007.

- [Gan02] Pierre Ganty's  Master Thesis. (in French) Algorithmes et
structures de données efficaces pour la manipulation de contraintes sur les
intervalles. Université Libre de Bruxelles. 2002.

MAIN AUTHOR COORDINATES
-----------------------

pierreganty@gmail.com
