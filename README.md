# IAPL

The **Interval Algebra Problem Library (IAPL)** provides a set of problems for testing and benchmarking qualitative temporal reasoners based on Allen's Interval Algebra.

The problem library contains *consistent* problems from the following subalgebras:
1. [Batsakis et al.'s](https://content.iospress.com/articles/semantic-web/sw248) subalgebra (with 29 relations)
2. Pointisable subalgebra (with 187 relations)

The problem sources (in [GQR](https://www.sfbtr8.spatial-cognition.de/en/project/reasoning/r4-logospace/research-tools/gqr/index.html) format) are kept under [csps](csps). Their RDF/OWL versions together with associated questions are kept under the following directories:

| Dir                        | Subalgebra        | Format            |
| -------------------------- | ----------------- | ------------------|
| [batsakis-29](batsakis-29) | Batsakis et al.'s | Batsakis et al.'s |
| [timex-29](timex-29)       | Batsakis et al.'s | IBM `timex`       |
| [timex-187](timex-187)     | Pointisable       | IBM `timex`       |

### Problem names

Problems are named according to the following scheme:
```
p_<size>_d<degree>_s<rel-size>_<digest>.<ext>
```
where
* `size` is the number of intervals in the problem
* `degree` is the average degree of an interval of the problem
* `rel-size` is the average relation size of an edge of the problem
* `digest` is the md5 digest that uniquely identifies the problem
