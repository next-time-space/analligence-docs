---
title: "Build Space"
---

# Build Space

So far we have setup all segments. Now it's time to build the craft script. Build is based out of workspace. We can create a build that consists of selected catalogs. Only the included catalogs will be captured when it's integrated. Including or excluding catalogs can be done doing one more build on top of existing build.

## Create build

(1) Click on **Build Space** from left navigation.

(2) Click on **Create New Build** button on top.

(3) Side bar will be opened and first step select all the catalogs you want to include in the craft script and click Next

(4) **Javascript Origins** is security check we don when we get the captured data. The origin has to be exact same your domain name. Our product intellisense will show you all possible origins from catalogs. Delete or add origins based on your domain name and click next.

(5) **Tag version** is required to create build version. It follows same version increment as npm.

(6) **Include JQuery Script** option allows us to include jquery from our repo or if you allow us to use your global jquery ($) definitions. Select based of it.

(7) After successful build it will show you new build version.

<img alt="Analligence Build" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_build.png">

_Be advised, sandbox environment old builds will be cleared automatically._

## Next step

Next step would be testing this craft script in local environment. Check out [Test Space](/docs/editors/test-space)