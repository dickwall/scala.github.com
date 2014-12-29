---
layout: overview-large
title: Overview

partof: scaladoc
num: 1
outof: 3
---

#Scaladoc Overview

If you want to know how to use Scaladoc effectively, please jump
directly to [Scaladoc Usage](/overview/scaladoc/usage.html).

## Introduction

Scaladoc is documentation that lives with the code in comments that look
like this:

    /** Composes two instances of Function1 in a new Function1, 
      * with this function applied last.
      *
      *  @tparam A the type to which function `g` can be applied
      *  @param  g a function A => T1
      *  @return   a new function `f` such that 
      *               `f(x) == apply(g(x))`
      */
    def compose[A](g: A => T1): A => R = { 
      x => apply(g(x)) 
    }

The start of a Scaladoc comment is denoted by `/**` and is closed by
`*/`. Within the body of the comment, Type Parameters (`@tparam`),
function parameters (`@param`) and function returns (`@return`) are
commonly specified, along with a description of the function, class,
trait, object, field or anything else that the scaladoc comment
applies to.

During the build and deployment process, these documents are collected,
verified by the compiler (in as much as the parameters, types and
returns are checked against the actual code) and formatted into
the API documentation you see for many Scala projects, including
Scala's own core libraries.

### Contributing to Scaladoc

If you are interested in contributing to Scaladoc for the core libraries
please read the [Basics Guide](/overview/scaladoc/basics.html) first, 
then see our [Scaladoc Contribution Guide](/overview/scaladoc) which covers
the steps necessary to clone the repository and work on the documentation.

### Using Scaladoc

If you are interested in Scaladoc from a usage perspective, take a look
at the [Scaladoc Usage](/overview/scaladoc/usage.html) page which covers
many of the extended features of Scaladoc you may not be aware of.

