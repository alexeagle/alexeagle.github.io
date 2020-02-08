---
layout: home
---

🐙 [github.com/alexeagle](https://github.com/alexeagle)
|
🐦 [twitter.com/jakeherringbone](http://twitter.com/jakeherringbone)

> Last updated January 2020

# Summary

Googler since 2008, passionate about 
developer productivity via toolchain ergonomics, 
refined developer experience, 
and expert tooling.

World-class Expert in Bazel build system, https://bazel.build

Professional programmer for 23 years.

Open-source advocate and public speaker.

# Major Achievements

Created [Error Prone](https://errorprone.info), a static analysis plugin for the Java compiler that detects many classes of programming mistakes.
While working with [Findbugs](http://findbugs.sourceforge.net/) author, I realized we could host the analysis in the compiler itself. Rolled out stricter compiler across Google monorepo by creating a MapReduce framework that runs the compiler in "fix mode" across all compilations in parallel. This effort became a staffed team, has over 600 checks and has prevented thousands of bugs including some severe ones.

Added [JavaScript support](https://github.com/bazelbuild/rules_nodejs) to the [Bazel] build tool, allowing development of Web and Node.js server apps. Open-sourced Google's TypeScript/Angular build and serve toolchain. This has thousands of users including some large enterprises.

Migrated the Angular project to TypeScript, made TypeScript an official Google language and wired Angular development into Google's toolchain.

Led Google-scale infrastructure to run continuous integration for nearly all Google projects and GUI to show all build and test results.

# Work Experience

## Google, 11 years

| Time period          |  Perf rating  |
| -------------------- | ------------- |
| 2016 Q3 – 2017 Q1    | Exceeds Expectations |
| 2017 Q3 – 2018 Q3    | Strongly Exceeds |
| 2019 Q1 – Q3         | Superb |

### BazelWeb

[Bazel] is a general-purpose build tool used for all nearly software at Google.

I wrote the Angular support used both internally and publicly. I also wrote the public version of JavaScript plugin (rules), including Node.js runtime, TypeScript compilation, and serving and testing integration. This is a comprehensive set of integrations for building and testing complete full-stack applications.

According to Google's metrics, rules_nodejs is the most popular Bazel plugin, with over 20k daily downloads.
A summary of my work is on [rules_nodejs contributors](https://github.com/bazelbuild/rules_nodejs/graphs/contributors)

### Angular

Tech Lead for Angular CLI and Tooling (1.5M users).

Led DevInfra work such as syncing code changes between GitHub and Google-internal repo.

Converted Angular itself to TypeScript.

Migrated Angular to Build&Test with Bazel, along with its ecosystem (Material components, ngrx, Angular Universal). 87% reduction in Angular's CI latency.

### TypeScript

Founding member of team that implemented TypeScript as a supported language in Google. Wrote Bazel integrations, tooling for making TypeScript edits across the entire monorepo. Implemented tslint across Google's code, built into code review tool.

Wrote third-party strictness checker to build into the TypeScript compiler, https://tsetse.info. This is modelled on my very successful project Error Prone which does the same for Java.

### Google-wide continuous integration (TAP)

This is Google's CI, based on running Bazel and Remote Build Execution on a massive cluster. Led the migration of project definitions to a Maven-like format, improved team processes and testing practices.

Tech Lead for two years.

### Bazel Results UI (Sponge)

This service automatically injests event data from all Bazel executions and presents results in a GUI.
Allows more intuitive comprehension of build and test failures, troubleshooting slow builds, sharing permalink when requesting help.

Tech Lead for one year.

## Opower, 1 year

As employee #2 I got to build the UI for the company's flagship "Home energy reports" product.
This was rendered onto paper and served by the US Postal Service!
The company was later acquired by Oracle for $50M

## Earlier employment
See my [LinkedIn profile](https://www.linkedin.com/in/alexeagle) for employment history 1997-2007.

# Education

- Harvard: B.A. in Computer Science, Magna cum Laude _(2001)_
- Boy Scouts of America: Eagle Scout

# Talks and Publications

**Blog**

[dev.to/jakeherringbone](https://dev.to/jakeherringbone)
(prior to September 2019: [medium.com/@jakeherringbone](https://medium.com/@jakeherringbone))

**Publications**

- Communications of the ACM: [Lessons from Building Static Analysis Tools at Google](https://cacm.acm.org/magazines/2018/4/226371-lessons-from-building-static-analysis-tools-at-google/fulltext) _(April 2018)_
- Testing on the Toilet: [Change-Detector Tests Considered Harmful](https://testing.googleblog.com/2015/01/testing-on-toilet-change-detector-tests.html) _(January 2015; Won "flushy" award for top 4 articles of the year.)_

**Conference Talks**

- BazelCon 2019: Bazel Migration Patterns [🎬](https://www.youtube.com/watch?v=UwuRGpVpmbo&list=PLxNYxgaZ8Rsf-7g43Z8LyXct9ax6egdSj&index=35&t=0s)
- BazelCon 2019: Lightning talk "Why not to have Bazel Dependencies [🎬](https://www.youtube.com/watch?list=PLxNYxgaZ8Rsf-7g43Z8LyXct9ax6egdSj&v=2KzOLddhdoI)
- ng-conf 2019: The Bazel opt-in preview is here [🎬](https://www.youtube.com/watch?v=J1lnp-nU4wM)
- BazelCon 2018: Building Large Angular Apps with Bazel [🎬](https://www.youtube.com/watch?v=yBg9zG6ZGb4)
- ng-conf 2018: Full Stack development with Nx and Bazel [📚](https://docs.google.com/presentation/d/1fSZwcpO9hUBFd_k9hUS45ZyVJcZLEyz0VxISSOnIZ1I/preview) [🎬](https://www.youtube.com/watch?v=1KDDIhcQORM) _(April 2018)_
- Google Cloud Next: Building Apps Like Google with Angular, Bazel, and GCP [🎬](https://www.youtube.com/watch?v=lDyIc2Abkwg) _(April 2019)_
- AngularMIX: Develop Angular like Google Does [📚](https://docs.google.com/presentation/d/1b0PdG-bxN0nwHa3ZuA0a_anOEYeMoI_CSsZl6ngZWp8/preview?slide=id.g26d86d3325_0_0) _(October 2018)_

**Meetup Talks**

- ModernWeb Meetup: Layering in JS tooling [📚](https://hackmd.io/p/HJZ_ekxuN) [🎬](https://drive.google.com/file/d/1AxrwjLUf_35Z2C9VK5Ut7wo5L89roHH2/view) _(March 2019)_
- AngularNYC Meetup: Bazel in Angular CLI [🎬](https://www.youtube.com/watch?v=fEUgZopCK8E) [📚](https://docs.google.com/presentation/d/1VcSkWDFkmkZKCP9yTfKbq-lTMU3qW_3zNabKItCWDec/preview) _(January 2019)_

[Bazel]: https://bazel.build
