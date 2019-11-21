# babette_example_7

Branch   |[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)                                                                                           |[![AppVeyor logo](pics/AppVeyor.png)](https://appveyor.com)                                                                                               
---------|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
`master` |[![Build Status](https://travis-ci.org/richelbilderbeek/babette_example_7.svg?branch=master)](https://travis-ci.org/richelbilderbeek/babette_example_7) |[![Build status](https://ci.appveyor.com/api/projects/status/0vrfbhulq2h3dg8i/branch/master?svg=true)](https://ci.appveyor.com/project/richelbilderbeek/babette-example-7/branch/master)
`develop`|[![Build Status](https://travis-ci.org/richelbilderbeek/babette_example_7.svg?branch=develop)](https://travis-ci.org/richelbilderbeek/babette_example_7)|[![Build status](https://ci.appveyor.com/api/projects/status/0vrfbhulq2h3dg8i/branch/develop?svg=true)](https://ci.appveyor.com/project/richelbilderbeek/babette-example-7/branch/develop)

A [babette example](https://github.com/richelbilderbeek/babette_examples).

## Example #7: HKY site model with a non-zero proportion of invariants

![Example #7: HKY site model with a non-zero proportion of invariants](hky_prop_invariant_0_5_2_4.png)

```{r}
posterior <- bbt_run(
  "my_alignment.fas",
  site_model = create_hky_site_model(
    gamma_site_model = create_gamma_site_model(prop_invariant = 0.5)
  )
)
```

Thanks to Yacine Ben Chehida for this use case

## Result

![](result.png)
