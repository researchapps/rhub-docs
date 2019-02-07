---
title: "How do R-hub and CRAN platforms compare?"
date: 2018-01-28T21:55:52+01:00
anchor: "rhub-cran-platforms"
weight: 15

---

You might want to know how R-hub and CRAN platforms compare in general, but that's especially crucial when you're using R-hub to reproduce a failure for submitting or keeping your package on CRAN. For different reasons, including the constant evolution of CRAN platforms, R-hub platforms are not exactly similar. 

If you run into an issue on CRAN that you want to reproduce we recommend

* Looking at settings of CRAN platforms via https://cran.r-project.org/web/checks/check_flavors.html,

* Looking at settings of R-hub platforms via `tibble::as.tibble(rhub::platforms())`,

* Running a check on the closest R-hub platform to the problematic CRAN platform.

* If that does not work, 
    * If you guess what causes the issue is e.g. the particular compiler and your package has compiled code, download the compiler and try reproducing the issue locally.
    * [Ask for help](#pkg-dev-help).
    
Good luck!