# Node Build Containers  
[TechnologyAdvice](http://www.technologyadvice.com) Node.js build environment

## What's this?
TechnologyAdvice launches a significant piece of our application stack into
lightweight Node.js Docker containers. The problem with lightweight containers
is that they often don't have the build tools necessary for development and
CI!

To support this, TechnologyAdvice engineers build on top of these containers,
and then deploy applications into slim boxes at a fraction of the size. These
build boxes use our deploy environment as the starting layer, to ensure
production compatibility.

## These are unsafe to use!
Please feel free to base your development or deploy environments off of ours,
but we discourage you from linking to these dockerfiles directly or using live
builds of these from Docker Hub, as they _will_ change in potentially
destructive ways to support our team's need-of-the-moment.

## License
All original content is Copyright (c) 2015 TechnologyAdvice, released under
the ultra-permissive ISC license. See LICENSE.txt for details.

