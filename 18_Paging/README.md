## 1
~~~
By increasing the addressspace with a constant page size the size of pagetable increases by factor 2^n
And by increasing the page size with a constant addressspace size the pagetable decreases by factor 2^n
When having really big pages the effiency of having a pagetable is getting lost. Because then you have a really big offset and have to alot of comparisons.
~~~

## 2

~~~
More and more PTE will get valid. Therefore all virtual addresses will be valid
~~~

## 3

~~~
1. In a real computer system there is never such a small address space

2. The problem with these parameters is that the physical memory is 1m and the address space is only 32k. This means that a very small
fraction of the address space is mapped to a really big physical memory.

3. These parameters are completely unrealistic because the addressspace is only the half of the physical memory.
Furthermore the pages have a size of only 1m in a pagetable with the size of 256m. Therefore there can be 256 PTEs.
~~~