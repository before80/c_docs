+++
title = "termsDefinitionsAndSymbols"
weight = 30
date = 2023-06-28T20:12:01+08:00
description = ""
isCJKLanguage = true
draft = false
+++

# Terms, definitions, and symbols

 

For the purposes of this document, the terms and definitions given in ISO/IEC 2382, ISO 80000–2,and the following apply. 

ISO and IEC maintain terminological databases for use in standardization at the following addresses:

- ISO Online browsing platform: available at https://www.iso.org/obp

- IEC Electropedia: available at http://www.electropedia.org/

 

Additional terms are defined where they appear in *italic* type or on the left side of a syntax rule.Terms explicitly defined in this document are not to be presumed to refer implicitly to similar termsdefined elsewhere.

## 3.1 access (verb)

<execution-time action> to read or modify the value of an object

 

**Note 1 to entry:** Where only one of these two actions is meant, "read" or "modify" is used. 

**Note 2 to entry:** "Modify" includes the case where the new value being stored is the same as the previous value. 

**Note 3 to entry:** Expressions that are not evaluated do not access objects.

## 3.2 alignment

requirement that objects of a particular type be located on storage boundaries with addresses that are particular multiples of a byte address

### 3.3 argument

actual argument

DEPRECATED: actual parameter

expression in the comma-separated list bounded by the parentheses in a function call expression, or a sequence of preprocessing tokens in the comma-separated list bounded by the parentheses in a function-like macro invocation

## 3.4 behavior

external appearance or action

### 3.4.1 implementation-defined behavior

unspecified behavior where each implementation documents how the choice is made 

**Note 1 to entry:** J.3 gives an overview over properties of C programs that lead to implementation-defined behavior. 

**EXAMPLE** 

An example of implementation-defined behavior is the propagation of the high-order bit when a signed integer is shifted right.

### 3.4.2 locale-specific behavior

behavior that depends on local conventions of nationality, culture, and language that each implementation documents



**Note 1 to entry:** J.4 gives an overview over properties of C programs that lead to locale-specific behavior.

**EXAMPLE** An example of locale-specific behavior is whether the **islower** function returns true for characters other than the 26 lowercase Latin letters.

**3.4.3****undefined behavior**

behavior, upon use of a nonportable or erroneous program construct or of erroneous data, for which this document imposes no requirements

**Note 1 to entry:** Possible undefined behavior ranges from ignoring the situation completely with unpredictable results, to behaving during translation or program execution in a documented manner characteristic of the environment (with or without the issuance of a diagnostic message), to terminating a translation or execution (with the issuance of a diagnostic message).

**Note 2 to entry:** J.2 gives an overview over properties of C programs that lead to undefined behavior.

**EXAMPLE** An example of undefined behavior is the behavior on integer overflow.

**3.4.4****unspecified behavior**

behavior, that results from the use of an unspecified value, or other behavior upon which this document provides two or more possibilities and imposes no further requirements on which is chosen in any instance

**Note 1 to entry:** J.1 gives an overview over properties of C programs that lead to unspecified behavior.

**EXAMPLE** An example of unspecified behavior is the order in which the arguments to a function are evaluated.

**3.5****bit**

unit of data storage in the execution environment large enough to hold an object that can have one of two values

**Note 1 to entry:** It need not be possible to express the address of each individual bit of an object.

**3.6****byte**

addressable unit of data storage large enough to hold any member of the basic character set of the execution environment



**Note 1 to entry:** It is possible to express the address of each individual byte of an object uniquely.

**Note 2 to entry:** A byte is composed of a contiguous sequence of bits, the number of which is implementation-defined. The

least significant bit is called the *low-order bit*; the most significant bit is called the *high-order bit*.

**3.7****character**

*⟨*abstract*⟩* member of a set of elements used for the organization, control, or representation of data

**3.7.1****character**

single-byte character

*⟨*C*⟩* bit representation that fits in a byte

**3.7.2** **multibyte character**

sequence of one or more bytes representing a member of the extended character set of either the source or the execution environment

**Note 1 to entry:** The extended character set is a superset of the basic character set.