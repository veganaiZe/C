[<img width="42px" src="https://user-images.githubusercontent.com/7102064/159596043-1a7a3e4d-abdb-4023-9ec7-ac934ef8f69e.png"
alt="C" /> programming](https://en.cppreference.com/w/c)
=======================

_Quick reference for C fundamentals_


[Language](https://en.cppreference.com/w/c/language.html)
----------

* [Keywords](https://en.cppreference.com/w/c/keyword.html)
* [Operator Precendence](https://en.cppreference.com/w/c/language/operator_precedence.html)
* Reserved Names: ([cppreference](https://en.cppreference.com/w/c/language/identifiers.html#Reserved_identifiers) / [gnu libc manual](https://www.gnu.org/software/libc/manual/html_node/Reserved-Names.html) / [c99 7.1.3](https://www.open-std.org/jtc1/sc22/wg14/www/docs/n1256.pdf#page=178))
    ```C
    /* All keywords & standard library names are reserved. */
    
    extern _reserved;               /* extern _(a-z..)                       */
    void _Reserved, __reserved;     /* _(A-Z) and __(a-z|A-Z)                */

    void E;                         /* E(0-9..) and E(A-Z..)                 */
    void issomething, tosomething;  /* is(a-z..) and to(a-z..)               */
    void LC_;                       /* LC_(A-Z..)                            */
    void somethingf, somethingl;    /* (a-z..)f and (a-z..)l                 */
    void SIG, SIG_;                 /* SIG(A-Z..) and SIG_(A-Z..)            */
    void mem, str, wcs;             /* mem(a-z..) and str(a-z..), wcs(a-z..) */
    void _t;                        /* (a-z..)_t                             */

    void l_, F_, O_, S_;            /* l_(..), F_(..), O_(..), S_(..); `fcntl.h` */
    void _MAX;                      /* (..)_MAX; `limits.h`                      */

    /* All others prefixed with `_` always reserved for file-scope usage (including tag name spaces). */
    ```


[Input / Output](https://en.cppreference.com/w/c/io.html)
----------------

* [printf](https://en.cppreference.com/w/c/io/fprintf.html)


[Memory Management](https://cppreference.net/c/memory.html)
-------------------

```C
#include <stdlib.h>

void * calloc(size_t element_count, size_t element_size);  /* Dynamically allocate `0` initialized memory block; NULL on failure */
void   free(void * dynamic_memory_block);  /* NULL pointer does nothing; undefined if already freed */
void * malloc(size_t size_bytes);  /* Dynamically allocate uninitialized memory block; NULL on failure */
void * realloc(void * dynamic_memory_block, size_t new_size_bytes);  /* Effectively resize memory block; NULL on failure */
```


[Preprocessor](https://en.wikipedia.org/wiki/C_preprocessor)
--------------

* [Header Include Guards](https://en.wikipedia.org/wiki/Include_guard)
    ```C
    #ifndef FILENAME_H
    #define FILENAME_H
        /*...*/
    #endif  /* FILENAME_H */
    ```
* [Effective Block Comment](https://gcc.gnu.org/onlinedocs/cpp/Deleted-Code.html) (Compatible with nested `/*...*/` comments but needs balanced single quotes.)
    ```C
    #if 0
        /*...*/
    #endif
    ```


[Search & Sort](https://en.cppreference.com/w/c/algorithm)
---------------

```C
#include <stdlib.h>

/* qsort, despite name, is NOT required to implement quicksort -- no complexity or stability guarantees. */
void qsort(void * array,
           size_t element_count,  /* sizeof array / sizeof *array */
           size_t element_bytesize,  /* sizeof *array */
           int (*compare_function)(const void * a, const void * b));  /* returns value <, >, or == 0 */

/* bsearch, despite name, is NOT required to implement binary search -- no complexity guarantees. */
void * bsearch(const void * keyword,
               const void * array,
               size_t element_count,  /* sizeof array / sizeof *array */
               size_t element_bytesize,  /* sizeof *array */
               int (*compare_function)(const void * keyword, const void * element));  /* returns value <, >, or == 0 */


int compare_ints(const void * a, const void * b)
{
    int x = *(const int*)a;
    int y = *(const int*)b;

    return x < y ? -1 : x > y ? 1 : 0;
}
```


[Strings](https://en.cppreference.com/w/c/string.html)
---------

```C
#include <string.h>

size_t strlen(const char * string);  /* returns length; upto but not including null character '\0' */
```
