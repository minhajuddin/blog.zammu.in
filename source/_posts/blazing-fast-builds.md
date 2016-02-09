title: Blazing fast builds
date: 2016-02-09 18:19:28
tags:
- Speed
---

We have started caching our npm packages and gems to speed up the builds. This
has yielded us an impressive speed up of in our deploys. Now, whenever you add a
site for the first time it caches the gems or npm packages which are used by
your blog/site. The next time you run the build it uses this cache so that it
doesn't have to install the gems or npm packages.

I am very happy with the results, The speedups are really impressive.

| Static Site Generator | Previous Build time  | Current Build time | % increase in performance |
| --                    | --                   | --                 | --                        |
| Hexo                  | 30 seconds           | 9 seconds          | 233%                      |
| Jekyll                | 30 seconds           | 5 seconds          | 500%                      |
| Middleman             | 2 minutes 30 seconds | 7 seconds          | 2042%                     |
| Octopress             | 1 minute 15 seconds  | 9 seconds          | 733%                      |
| Hugo                  | 3 seconds            | 3 seconds          | 0%                        |

One thing to note is the speed of Hugo, it has always been fast :)
