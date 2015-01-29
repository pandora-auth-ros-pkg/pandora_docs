# PANDORA documentation repo | [Wiki](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki)

This repo is intended for documentation files such as images, UML diagrams, pdfs and more. 
If you add a UML diagram, consider uploading the original file (.zargo, .vsdx, .dia, etc) as well as images and pdfs for that diagram in order to be easily downloadable and viewable. 
In case you need to upload an image in order to use it from the wiki, you should upload that image directly to the wiki repo. 
Clone the `https://github.com/pandora-auth-ros-pkg/pandora_docs.wiki.git` repo and you will find a folder named `images` in it.

## Quick links

- [Wiki home](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki)
- [Setting up packages](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki/Setup%20Packages)
- [Coding guidelines](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki/Coding-Guidelines)

## API documentation and Jenkins builds

|       Metapackage     |                             API Documentation                             | Jenkins build | Build status* |
| --------------------- | :------------------------------------------------------------------------:|:-----------:|:-------:|
| pandora_common        | -                                                                         | [Job](http://jenkins.pandora.ee.auth.gr/job/test-pandora_common/) | [![Build Status](http://jenkins.pandora.ee.auth.gr/buildStatus/icon?job=test-pandora_common/hydro-devel)](http://jenkins.pandora.ee.auth.gr/job/test-pandora_common/branch/hydro-devel/) |
| pandora_data_fusion   | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_data_fusion/html/)  | [Job](http://jenkins.pandora.ee.auth.gr/job/test-pandora_data_fusion/) | [![Build Status](http://jenkins.pandora.ee.auth.gr/buildStatus/icon?job=test-pandora_data_fusion/hydro-devel)](http://jenkins.pandora.ee.auth.gr/job/test-pandora_data_fusion/branch/hydro-devel/) |
| pandora_fsm           | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_fsm/html/)          | -           | - |
| pandora_vision        | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_vision/html/)       | [Job](http://jenkins.pandora.ee.auth.gr/job/test-pandora_vision/)        | [![Build Status](http://jenkins.pandora.ee.auth.gr/buildStatus/icon?job=test-pandora_vision/hydro-devel)](http://jenkins.pandora.ee.auth.gr/job/test-pandora_vision/branch/hydro-devel/) |
| pandora_visualization | -                                                                         | [Job](http://jenkins.pandora.ee.auth.gr/job/test-pandora_visualization/)    | [![Build Status](http://jenkins.pandora.ee.auth.gr/buildStatus/icon?job=test-pandora_visualization/hydro-devel)](http://jenkins.pandora.ee.auth.gr/job/test-pandora_visualization/branch/hydro-devel/) |

*hydro-devel
